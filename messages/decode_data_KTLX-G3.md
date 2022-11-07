# KTLX-G3 data message
##### [back to readme](../README.md#data-messages)  
V5 table  
1445 bytes   
message type 270A  
  

| HEX  	| DEC 	| TYPE     	| VALUE                                                                             	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                         	|
| 0x01 	| 1   	| uInt16LE 	| always 98 msg length - excl msg header(0x00 - 0x0A), checksum and last byte       	|
| 0x02 	| 2   	| uInt16LE 	| always 05 msg length                                                              	|
| 0x03 	| 3   	| uInt16LE 	| always 10 msg type - data                                                         	|
| 0x04 	| 4   	| uInt16LE 	| always 42 msg type - data                                                         	|
| 0x05 	| 5   	| uInt8    	| message nr - starts from 00(synced with server?)                                  	|
| 0x06 	| 6   	| uInt8    	| message nr - starts from 01                                                       	|
| 0x07 	| 7   	| uInt32LE 	| data logger SN                                                                    	|
| 0x08 	| 8   	| uInt32LE 	| data logger SN                                                                    	|
| 0x09 	| 9   	| uInt32LE 	| data logger SN                                                                    	|
| 0x0A 	| 10  	| uInt32LE 	| data logger SN                                                                    	|
| ---- 	| --- 	| -------- 	|                                                                                   	|
| 0x0B 	| 11  	| uInt8    	| always 01                                                                         	|
| 0x0C 	| 12  	| uInt16LE 	| always 0A Sensor Type List                                                        	|
| 0x0D 	| 13  	| uInt16LE 	| always 27 Sensor Type List                                                        	|
| 0x0E 	| 14  	| uInt32LE 	| total operation time (sec)                                                        	|
| 0x0F 	| 15  	| uInt32LE 	| total operation time (sec)                                                        	|
| 0x10 	| 16  	| uInt32LE 	| total operation time (sec)                                                        	|
| 0x11 	| 17  	| uInt32LE 	| total operation time (sec)                                                        	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x50 	| 80  	| int16BE  	| inverter plate temperature (°C)                                                   	|
| 0x51 	| 81  	| int16BE  	| inverter plate temperature (°C)                                                   	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x54 	| 84  	| int16BE  	| inverter radiator temperature (°C)                                                	|
| 0x55 	| 85  	| int16BE  	| inverter radiator temperature (°C)                                                	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x78 	| 120 	| uInt16BE 	| year                                                                              	|
| 0x79 	| 121 	| uInt16BE 	| year                                                                              	|
| 0x7A 	| 122 	| uInt16BE 	| month                                                                             	|
| 0x7B 	| 123 	| uInt16BE 	| month                                                                             	|
| 0x7C 	| 124 	| uInt16BE 	| day                                                                               	|
| 0x7D 	| 125 	| uInt16BE 	| day                                                                               	|
| 0x7E 	| 126 	| uInt16BE 	| hour                                                                              	|
| 0x7F 	| 127 	| uInt16BE 	| hour                                                                              	|
| 0x80 	| 128 	| uInt16BE 	| minute                                                                            	|
| 0x81 	| 129 	| uInt16BE 	| minute                                                                            	|
| 0x82 	| 130 	| uInt16BE 	| second                                                                            	|
| 0x83 	| 131 	| uInt16BE 	| second                                                                            	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x8E 	| 142 	| string   	| inverter SN - string(14)                                                          	|
| 0x8F 	| 143 	| string   	| inverter SN - string                                                              	|
| 0x90 	| 144 	| string   	| inverter SN - string                                                              	|
| 0x91 	| 145 	| string   	| inverter SN - string                                                              	|
| 0x92 	| 146 	| string   	| inverter SN - string                                                              	|
| 0x93 	| 147 	| string   	| inverter SN - string                                                              	|
| 0x94 	| 148 	| string   	| inverter SN - string                                                              	|
| 0x95 	| 149 	| string   	| inverter SN - string                                                              	|
| 0x96 	| 150 	| string   	| inverter SN - string                                                              	|
| 0x97 	| 151 	| string   	| inverter SN - string                                                              	|
| 0x98 	| 152 	| string   	| inverter SN - string                                                              	|
| 0x99 	| 153 	| string   	| inverter SN - string                                                              	|
| 0x9A 	| 154 	| string   	| inverter SN - string                                                              	|
| 0x9B 	| 155 	| string   	| inverter SN - string                                                              	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0xC6 	| 198 	| uInt16BE 	| frequency AC / 100 (Hz)                                                           	|
| 0xC7 	| 199 	| uInt16BE 	| frequency AC / 100 (Hz)                                                           	|
| 0xC8 	| 200 	| uInt16BE 	| currentPower / 100 (W)                                                            	|
| 0xC9 	| 201 	| uInt16BE 	| currentPower / 100 (W)                                                            	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0xD8 	| 216 	| uInt16BE 	| VAC1 / 10 (V)                                                                     	|
| 0xD9 	| 217 	| uInt16BE 	| VAC1 / 10 (V)                                                                     	|
| 0xDA 	| 218 	| uInt16BE 	| IAC1 / 100 (I)                                                                    	|
| 0xDB 	| 219 	| uInt16BE 	| IAC1 / 100 (I)                                                                    	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0xEE 	| 238 	| uInt16BE 	| VAC2 / 10 (V)                                                                     	|
| 0xEF 	| 239 	| uInt16BE 	| VAC2 / 10 (V)                                                                     	|
| 0xF0 	| 240 	| uInt16BE 	| IAC2 / 100 (I)                                                                    	|
| 0xF1 	| 241 	| uInt16BE 	| IAC2 / 100 (I)                                                                    	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x104	| 260 	| uInt16BE 	| VAC3 / 10 (V)                                                                     	|
| 0x105	| 261 	| uInt16BE 	| VAC3 / 10 (V)                                                                     	|
| 0x106	| 262 	| uInt16BE 	| IAC3 / 100 (I)                                                                    	|
| 0x107	| 263 	| uInt16BE 	| IAC3 / 100 (I)                                                                    	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x166	| 358 	| uInt16BE 	| VDC1 / 10 (V)                                                                     	|
| 0x167	| 359 	| uInt16BE 	| VDC1 / 10 (V)                                                                     	|
| 0x168	| 360 	| uInt16BE 	| IDC1 / 100 (I)                                                                    	|
| 0x169	| 361 	| uInt16BE 	| IDC1 / 100 (I)                                                                    	|
| 0x16A	| 362 	| uInt16BE 	| PDC1 / 100 (W)                                                                    	|
| 0x16B	| 363 	| uInt16BE 	| PDC1 / 100 (W)                                                                    	|
| 0x16C	| 358 	| uInt16BE 	| VDC2 / 10 (V)                                                                     	|
| 0x16D	| 359 	| uInt16BE 	| VDC2 / 10 (V)                                                                     	|
| 0x16E	| 360 	| uInt16BE 	| IDC2 / 100 (I)                                                                    	|
| 0x16F	| 361 	| uInt16BE 	| IDC2 / 100 (I)                                                                    	|
| 0x170	| 362 	| uInt16BE 	| PDC2 / 100 (W)                                                                    	|
| 0x171	| 363 	| uInt16BE 	| PDC2 / 100 (W)                                                                    	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x286	| 646 	| uInt32BE 	| daily energy / 100 (kWh)                                                          	|
| 0x287	| 647 	| uInt32BE 	| daily energy / 100 (kWh)                                                          	|
| 0x288	| 648 	| uInt32BE 	| daily energy / 100 (kWh)                                                          	|
| 0x289	| 649 	| uInt32BE 	| daily energy / 100 (kWh)                                                          	|
| 0x28A	| 650 	| uInt32BE 	| total energy / 10 (kWh)                                                           	|
| 0x28B	| 651 	| uInt32BE 	| total energy / 10 (kWh)                                                           	|
| 0x28C	| 652 	| uInt32BE 	| total energy / 10 (kWh)                                                           	|
| 0x28D	| 653 	| uInt32BE 	| total energy / 10 (kWh)                                                           	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x2D2	| 722 	| uInt16BE 	| Bus voltage / 10 (V)                                                              	|
| 0x2D3	| 723 	| uInt16BE 	| Bus voltage / 10 (V)                                                              	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x2E0	| 736 	| uInt16BE 	| combinerVoltage group 1 / 10 (V)                                                  	|
| 0x2E1	| 737 	| uInt16BE 	| combinerVoltage group 1 / 10 (V)                                                  	|
| 0x2E2	| 738 	| uInt16BE 	| String current group 1 / 100 (I)                                                  	|
| 0x2E3	| 739 	| uInt16BE 	| String current group 1 / 100 (I)                                                  	|
| ---- 	| --- 	| -------- 	| --------------------------------------------------                                	|
| 0x2E6	| 742 	| uInt16BE 	| combinerVoltage group 2 / 10 (V)                                                  	|
| 0x2E7	| 743 	| uInt16BE 	| combinerVoltage group 2 / 10 (V)                                                  	|
| 0x2E8	| 744 	| uInt16BE 	| String current group 2 / 100 (I)                                                  	|
| 0x2E9	| 745 	| uInt16BE 	| String current group 2 / 100 (I)                                                  	|
| ---- 	| --- 	| -------- 	|                                                                                   	|
| 0x5A3	| 162 	| uInt8    	| checksum - add all bytes, except first, last, and checksum itself, than mod 256   	|
| 0x5A4	| 163 	| uInt8    	| always 15                                                                         	|
