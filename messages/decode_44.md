# 44 bytes long message
##### [back to readme](../README.md#other-messages)  
V5 table  
44bytes  
default value type is uInt16LE 

| HEX  	| DEC 	| TYPE 	   	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 1C msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - ?                                                                                    	|
| 0x04 	| 4   	| uInt16LE 	| always 48? msg type - ?                                                                                   	|
| 0x05 	| 5   	| uInt8    	| message nr - starts from 00(synced with server?)                                                          	|
| 0x06 	| 6   	| uInt8    	| message nr - starts from 01                                                                               	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                                            	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x0B 	| 11  	| uInt16LE 	|                                                                                                           	|
| 0x0C 	| 12  	| uInt16LE 	|                                                                                                           	|
| 0x0D 	| 13  	| uInt16LE 	|                                                                                                           	|
| 0x0E 	| 14  	| uInt16LE 	|                                                                                                           	|
| 0x0F 	| 15  	| uInt16LE 	|                                                                                                           	|
| 0x10 	| 16  	| uInt16LE 	|                                                                                                           	|
| 0x11 	| 17  	| uInt16LE 	|                                                                                                           	|
| 0x12 	| 18  	| uInt16LE 	|                                                                                                           	|
| 0x13 	| 19  	| uInt16LE 	|                                                                                                           	|
| 0x14 	| 20  	| Int32LE 	| current time (timestamp)?                                                                                 	|
| 0x15 	| 21  	| Int32LE 	| current time (timestamp)?                                                                                 	|
| 0x16 	| 22  	| Int32LE 	| current time (timestamp)?                                                                                 	|
| 0x17 	| 23  	| Int32LE 	| current time (timestamp)?                                                                                 	|
| 0x18 	| 24  	| uInt16LE 	|                                                                                                           	|
| 0x19 	| 25  	| uInt16LE 	|                                                                                                           	|
| 0x1A 	| 26  	| string   	| inverter SN - string(16)                                                                                  	|
| 0x1B 	| 27  	| string   	| inverter SN - string                                                                                      	|
| 0x1C 	| 28  	| string   	| inverter SN - string                                                                                      	|
| 0x1D 	| 29  	| string   	| inverter SN - string                                                                                      	|
| 0x1E 	| 30  	| string   	| inverter SN - string                                                                                      	|
| 0x1F 	| 31  	| string   	| inverter SN - string                                                                                      	|
| 0x20 	| 32  	| string   	| inverter SN - string                                                                                      	|
| 0x21 	| 33  	| string   	| inverter SN - string                                                                                      	|
| 0x22 	| 34  	| string   	| inverter SN - string                                                                                      	|
| 0x23 	| 35  	| string   	| inverter SN - string                                                                                      	|
| 0x24 	| 36  	| string   	| inverter SN - string                                                                                      	|
| 0x25 	| 37  	| string   	| inverter SN - string                                                                                      	|
| 0x26 	| 38  	| string   	| inverter SN - string                                                                                      	|
| 0x27 	| 39  	| string   	| inverter SN - string                                                                                      	|
| 0x28 	| 40  	| string   	| inverter SN - string [space]                                                                              	|
| 0x29 	| 41  	| string   	| inverter SN - string [space]                                                                              	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x2A 	| 42  	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0x2B 	| 43  	| uInt8    	| always 15                                                                                                 	|
