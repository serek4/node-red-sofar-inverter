# KTL-X data message
##### [back to readme](../README.md#data-messages)  
V5 table  
164 bytes   
message type 0x2701  
default value type is uInt16LE  

| HEX  	| DEC 	| TYPE     	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always 97 msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
| 0x02 	| 2   	| uInt16LE 	| always 00 msg length                                                                                      	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - data                                                                                 	|
| 0x04 	| 4   	| uInt16LE 	| always 42 msg type - data                                                                                 	|
| 0x05 	| 5   	| uInt8    	| message nr - starts from 00(synced with server?)                                                          	|
| 0x06 	| 6   	| uInt8    	| message nr - starts from 01                                                                               	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                                            	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                                            	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0x0B 	| 11  	| uInt8    	| always 01 (81?)                                                                                           	|
| 0x0C 	| 12  	| uInt16LE 	| always 01 Sensor Type List?                                                                               	|
| 0x0D 	| 13  	| uInt16LE 	| always 27 Sensor Type List?                                                                               	|
| 0x0E 	| 14  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x0F 	| 15  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x10 	| 16  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x11 	| 17  	| uInt32LE 	| total operation time (sec)                                                                                	|
| 0x12 	| 18  	| uInt32LE 	| timer - every >=10740s - (uInt16LE?) reset after F429(3h interval?),                                      	|
| 0x13 	| 19  	| uInt32LE 	| timer - every >=10740s - hello msg, data, hello_cd and hello_end msg sended after                         	|
| 0x14 	| 20  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x15 	| 21  	| uInt32LE 	| timer - every >=10740s                                                                                    	|
| 0x16 	| 22  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x17 	| 23  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x18 	| 24  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x19 	| 25  	| uInt32LE 	| timestamp of ?                                                                                            	|
| 0x1A 	| 26  	| uInt16LE 	| always 01                                                                                                 	|
| 0x1B 	| 27  	| uInt16LE 	| always 00                                                                                                 	|
| 0x1C 	| 28  	| uInt16LE 	| increasing by 1 every msg - (uInt32LE?)                                                                   	|
| 0x1D 	| 29  	| uInt16LE 	| increasing by 1 every msg                                                                                 	|
| 0x1E 	| 30  	| uInt16LE 	| always 00                                                                                                 	|
| 0x1F 	| 31  	| uInt16LE 	| always 00                                                                                                 	|
| 0x20 	| 32  	| string   	| inverter SN - string(16)                                                                                  	|
| 0x21 	| 33  	| string   	| inverter SN - string                                                                                      	|
| 0x22 	| 34  	| string   	| inverter SN - string                                                                                      	|
| 0x23 	| 35  	| string   	| inverter SN - string                                                                                      	|
| 0x24 	| 36  	| string   	| inverter SN - string                                                                                      	|
| 0x25 	| 37  	| string   	| inverter SN - string                                                                                      	|
| 0x26 	| 38  	| string   	| inverter SN - string                                                                                      	|
| 0x27 	| 39  	| string   	| inverter SN - string                                                                                      	|
| 0x28 	| 40  	| string   	| inverter SN - string                                                                                      	|
| 0x29 	| 41  	| string   	| inverter SN - string                                                                                      	|
| 0x2A 	| 42  	| string   	| inverter SN - string                                                                                      	|
| 0x2B 	| 43  	| string   	| inverter SN - string                                                                                      	|
| 0x2C 	| 44  	| string   	| inverter SN - string                                                                                      	|
| 0x2D 	| 45  	| string   	| inverter SN - string                                                                                      	|
| 0x2E 	| 46  	| string   	| inverter SN - string [space]                                                                              	|
| 0x2F 	| 47  	| string   	| inverter SN - string [space]                                                                              	|
| 0x30 	| 48  	| int16LE  	| inverter temperature (°C)/10                                                                              	|
| 0x31 	| 49  	| int16LE  	| inverter temperature (°C)/10                                                                              	|
| 0x32 	| 50  	| uInt16LE 	| VDC1/10 (V)                                                                                               	|
| 0x33 	| 51  	| uInt16LE 	| VDC1/10 (V)                                                                                               	|
| 0x34 	| 52  	| uInt16LE 	| VDC2/10 (V)                                                                                               	|
| 0x35 	| 53  	| uInt16LE 	| VDC2/10 (V)                                                                                               	|
| 0x36 	| 54  	| uInt16LE 	| IDC1/10 (I)                                                                                               	|
| 0x36 	| 55  	| uInt16LE 	| IDC1/10 (I)                                                                                               	|
| 0x38 	| 56  	| uInt16LE 	| IDC2/10 (I)                                                                                               	|
| 0x37 	| 57  	| uInt16LE 	| IDC2/10 (I)                                                                                               	|
| 0x3A 	| 58  	| uInt16LE 	| IAC1/10 (I)                                                                                               	|
| 0x3B 	| 59  	| uInt16LE 	| IAC1/10 (I)                                                                                               	|
| 0x3C 	| 60  	| uInt16LE 	| IAC2/10 (I)                                                                                               	|
| 0x3D 	| 61  	| uInt16LE 	| IAC2/10 (I)                                                                                               	|
| 0x3E 	| 62  	| uInt16LE 	| IAC3/10 (I)                                                                                               	|
| 0x3F 	| 63  	| uInt16LE 	| IAC3/10 (I)                                                                                               	|
| 0x40 	| 64  	| uInt16LE 	| VAC1/10 (V)                                                                                               	|
| 0x41 	| 65  	| uInt16LE 	| VAC1/10 (V)                                                                                               	|
| 0x42 	| 66  	| uInt16LE 	| VAC2/10 (V)                                                                                               	|
| 0x43 	| 67  	| uInt16LE 	| VAC2/10 (V)                                                                                               	|
| 0x44 	| 68  	| uInt16LE 	| VAC3/10 (V)                                                                                               	|
| 0x45 	| 79  	| uInt16LE 	| VAC3/10 (V)                                                                                               	|
| 0x46 	| 70  	| uInt16LE 	| FAC/100 (Hz)                                                                                              	|
| 0x47 	| 71  	| uInt16LE 	| FAC/100 (Hz)                                                                                              	|
| 0x48 	| 72  	| uInt32LE 	| current power(W)                                                                                          	|
| 0x49 	| 73  	| uInt32LE 	| current power(W)                                                                                          	|
| 0x4A 	| 74  	| uInt32LE 	| current power(W)                                                                                          	|
| 0x4B 	| 75  	| uInt32LE 	| current power(W)                                                                                          	|
| 0x4C 	| 76  	| uInt32LE 	| daily energy/100(kWh)                                                                                     	|
| 0x4D 	| 77  	| uInt32LE 	| daily energy/100(kWh)                                                                                     	|
| 0x4E 	| 78  	| uInt32LE 	| daily energy/100(kWh)                                                                                     	|
| 0x4F 	| 79  	| uInt32LE 	| daily energy/100(kWh)                                                                                     	|
| 0x50 	| 80  	| uInt32LE 	| total energy/10(kWh)                                                                                      	|
| 0x51 	| 81  	| uInt32LE 	| total energy/10(kWh)                                                                                      	|
| 0x52 	| 82  	| uInt32LE 	| total energy/10(kWh)                                                                                      	|
| 0x53 	| 83  	| uInt32LE 	| total energy/10(kWh)                                                                                      	|
| 0x54 	| 84  	| uInt32LE 	| total time (h)                                                                                            	|
| 0x55 	| 85  	| uInt32LE 	| total time (h)                                                                                            	|
| 0x56 	| 86  	| uInt32LE 	| total time (h)                                                                                            	|
| 0x57 	| 87  	| uInt32LE 	| total time (h)                                                                                            	|
| 0x58 	| 88  	| uInt16LE 	| inverter status: 00 - standby, 02 - normal, 03 - fault, 04 - permanent                                    	|
| 0x59 	| 89  	| uInt16LE 	| inverter status: Low byte only                                                                            	|
| 0x5A 	| 90  	| uInt8    	| [fault code](fault-code_data-0x5A.md)                                                                     	|
| 0x5B 	| 91  	| uInt8    	| [fault code](fault-code_data-0x5B.md)                                                                     	|
| 0x5C 	| 92  	| uInt8    	| [fault code](fault-code_data-0x5C.md)                                                                     	|
| 0x5D 	| 93  	| uInt8    	| [fault code](fault-code_data-0x5D.md)                                                                     	|
| 0x5E 	| 94  	| uInt16LE 	| fault code?                                                                                               	|
| 0x5F 	| 95  	| uInt16LE 	| fault code?                                                                                               	|
| 0x60 	| 96  	| uInt16LE 	| fault code?                                                                                               	|
| 0x61 	| 97  	| uInt16LE 	| fault code?                                                                                               	|
| 0x62 	| 98  	| uInt16LE 	| fault code?                                                                                               	|
| 0x63 	| 99  	| uInt16LE 	| fault code?                                                                                               	|
| 0x64 	| 100 	| uInt16LE 	| alert msg code?                                                                                           	|
| 0x65 	| 101 	| uInt16LE 	| alert msg code?                                                                                           	|
| 0x66 	| 102 	| uInt16LE 	| inner board msg code?                                                                                     	|
| 0x67 	| 103 	| uInt16LE 	| inner board msg code?                                                                                     	|
| 0x68 	| 104 	| string   	| inverter firmware? - string (4)                                                                           	|
| 0x69 	| 105 	| string   	| inverter firmware? - string                                                                               	|
| 0x6A 	| 106 	| string   	| inverter firmware? - string                                                                               	|
| 0x6B 	| 107 	| string   	| inverter firmware? - string                                                                               	|
| 0x6C 	| 108 	| string   	| hardware version - string (4)                                                                             	|
| 0x6D 	| 109 	| string   	| hardware version - string                                                                                 	|
| 0x6E 	| 110 	| string   	| hardware version - string                                                                                 	|
| 0x6F 	| 111 	| string   	| hardware version - string                                                                                 	|
| 0x70 	| 112 	| int16LE  	| logger temperature (°C)                                                                                   	|
| 0x71 	| 113 	| int16LE  	| logger temperature (°C)                                                                                   	|
| 0x72 	| 114 	| uInt16LE 	| Bus voltage/10 (V)                                                                                        	|
| 0x73 	| 115 	| uInt16LE 	| Bus voltage/10 (V)                                                                                        	|
| 0x74 	| 116 	| uInt16LE 	| Vice CPU input voltage/10 (V)                                                                             	|
| 0x75 	| 117 	| uInt16LE 	| Vice CPU input voltage/10                                                                                 	|
| 0x76 	| 118 	| uInt16LE 	| ? value around 800                                                                                        	|
| 0x77 	| 119 	| uInt16LE 	| ? value around 800                                                                                        	|
| 0x78 	| 120 	| uInt16LE 	| countdown time(60h - 0x3C00)                                                                              	|
| 0x79 	| 121 	| uInt16LE 	| countdown time                                                                                            	|
| 0x7A 	| 122 	| uInt16LE 	| always 01                                                                                                 	|
| 0x7B 	| 123 	| uInt16LE 	| always 00                                                                                                 	|
| 0x7C 	| 124 	| uInt16LE 	| PV1 insulation resistance                                                                                 	|
| 0x7D 	| 125 	| uInt16LE 	| PV1 insulation resistance                                                                                 	|
| 0x7E 	| 126 	| uInt16LE 	| PV2 insulation resistance                                                                                 	|
| 0x7F 	| 127 	| uInt16LE 	| PV2 insulation resistance                                                                                 	|
| 0x80 	| 128 	| uInt16LE 	| insulation impedance - cathode to ground                                                                  	|
| 0x81 	| 129 	| uInt16LE 	| insulation impedance - cathode to ground                                                                  	|
| 0x82 	| 130 	| uInt16LE 	| country code - (uInt8?)                                                                                   	|
| 0x83 	| 131 	| uInt16LE 	| country code                                                                                              	|
| 0x84 	| 132 	| uInt16LE 	| always 00                                                                                                 	|
| 0x85 	| 133 	| uInt16LE 	| always 00                                                                                                 	|
| 0x86 	| 134 	| uInt16LE 	| always 00                                                                                                 	|
| 0x87 	| 134 	| uInt16LE 	| always 00                                                                                                 	|
| 0x88 	| 134 	| uInt16LE 	| leaking current                                                                                           	|
| 0x89 	| 134 	| uInt16LE 	| leaking current                                                                                           	|
| 0x8A 	| 138 	| uInt16LE 	| A-phase DC distribution                                                                                   	|
| 0x8B 	| 139 	| uInt16LE 	| A-phase DC distribution                                                                                   	|
| 0x8C 	| 140 	| uInt16LE 	| B-phase DC distribution                                                                                   	|
| 0x8D 	| 141 	| uInt16LE 	| B-phase DC distribution                                                                                   	|
| 0x8E 	| 142 	| uInt16LE 	| C-phase DC distribution                                                                                   	|
| 0x8F 	| 143 	| uInt16LE 	| C-phase DC distribution                                                                                   	|
| 0x90 	| 144 	| string   	| main inverter firmware - string (4)                                                                       	|
| 0x91 	| 145 	| string   	| main inverter firmware - string                                                                           	|
| 0x92 	| 146 	| string   	| main inverter firmware - string                                                                           	|
| 0x93 	| 147 	| string   	| main inverter firmware - string                                                                           	|
| 0x94 	| 148 	| string   	| slave inverter firmware - string (4)                                                                      	|
| 0x95 	| 149 	| string   	| slave inverter firmware - string                                                                          	|
| 0x96 	| 150 	| string   	| slave inverter firmware - string                                                                          	|
| 0x97 	| 151 	| string   	| slave inverter firmware - string                                                                          	|
| 0x98 	| 152 	| uInt8    	| year                                                                                                      	|
| 0x99 	| 153 	| uInt8    	| month                                                                                                     	|
| 0x9A 	| 154 	| uInt8    	| day                                                                                                       	|
| 0x9B 	| 155 	| uInt8    	| hour                                                                                                      	|
| 0x9C 	| 156 	| uInt8    	| minute                                                                                                    	|
| 0x9D 	| 157 	| uInt8    	| second                                                                                                    	|
| 0x9E 	| 158 	| uInt16LE 	| ? changes with the current power - (uInt32LE?)                                                            	|
| 0x9F 	| 159 	| uInt16LE 	| ? changes with the current power                                                                          	|
| 0xA0 	| 160 	| uInt16LE 	| always 00                                                                                                 	|
| 0xA1 	| 161 	| uInt16LE 	| always 00                                                                                                 	|
| ---- 	| --- 	| -------- 	|                                                                                                           	|
| 0xA2 	| 162 	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0xA3 	| 163 	| uInt8    	| always 15                                                                                                 	|
