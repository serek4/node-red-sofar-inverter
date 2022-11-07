# hello_cd message
##### [back to readme](../README.md#messages-flow)  
V5 table  
41 bytes  
default value type is uInt16LE 

| HEX  	| DEC 	| TYPE 	   	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 97 msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - ?                                                                                    	|
| 0x04 	| 4   	| uInt16LE 	| always 48 msg type - ?                                                                                    	|
| 0x05 	| 5   	| uInt8    	| message nr - starts from 00(synced with server?)                                                          	|
| 0x06 	| 6   	| uInt8    	| message nr - starts from 01                                                                               	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                                            	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x0B 	| 11  	| uInt8    	| always 01                                                                                                 	|
| 0x0C 	| 12  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0D 	| 13  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0E 	| 14  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0F 	| 15  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x10 	| 16  	| uInt32LE 	| timer - every >=10740s - (uInt16LE?) reset after F429(3h interval),                                       	|
| 0x11 	| 17  	| uInt32LE 	| timer - every >=10740s - hello msg, data, hello_cd and hello_end msg sended after                         	|
| 0x12 	| 18  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x13 	| 19  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x14 	| 20  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x15 	| 21  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x16 	| 22  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x17 	| 23  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x18 	| 24  	| uInt16LE 	| always 01                                                                                                 	|
| 0x19 	| 25  	| uInt16LE 	| always 01                                                                                                 	|
| 0x1A 	| 26  	| uInt16LE 	| always 0C - (2x uInt16LE or uInt32LE?)                                                                    	|
| 0x1B 	| 27  	| uInt16LE 	| ?                                                                                                         	|
| 0x1C 	| 28  	| uInt16LE 	| ? increasing                                                                                              	|
| 0x1D 	| 29  	| uInt16LE 	| ? increasing cd 17? 16? 15?                                                                               	|
| 0x1E 	| 30  	| uInt8    	| always 00                                                                                                 	|
| 0x1F 	| 31  	| uInt32LE 	| 00 or ? - (2x uInt16LE or uInt32LE?)                                                                      	|
| 0x20 	| 32  	| uInt32LE 	| 00 or ?                                                                                                   	|
| 0x21 	| 33  	| uInt32LE 	| always 00                                                                                                 	|
| 0x22 	| 34  	| uInt32LE 	| always 00                                                                                                 	|
| 0x23 	| 35  	| uInt32LE 	| 00 or timestamp of ?                                                                                      	|
| 0x24 	| 36  	| uInt32LE 	| 00 or timestamp of ?                                                                                      	|
| 0x25 	| 37  	| uInt32LE 	| 00 or timestamp of ?                                                                                      	|
| 0x26 	| 38  	| uInt32LE 	| 00 or timestamp of ?                                                                                      	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x27 	| 39  	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0x28 	| 40  	| uInt8    	| always 15                                                                                                 	|
