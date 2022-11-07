# byte 0x5C(92 DEC) of data message
##### [back to readme](../README.md#data-messages)
##### [back to KTL-X data msg](decode_data_KTL-X.md)

e.g. `0x0A = 0x08 + 0x02 -> GridUFP and GridUVP`

| bit      	| HEX   	| description                                      	|
|----------	|-------	|--------------------------------------------------	|
| 00000001 	| +0x01 	| ID01 - GridOVP (grid over voltage protection)    	|
| 00000010 	| +0x02 	| ID02 - GridUVP (grid under voltage protection)   	|
| 00000100 	| +0x04 	| ID03 - GridOFP (grid over frequency protection)  	|
| 00001000 	| +0x08 	| ID04 - GridUFP (grid under frequency protection) 	|
| 00010000 	| +0x10 	| ID05 - PVUVP (PV Under Voltage Protection)       	|
| 00100000 	| +0x20 	| ID06 - GridLVRT (Grid Low Voltage Ride through)  	|
| 01000000 	| +0x40 	| ID07 - reserved                                  	|
| 10000000 	| +0x80 	| ID08 - reserved                                  	|
