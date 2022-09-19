# Node-red server/proxy for Sofar inverters
- subflow captures messages from wifi logger and decode them into JSON message
- proxy data to default (solarmanpv.com (ginlong.com)) server
- uses v5 data frames

## Tested on:

- LSW-3 data logger (`SN: 17xxxxxxxx` `firmware: LSW3_14_FFFF_1.0.34`) and **Sofar 4.4KTL-X**  
- **Sofar ME3000SP (RETROFIT ZST-3000SP)** added by [mattiarossi](https://github.com/mattiarossi)  
- **Sofar HYD6000-ES** added by [daniel-pro](https://github.com/daniel-pro)  

## wifi logger settings

go to `http://\<wifi logger local IP\>`  
in advanced tab set server B to `<node-red IP>` on port `10000` `TCP`  
![advanced settings](images/wifi-logger-advanced-settings.png)  

## node-red settings

import [node-red-subflow](node-red-subflow.json) to node-red, u will get sofar inverter node in subflow category  
![subflow example](images/subflow-node-example.png)  
now your `sofar inverter` node should have 1 connection and receive data  

`sofar inverter` default properties  
![subflow properties](images/subflow-properties.png)  
by default node will listen on TCP port 10000, and will resend data to default solarmanpv.com server as well  

## node-red did not connect

if `sofar inverter` node do not have active connection  
go to `http://\<wifi logger local IP\>/config_hide.html`  
and change server A (default server) to `<node-red IP>`  
![advanced settings](images/wifi-logger-hidden-menu.png)  

---
## messages flow

### after power on:

wifi logger ([hello msg](messages/decode_hello-msg.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([KTL-X](messages/decode_data_KTL-X.md)/[ME3000SP](messages/decode_data_me3000sp.md)/[HYD6000ES](messages/decode_data_HYD6000ES.md) data msg) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([hello cd msg](messages/decode_hello_cd-msg.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([hello end msg](messages/decode_hello_end-msg.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  

### 120s interval:

wifi logger ([heartbeat msg](messages/decode_heartbeat.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger

### 5min interval:

wifi logger ([KTL-X](messages/decode_data_KTL-X.md)/[ME3000SP](messages/decode_data_me3000sp.md)/[HYD6000ES](messages/decode_data_HYD6000ES.md) data msg) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  

### ~3h interval:

wifi logger ([hello msg](messages/decode_hello-msg.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([KTL-X](messages/decode_data_KTL-X.md)/[ME3000SP](messages/decode_data_me3000sp.md)/[HYD6000ES](messages/decode_data_HYD6000ES.md) data msg) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([hello cd msg](messages/decode_hello_cd-msg.md)) -> server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger  
wifi logger ([hello end msg](messages/decode_hello_end-msg.md)) ->server ([srv-response msg](messages/decode_srv-response.md)) -> wifi logger

### other messages:

sended after some connection problems (presumably)  
[60bytes msg](messages/decode_60.md) and [44bytes msg](messages/decode_44.md)  
