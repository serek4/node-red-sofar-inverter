# Sofar wifi stick communication with ginlong.com (solarman.cn) server

## http://(wifi stick local IP)/config_hide.html

### wifi stick:

    SN: 174xxxxxxx
    firmware: LSW3_14_FFFF_1.0.34

## wifi stick (hello msg) -> ginlong server (srv-response) -> wifi stick Internal srv
## 5min interval: wifi stick (data) -> ginlong server (srv-response) -> wifi stick Internal srv
### 120s interval: wifi stick Internal srv (heartbeat) ->ginlong server (srv-response) -> wifi stick Internal srv
#### ?: wifi stick (40) ->ginlong server (srv-response) -> wifi stick Internal srv
#### ?: wifi stick (72) ->ginlong server (srv-response) -> wifi stick Internal srv