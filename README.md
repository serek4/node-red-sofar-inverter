# Sofar wifi stick communication with ginlong.com (solarmanpv.com) server

## wifi stick:

    SN: 174xxxxxxx
    firmware: LSW3_14_FFFF_1.0.34

## http://(wifi stick local IP)/config_hide.html

hiden menu for wifi stick with default server settings

## after power on:

wifi stick (hello msg) -> ginlong server (srv-response) -> wifi stick  
wifi stick (data) -> ginlong server (srv-response) -> wifi stick  
wifi stick (41) ->ginlong server (srv-response) -> wifi stick  
wifi stick (73) ->ginlong server (srv-response) -> wifi stick  

## 120s interval:

wifi stick (heartbeat) ->ginlong server (srv-response) -> wifi stick

## 5min interval:

wifi stick (data) -> ginlong server (srv-response) -> wifi stick

## ~3h interval:

wifi stick (hello msg) -> ginlong server (srv-response) -> wifi stick  
wifi stick (data) -> ginlong server (srv-response) -> wifi stick  
wifi stick (41) ->ginlong server (srv-response) -> wifi stick  
wifi stick (73) ->ginlong server (srv-response) -> wifi stick