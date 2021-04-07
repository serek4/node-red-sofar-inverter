# Sofar wifi stick communication with ginlong.com (solarmanpv.com) server

## wifi stick:

    SN: 174xxxxxxx
    firmware: LSW3_14_FFFF_1.0.34

## node-red settings

import `node-red-flow.json` in node-red

it is setup to get messages from inverter and send them to solarmanpv.com aswell  
if you don't want to use home.solarman.cn (or m.ginlong.com) site  
you can disconnect `solarmanpv.com(TCP request node)`  
and connect `generate response(function node)` instead

## wifi stick settings

go to http://\<wifi stick local IP\>  
in advanced tab set server B to `<node-red IP>` on port `10000` `TCP`  
thats it.

## but if node-red did not connect to inverter

if `Inverter stick out(TCP in node)` did not connect  
go to http://\<wifi stick local IP\>/config_hide.html  
and change server A (default server) to `<node-red IP>`

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