# 60 bytes long message
##### [back to readme](../README.md#other-messages)  
V5 table  
60 bytes   
default value type is uInt16LE  

| HEX  	| DEC 	| TYPE 	   	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 2F msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - ?                                                                                    	|
| 0x04 	| 4   	| uInt16LE 	| always 43? msg type - ?                                                                                   	|
| 0x05 	| 5   	| uInt8    	| message nr - starts from 00(synced with server?)                                                          	|
| 0x06 	| 6   	| uInt8    	| message nr - starts from 01                                                                               	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                                            	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x0B 	| 11  	| uInt8    	| always 81?                                                                                                	|
| 0x0C 	| 12  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0D 	| 13  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0E 	| 14  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0F 	| 15  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x10 	| 16  	| uInt16LE 	| ?                                                                                                         	|
| 0x11 	| 17  	| uInt16LE 	| ?                                                                                                         	|
| 0x12 	| 18  	| uInt16LE 	| always 00                                                                                                 	|
| 0x13 	| 19  	| uInt16LE 	| always 00                                                                                                 	|
| 0x14 	| 20  	| uInt16LE 	| ?                                                                                                         	|
| 0x15 	| 21  	| uInt16LE 	| ?                                                                                                         	|
| 0x16 	| 22  	| uInt16LE 	| ?                                                                                                         	|
| 0x17 	| 23  	| uInt16LE 	| ?                                                                                                         	|
| 0x18 	| 24  	| uInt16LE 	| ?                                                                                                         	|
| 0x19 	| 25  	| uInt16LE 	| ?                                                                                                         	|
| 0x1A 	| 26  	| string   	| wifi ssid - string (30?) padded with 00 at end                                                            	|
| 0x1B 	| 27  	| string   	| wifi ssid - string                                                                                        	|
| 0x1C 	| 28  	| string   	| wifi ssid - string                                                                                        	|
| 0x1D 	| 29  	| string   	| wifi ssid - string                                                                                        	|
| 0x1E 	| 30  	| string   	| wifi ssid - string                                                                                        	|
| 0x1F 	| 31  	| string   	| wifi ssid - string                                                                                        	|
| 0x20 	| 32  	| string   	| wifi ssid - string                                                                                        	|
| 0x22 	| 33  	| string   	| wifi ssid - string                                                                                        	|
| 0x23 	| 34  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 35  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 36  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 37  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 38  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 39  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 40  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 41  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 42  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 43  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 44  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 45  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 46  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 47  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 48  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 49  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 50  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 51  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 52  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 53  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 54  	| string   	| wifi ssid - string                                                                                        	|
| 0x24 	| 55  	| string   	| wifi ssid - string                                                                                        	|
| 0x38 	| 56  	| uInt16LE 	| ?                                                                                                         	|
| 0x39 	| 57  	| uInt16LE 	| always 01 ?                                                                                               	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x3A 	| 58  	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0x3B 	| 59  	| uInt8    	| always 15                                                                                                 	|
