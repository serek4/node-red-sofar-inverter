# hello message
##### [back to readme](../README.md#messages-flow)  
V5 table  
99 bytes   
default value type is uInt16LE  

| HEX  	| DEC 	| TYPE     	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 56 msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - hello msg                                                                            	|
| 0x04 	| 4   	| uInt16LE 	| always 41 msg type - hello msg                                                                            	|
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
| 0x10 	| 16  	| uInt32LE 	| timer - every >=10740s - (uInt16LE?) reset after F429(3h interval?),                                      	|
| 0x11 	| 17  	| uInt32LE 	| timer - every >=10740s - hello msg, data, hello_cd and hello_end msg sended after                         	|
| 0x12 	| 18  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x13 	| 19  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x14 	| 20  	| uInt16LE 	| always 00                                                                                                 	|
| 0x15 	| 21  	| uInt16LE 	| always 00                                                                                                 	|
| 0x16 	| 22  	| uInt16LE 	| always 00                                                                                                 	|
| 0x17 	| 23  	| uInt16LE 	| always 00                                                                                                 	|
| 0x18 	| 24  	| uInt8    	| uploading frequency (min)                                                                                 	|
| 0x19 	| 25  	| uInt8    	| data logging frequency (sec)                                                                              	|
| 0x1A 	| 26  	| uInt8    	| heartbeat frequency (sec)                                                                                 	|
| 0x1B 	| 27  	| uInt8    	| max nr of connected devices or command type                                                               	|
| 0x1C 	| 28  	| uInt8    	| signal quality?                                                                                           	|
| 0x1D 	| 29  	| uInt8    	| sensor type nr?                                                                                           	|
| 0x1E 	| 30  	| string   	| module version - string(39?) padded with 00 at the end                                                    	|
| 0x1F 	| 31  	| string   	| module version - string                                                                                   	|
| 0x20 	| 32  	| string   	| module version - string                                                                                   	|
| 0x21 	| 33  	| string   	| module version - string                                                                                   	|
| 0x22 	| 34  	| string   	| module version - string                                                                                   	|
| 0x23 	| 35  	| string   	| module version - string                                                                                   	|
| 0x24 	| 36  	| string   	| module version - string                                                                                   	|
| 0x25 	| 37  	| string   	| module version - string                                                                                   	|
| 0x26 	| 38  	| string   	| module version - string                                                                                   	|
| 0x27 	| 39  	| string   	| module version - string                                                                                   	|
| 0x28 	| 40  	| string   	| module version - string                                                                                   	|
| 0x29 	| 41  	| string   	| module version - string                                                                                   	|
| 0x2A 	| 42  	| string   	| module version - string                                                                                   	|
| 0x2B 	| 43  	| string   	| module version - string                                                                                   	|
| 0x2C 	| 44  	| string   	| module version - string                                                                                   	|
| 0x2D 	| 45  	| string   	| module version - string                                                                                   	|
| 0x2E 	| 46  	| string   	| module version - string                                                                                   	|
| 0x2F 	| 47  	| string   	| module version - string                                                                                   	|
| 0x30 	| 48  	| string   	| module version - string                                                                                   	|
| 0x31 	| 49  	| string   	| module version - string                                                                                   	|
| 0x32 	| 50  	| string   	| module version - string                                                                                   	|
| 0x33 	| 51  	| string   	| module version - string                                                                                   	|
| 0x34 	| 52  	| string   	| module version - string                                                                                   	|
| 0x35 	| 53  	| string   	| module version - string                                                                                   	|
| 0x36 	| 54  	| string   	| module version - string                                                                                   	|
| 0x37 	| 55  	| string   	| module version - string                                                                                   	|
| 0x38 	| 56  	| string   	| module version - string                                                                                   	|
| 0x39 	| 57  	| string   	| module version - string                                                                                   	|
| 0x3A 	| 58  	| string   	| module version - string                                                                                   	|
| 0x3B 	| 59  	| string   	| module version - string                                                                                   	|
| 0x3C 	| 60  	| string   	| module version - string                                                                                   	|
| 0x3D 	| 61  	| string   	| module version - string                                                                                   	|
| 0x3E 	| 62  	| string   	| module version - string                                                                                   	|
| 0x3F 	| 63  	| string   	| module version - string                                                                                   	|
| 0x40 	| 64  	| string   	| module version - string                                                                                   	|
| 0x41 	| 65  	| string   	| module version - string                                                                                   	|
| 0x42 	| 66  	| string   	| module version - string                                                                                   	|
| 0x43 	| 67  	| string   	| module version - string                                                                                   	|
| 0x44 	| 68  	| string   	| module version - string                                                                                   	|
| 0x45 	| 69  	| string   	| module version - string                                                                                   	|
| 0x46 	| 70  	| hex      	| STA mac address (6)                                                                                       	|
| 0x47 	| 71  	| hex      	| STA mac address                                                                                           	|
| 0x48 	| 72  	| hex      	| STA mac address                                                                                           	|
| 0x49 	| 73  	| hex      	| STA mac address                                                                                           	|
| 0x4A 	| 74  	| hex      	| STA mac address                                                                                           	|
| 0x4B 	| 75  	| hex      	| STA mac address                                                                                           	|
| 0x4C 	| 76  	| string   	| local IP - string(15?) padded with 00 at end                                                              	|
| 0x4D 	| 77  	| string   	| local IP - string                                                                                         	|
| 0x4E 	| 78  	| string   	| local IP - string                                                                                         	|
| 0x4F 	| 79  	| string   	| local IP - string                                                                                         	|
| 0x50 	| 80  	| string   	| local IP - string                                                                                         	|
| 0x51 	| 81  	| string   	| local IP - string                                                                                         	|
| 0x52 	| 82  	| string   	| local IP - string                                                                                         	|
| 0x53 	| 83  	| string   	| local IP - string                                                                                         	|
| 0x54 	| 84  	| string   	| local IP - string                                                                                         	|
| 0x55 	| 85  	| string   	| local IP - string                                                                                         	|
| 0x56 	| 86  	| string   	| local IP - string                                                                                         	|
| 0x57 	| 87  	| string   	| local IP - string                                                                                         	|
| 0x58 	| 88  	| string   	| local IP - string                                                                                         	|
| 0x59 	| 89  	| string   	| local IP - string                                                                                         	|
| 0x5A 	| 90  	| string   	| local IP - string                                                                                         	|
| 0x5B 	| 91  	| uInt16LE 	| always 00                                                                                                 	|
| 0x5C 	| 92  	| uInt16LE 	| always 00                                                                                                 	|
| 0x5D 	| 93  	| uInt16LE 	| always 00                                                                                                 	|
| 0x5E 	| 94  	| uInt16LE 	| always 01                                                                                                 	|
| 0x5F 	| 95  	| uInt16LE 	| always 01 Sensor Type List?                                                                               	|
| 0x60 	| 96  	| uInt16LE 	| always 27 Sensor Type List?                                                                               	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x61 	| 97  	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0x62 	| 98  	| uInt8    	| always 15                                                                                                 	|
