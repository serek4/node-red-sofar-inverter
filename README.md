# Sofar wifi stick communication with ginlong.com (solarmanpv.com) server

## wifi stick:

    SN: 174xxxxxxx
    firmware: LSW3_14_FFFF_1.0.34

## node-red settings

import `node-red-flow.json` in node-red  
![advanced settings](/images/node-red-KTL-X-server-flow.png)  

## wifi stick settings

go to http://\<wifi stick local IP\>  
in advanced tab set server B to `<node-red IP>` on port `10000` `TCP`  
![advanced settings](/images/wifi-stick-advanced-settings.png)  

thats it.

## but if node-red did not connect to inverter

if `Inverter stick out(TCP in node)` did not connect  
go to http://\<wifi stick local IP\>/config_hide.html  
and change server A (default server) to `<node-red IP>`  
![advanced settings](/images/wifi-stick-hiden-menu.png)  

if you want to still send data to solarmanpv.com (or m.ginlong.com) site aswell  
you can disconnect `generate response(function node)`   
and connect `solarmanpv.com(TCP request node)` instead 
![advanced settings](/images/node-red-KTL-X-proxy-flow.png)  

---
## messages flow

### after power on:

wifi stick (hello msg) -> ginlong server (srv-response) -> wifi stick  
wifi stick (data) -> ginlong server (srv-response) -> wifi stick  
wifi stick (41) ->ginlong server (srv-response) -> wifi stick  
wifi stick (73) ->ginlong server (srv-response) -> wifi stick  

### 120s interval:

wifi stick (heartbeat) ->ginlong server (srv-response) -> wifi stick

### 5min interval:

wifi stick (data) -> ginlong server (srv-response) -> wifi stick

### ~3h interval:

wifi stick (hello msg) -> ginlong server (srv-response msg) -> wifi stick  
wifi stick (data msg) -> ginlong server (srv-response msg) -> wifi stick  
wifi stick (41bytes msg) ->ginlong server (srv-response msg) -> wifi stick  
wifi stick (73bytes msg) ->ginlong server (srv-response msg) -> wifi stick
