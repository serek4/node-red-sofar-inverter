# byte 0x5D(93 DEC) of data message
##### [back to readme](../README.md#data-messages)
##### [back to KTL-X data msg](decode_data_KTL-X.md)


| bit      	| HEX   	| description                                                	|
|----------	|-------	|------------------------------------------------------------	|
| 00000001 	| +0x01 	| ID09 - PVOVP (PV Over Voltage Protection)                  	|
| 00000010 	| +0x02 	| ID10 - IpvUnbalance (PV Input Current Unbalance)           	|
| 00000100 	| +0x04 	| ID11 - PvConfigSetWrong (PV Input Mode Configure wrong)    	|
| 00001000 	| +0x08 	| ID12 - GFCIFault (Ground-Fault circuit interrupters Fault) 	|
| 00010000 	| +0x10 	| ID13 - PhaseSequenceFault (Phase sequence Fault)           	|
| 00100000 	| +0x20 	| ID14 - HwBoostOCP (hardware boost over current protection) 	|
| 01000000 	| +0x40 	| ID15 - HwAcOCP (Hardware AC over current protection)       	|
| 10000000 	| +0x80 	| ID16 - AcRmsOCP (The Grid current is too high)             	|
