# byte 0x58(88 DEC) of data message
##### [back to readme](../README.md) 
##### [back to data msg](decode_data.md) 

e.g. `0x0A = 0x08 + 0x02 -> GridUFP and GridUVP`

| bit      	| HEX   	| description                                	|
|----------	|-------	|--------------------------------------------	|
| 00000001 	| +0x01 	| ? GridOVP (grid over voltage protection)   	|
| 00000010 	| +0x02 	| GridUVP (grid under voltage protection)    	|
| 00000100 	| +0x04 	| ? GridOFP (grid over frequency protection) 	|
| 00001000 	| +0x08 	| GridUFP (grid under frequency protection)  	|
| 00010000 	| +0x10 	|                                            	|
| 00100000 	| +0x20 	|                                            	|
| 01000000 	| +0x40 	|                                            	|
| 10000000 	| +0x80 	|                                            	|
