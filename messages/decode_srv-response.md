# server response message
##### [back to readme](../README.md#messages-flow)  
V5 table  
23 bytes   
default value type is uInt16LE  

| HEX  	| DEC 	| TYPE     	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 0A msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - response                                                                             	|
| 0x04 	| 4   	| uInt16LE 	| msg type - response (request Dependent: 41->11, 42->12, 43->13, 47->17, 48->18)                           	|
| 0x05 	| 5   	| uInt8    	| message nr - req + 1?                                                                                     	|
| 0x06 	| 6   	| uInt8    	| message nr - matches req                                                                                  	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                                            	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x0B 	| 11  	| uInt8    	| always matches request                                                                                    	|
| 0x0C 	| 12  	| uInt8    	| always 01                                                                                                 	|
| 0x0D 	| 13  	| uInt32LE 	| timestamp(in sec)                                                                                         	|
| 0x0E 	| 14  	| uInt32LE 	| timestamp(in sec)                                                                                         	|
| 0x0F 	| 15  	| uInt32LE 	| timestamp(in sec)                                                                                         	|
| 0x10 	| 16  	| uInt32LE 	| timestamp(in sec)                                                                                         	|
| 0x11 	| 17  	| uInt16LE 	| always 78                                                                                                 	|
| 0x12 	| 18  	| uInt16LE 	| always 00                                                                                                 	|
| 0x13 	| 19  	| uInt16LE 	| always 00                                                                                                 	|
| 0x14 	| 20  	| uInt16LE 	| always 00                                                                                                 	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x15 	| 21  	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0x16 	| 22  	| uInt8    	| always 15                                                                                                 	|