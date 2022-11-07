# byte 0x5A(90 DEC) of data message
##### [back to readme](../README.md#data-messages)
##### [back to KTL-X data msg](decode_data_KTL-X.md)


| bit      	| HEX   	| description                                                 	|
|----------	|-------	|-------------------------------------------------------------	|
| 00000001 	| +0x01 	| ID17 - HwADFaultIGrid (The Grid current sampling is error)  	|
| 00000010 	| +0x02 	| ID18 - HwADFaultDCI (The DCI sampling is error)             	|
| 00000100 	| +0x04 	| ID19 - HwADFaultVGrid (The Grid voltage sampling is error)  	|
| 00001000 	| +0x08 	| ID20 - GFCIDeviceFault (GFCI device sampling is error)      	|
| 00010000 	| +0x10 	| ID21 - MChip_Fault (Main chip fault)                        	|
| 00100000 	| +0x20 	| ID22 - HwAuxPowerFault ( Hardware auxiliary power fault)    	|
| 01000000 	| +0x40 	| ID23 - BusVoltZeroFault (Bus voltage zero fault)            	|
| 10000000 	| +0x80 	| ID24 - IacRmsUnbalance (The output current is not balanced) 	|
