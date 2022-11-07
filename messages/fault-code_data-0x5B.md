# byte 0x5B(91 DEC) of data message
##### [back to readme](../README.md#data-messages)
##### [back to KTL-X data msg](decode_data_KTL-X.md)


| bit      	| HEX   	| description                                          	|
|----------	|-------	|------------------------------------------------------	|
| 00000001 	| +0x01 	| ID25 - BusUVP (Bus under voltage protection)         	|
| 00000010 	| +0x02 	| ID26 - BusOVP (Bus over voltage protection)          	|
| 00000100 	| +0x04 	| ID27 - VbusUnbalance (Bus voltage unbalance)         	|
| 00001000 	| +0x08 	| ID28 - DciOCP (The DCI is too high)                  	|
| 00010000 	| +0x10 	| ID29 - SwOCPInstant (The Grid current is too high)   	|
| 00100000 	| +0x20 	| ID30 - SwBOCPInstant (The input current is too high) 	|
| 01000000 	| +0x40 	| ID31 - reserved                                      	|
| 10000000 	| +0x80 	| ID32 - reserved                                      	|
