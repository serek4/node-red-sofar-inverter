# HYD6000-ES data message
##### [back to readme](../README.md#data-messages)
V5 table  
208 bytes  
message type 0x2708  
default value type is uInt16LE  

| HEX  	| DEC 	| TYPE     	| VALUE                                                                                                     	|
|------	|-----:	|----------	|--------------------------------------------------------------------------------------------------------------	|
| 0x00 	| 0   	| uInt8    	| always a5                                                                                                 	|
| 0x01 	| 1   	| uInt16LE 	| always C3 msg length - excl msg header(0x00 - 0x0A), checksum and last byte                               	|
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
| 0x0C 	| 12  	| uInt16LE 	| always 08 Sensor Type List?                                                                               	|
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
| 0x30 	| 48  	| uInt16LE	| DC PV1 Voltage(V) /10                                                                                     	|
| 0x31 	| 49  	| uInt16LE 	| DC PV1 Voltage(V) /10                                                                                     	|
| 0x32 	| 50  	| uInt16LE 	| DC PV1 current(A) /100 ?                                                                                  	|
| 0x33 	| 51  	| uInt16LE 	| DC PV1 current (A) /100 ?                                                                                 	|
| 0x34 	| 52  	| uInt16LE 	| DC PV1 Power(W) * 10                                                                                      	|
| 0x35 	| 53  	| uInt16LE 	| DC PV1 Power(W) * 10                                                                                      	|
| 0x36 	| 54  	| uInt16LE 	| DC PV2 Voltage /10                                                                                        	|
| 0x36 	| 55  	| uInt16LE 	| DC PV2 Voltage /10                                                                                        	|
| 0x38 	| 56  	| uInt16LE 	| DC PV2 current(A) /100 ?                                                                                  	|
| 0x37 	| 57  	| uInt16LE 	| DC PV2 current(A) /100 ?                                                                                  	|
| 0x3A 	| 58  	| uInt16LE 	| DC PV2 Power(W) * 10                                                                                      	|
| 0x3B 	| 59  	| uInt16LE 	| DC PV2 Power(W) * 10                                                                                      	|
| 0x3C 	| 60  	| uInt16LE 	| AC Voltage(V) /10                                                                                         	|
| 0x3D 	| 61  	| uInt16LE 	| AC Voltage(V) /10                                                                                         	|
| 0x3E 	| 62  	| uInt16LE 	| AC Current(A) /100                                                                                        	|
| 0x3F 	| 63  	| uInt16LE 	| AC Current(A) /100                                                                                        	|
| 0x40 	| 64  	| uInt16LE 	| AC Frequency (HZ) /100                                                                                    	|
| 0x41 	| 65  	| uInt16LE 	| AC Frequency (HZ) /100                                                                                    	|
| 0x42 	| 66  	| Int16LE 	| Battery Power (W) * 10                                                                                    	|
| 0x43 	| 67  	| Int16LE 	| Battery Power (W) * 10                                                                                    	|
| 0x44 	| 68  	| uInt16LE 	| Battery Voltage (V) /10                                                                                   	|
| 0x45 	| 79  	| uInt16LE 	| Battery Voltage (V) /10                                                                                   	|
| 0x46 	| 70  	| Int16LE 	| Battery Current (A) /100                                                                                  	|
| 0x47 	| 71  	| Int16LE 	| Battery Current (A) /100                                                     	                            	|
| 0x48 	| 72  	| uInt16LE 	| Remaining Battery Capacity (SoC) (%)                                                                      	|
| 0x49 	| 73  	| uInt16LE 	| Remaining Battery Capacity (SoC) (%)                                                                      	|
| 0x4A 	| 74  	| uInt16LE 	| Battery Temperature (C)                                                                                   	|
| 0x4B 	| 75  	| uInt16LE 	| Battery Temperature (C)                                                                                   	|
| 0x4C 	| 76  	| uInt16LE 	| Storage in/out power (W)                                                                                  	|
| 0x4D 	| 77  	| uInt16LE 	| Storage in/out power (W)                                                                                  	|
| 0x4E 	| 78  	| uInt16LE 	| Total Consumption Power (W) x10                                                                           	|
| 0x4F 	| 79  	| uInt16LE 	| Total Consumption Power (W) x10                                                                           	|
| 0x50 	| 80  	| uInt16LE 	| ????                                                                                                      	|
| 0x51 	| 81  	| uInt16LE 	| ????                                                                                                      	|
| 0x52 	| 82  	| uInt16LE 	| AC Output Total Power (W) x10                                                                             	|
| 0x53 	| 83  	| uInt16LE 	| AC Output Total Power (W) x10                                                                             	|
| 0x54 	| 84  	| uInt16LE 	| Emergency Output Voltage (V) /10                                                                          	|
| 0x55 	| 85  	| uInt16LE 	| Emergency Output Voltage (V) /10                                                                          	|
| 0x56 	| 86  	| uInt16LE 	| Emergency Output Power (W) x10                                                                            	|
| 0x57 	| 87  	| uInt16LE 	| Emergency Output Power (W) x10                                                                            	|
| 0x58 	| 88  	| uInt16LE 	| Daily Generation (Active) (kWh) /100                                                                      	|
| 0x59 	| 89  	| uInt16LE 	| Daily Generation (Active) (kWh) /100                                                                      	|
| 0x5A 	| 90  	| uInt16LE	| Daily on grid Energy (kWh) /100                                                                           	|
| 0x5B 	| 91  	| uInt16LE 	| Daily on grid Energy (kWh) /100                                                                           	|
| 0x5C 	| 92  	| uInt16LE 	| Daily Energy Purchased (kWh) /100                                                                         	|
| 0x5D 	| 93  	| uInt16LE 	| Daily Energy Purchased (kWh) /100                                                                         	|
| 0x5E 	| 94  	| uInt16LE 	| Daily Energy Used (kWh) /100                                                                              	|
| 0x5F 	| 95  	| uInt16LE 	| Daily Energy Used (kWh) /100                                                                              	|
| 0x60 	| 96  	| uInt16LE 	| Total Generation (Active) (kWh)                                                                           	|
| 0x61 	| 97  	| uInt16LE 	| Total Generation (Active) (kWh)                                                                           	|
| 0x62 	| 98  	| uInt16LE 	| always 00 ?                                                                                               	|
| 0x63 	| 99  	| uInt16LE 	| always 00 ?                                                                                               	|
| 0x64 	| 100 	| uInt16LE 	| Total On-grid Generation (kWh)                                                                            	|
| 0x65 	| 101 	| uInt16LE 	| Total On-grid Generation (kWh)                                                                            	|
| 0x66 	| 102 	| uInt16LE 	| always 00 ?                                                                      	                        	|
| 0x67 	| 103 	| uInt16LE 	| always 00 ?                                                                      	                        	|
| 0x68 	| 104 	| uInt32LE  | Total Energy Purchased (kWh)                                                                              	|
| 0x69 	| 105 	| uInt32LE  | Total Energy Purchased (kWh)                                                                              	|
| 0x6A 	| 106 	| uInt32LE  | Total Energy Purchased (kWh)                                                                              	|
| 0x6B 	| 107 	| uInt32LE  | Total Energy Purchased (kWh)                                                                              	|
| 0x6C 	| 108 	| uInt32LE  | Total Consumption Energy (kWh)                                                                            	|
| 0x6D 	| 109 	| uInt32LE  | Total Consumption Energy (kWh)                                                                            	|
| 0x6E 	| 110 	| uInt32LE  | Total Consumption Energy (kWh)                                                                            	|
| 0x6F 	| 111 	| uInt32LE  | Total Consumption Energy (kWh)                                                                            	|
| 0x70 	| 112 	| uInt16LE  | Battery Daily Energy Discharged (kWh) /100                                                                	|
| 0x71 	| 113 	| uInt16LE  | Battery Daily Energy Discharged (kWh) /100                                                                	|
| 0x72 	| 114 	| uInt16LE 	| Battery Daily Energy Charged (kWh) /100                                                                   	|
| 0x73 	| 115 	| uInt16LE 	| Battery Daily Energy Charged (kWh) /100                                                                   	|
| 0x74 	| 116 	| uInt32LE 	| Battery Total Energy Charged (kWh)                                                                        	|
| 0x75 	| 117 	| uInt32LE 	| Battery Total Energy Charged (kWh)                                                                        	|
| 0x76 	| 118 	| uInt32LE 	| Battery Total Energy Charged (kWh)                                                                        	|
| 0x77 	| 119 	| uInt32LE 	| Battery Total Energy Charged (kWh)                                                                        	|
| 0x78 	| 120 	| uInt32LE 	| Battery Total Energy Discharged (kWh)                                                                     	|
| 0x79 	| 121 	| uInt32LE 	| Battery Total Energy Discharged (kWh)                                                                     	|
| 0x7A 	| 122 	| uInt32LE 	| Battery Total Energy Discharged (kWh)                                                                     	|
| 0x7B 	| 123 	| uInt32LE 	| Battery Total Energy Discharged (kWh)                                                                     	|
| 0x7C 	| 124 	| uInt16LE 	| 02                                                                                                        	|
| 0x7D 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0x7E 	| 126 	| uInt16LE 	| ????                                                                                                      	|
| 0x7F 	| 127 	| uInt16LE 	| ????                                                                                                      	|
| 0x80 	| 128 	| uInt16LE 	| Battery Total Charging/Discharging Times                                                                  	|
| 0x81 	| 129 	| uInt16LE 	| Battery Total Charging/Discharging Times                                                                  	|
| 0x82 	| 130 	| uInt16LE 	| Bus Voltage (V) /10                                                                                       	|
| 0x83 	| 131 	| uInt16LE 	| Bus Voltage (V) /10                                                                                       	|
| 0x84 	| 132 	| uInt16LE 	| LLCBus Voltage (V) /10                                                                                    	|
| 0x85 	| 133 	| uInt16LE 	| LLCBus Voltage (V) /10                                                                                    	|
| 0x86 	| 134 	| uInt16LE 	| Buck Current (A)  /100                                                                               	    	|
| 0x87 	| 134 	| uInt16LE 	| Buck Current (A)  /100                                                                                    	|
| 0x88 	| 134 	| uInt16LE 	| Power Grid Voltage R/U/A(V) /10                                                                           	|
| 0x89 	| 134 	| uInt16LE 	| Power Grid Voltage R/U/A (V) /10                                                                          	|
| 0x8A 	| 138 	| uInt16LE 	| Power Grid Current R/U/A (A) /100                                                                         	|
| 0x8B 	| 139 	| uInt16LE 	| Power Grid Current R/U/A (A) /100                                                                         	|
| 0x8C 	| 140 	| uInt16LE 	| 64                                                                                                        	|
| 0x8D 	| 141 	| uInt16LE 	| 00                                                                                                        	|
| 0x8E 	| 142 	| uInt16LE 	| Inverter Temperature (C)                                                                                  	|
| 0x8F 	| 143 	| uInt16LE 	| Inverter Temperature (C)                                                                                  	|
| 0x90 	| 144 	| uInt16LE 	| Radiator Temperature (C)                                                                                  	|
| 0x91 	| 145 	| uInt16LE 	| Radiator Temperature (C)                                                                                  	|
| 0x92 	| 146 	| uInt16LE 	| 01                                                                                                        	|
| 0x93 	| 147 	| uInt16LE 	| 00                                                                                                        	|
| 0x94 	| 148 	| int16LE 	| Current DC Component                                                                                      	|
| 0x95 	| 149 	| int16LE 	| Current DC Component                                                                                      	|
| 0x96 	| 150 	| int16LE  	| Voltage DC Component                                                                                      	|
| 0x97 	| 151 	| int16LE  	| Voltage DC Component                                                                                      	|
| 0x98 	| 152 	| int16LE  	| 00                                                                                                        	|
| 0x99 	| 153 	| int16LE  	| 00                                                                                                        	|
| 0x9A 	| 154 	| int16LE 	| 00                                                                                                        	|
| 0x9B 	| 155 	| int16LE 	| 00                                                                                                        	|
| 0x9C 	| 156 	| int16LE 	| 00                                                                                                        	|
| 0x9D 	| 157 	| int16LE 	| 00                                                                                                        	|
| 0x9E 	| 158 	| int16LE 	| 00                                                                                                        	|
| 0x9F 	| 159 	| int16LE 	| 00                                                                                                        	|
| 0xA0 	| 160 	| int16LE 	| 00                                                                                                        	|
| 0xA1 	| 161 	| int16LE 	| 00                                                                                                        	|
| 0xA2 	| 125 	| int16LE 	| 00                                                                                                        	|
| 0xA3 	| 125 	| int16LE 	| 00                                                                                                        	|
| 0xA4 	| 125 	| uInt8 	| Daily generating Hours (h)                                                                                	|
| 0xA5 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xA6 	| 125 	| uInt32LE 	| Total Generating Hours (h)                                                                                	|
| 0xA7 	| 125 	| uInt32LE 	| Total Generating Hours (h)                                                                                	|
| 0xA8 	| 125 	| uInt32LE 	| Total Generating Hours (h)                                                                                	|
| 0xA9 	| 125 	| uInt32LE 	| Total Generating Hours (h)                                                                                	|
| 0xAA 	| 125 	| uInt16LE 	| Insulation impedance to ground PV2                                                                        	|
| 0xAB 	| 125 	| uInt16LE 	| Insulation impedance to ground PV2                                                                       		|
| 0xAC 	| 125 	| uInt16LE 	| Insulation impedance-PV to ground                                                                         	|
| 0xAD 	| 125 	| uInt16LE 	| Insulation impedance-PV to ground                                                                    	    	|
| 0xAE 	| 125 	| uInt16LE 	| Insulation impedance-Cathode to ground                                                                    	|
| 0xAF 	| 125 	| uInt16LE 	| Insulation impedance-Cathode to ground                                                                    	|
| 0xB0 	| 125 	| uInt16LE 	| 02                                                                                                        	|
| 0xB1 	| 125 	| uInt16LE 	| 00                                                                                                   	    	|
| 0xB2 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB3 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB4 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB5 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB6 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB7 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB8 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xB9 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xBA 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xBB 	| 125 	| uInt16LE 	| 00                                                                                                        	|
| 0xBC 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xBD 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xBE 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xBF 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC0 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC1 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC2 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC3 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC4 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC5 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC6 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC7 	| 125 	| uInt16LE 	| ????                                                                                                      	|
| 0xC8 	| 125 	| uInt8 	| Year                                                                                                      	|
| 0xC9 	| 125 	| uInt8 	| Month                                                                                                     	|
| 0xCA 	| 125 	| uInt8 	| Day                                                                                                       	|
| 0xCB 	| 125 	| uInt8 	| Hour                                                                                                      	|
| 0xCC 	| 125 	| uInt8 	| Minute                                                                                                    	|
| 0xCD 	| 125 	| uInt8 	| Second                                                                                                    	|
| 0xCE 	| 125 	| uInt8 	| checksum - add all bytes, except first, last, and checksum itself, than mod 256                           	|
| 0xCF 	| 125 	| uInt8 	| always 15                                                                 	                            	|
