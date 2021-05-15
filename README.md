# Retroninja 1541 Switchless Multi-ROM
<img src="rev1.1\images\render-top.png" alt="Render top" width="800"/><br/>
A microcontroller based switchless ROM switcher for the Commodore 1541 disk drive.
Switch between stock CBM DOS, JiffyDOS and other ROMs by issuing commands from Basic.
No computer modifications or drive enclosure modifications needed. Completely reversible drive modification.

Read the user's guide for more information. 
 
<img src="rev1.1\images\3Dpcb-top.png" alt="Render top" height="800"/>  <img src="rev1.1\images\3Dpcb-bottom.png" alt="Render bottom" height="800"/><br/>

## BOM
 |Component|Pcs |Name|Comment|
 |:--------|---:|:---|:------|
 | SST39SF010A | 1 | IC1 | 32PLCC Flash. SST39SF020/040 should work too.|
 | ATMEGA328P-AU | 1 | IC2 | 32TQFP |
 | 74AHCT273NSR | 1 | IC4 | 20-SO (5.3mm width) |
 | 741G04 | 1 | IC5 | Inverter single gate SOT-23 |
 | 100nF ceramic capacitor | 4 | C1, C2, C3, C4 | 0805 |
 | 30pF ceramic capacitor | 2 | C5, C6 | 0805 - 22pF works too |
 | 10k resistor | 1 | R1 | 0805 |
 | 560R resistor | 1 | R2 | 0805 - LED current limiting resistor|
 | LED | 1 | D1 | 0805 |
 | ECS-160-20-3X-TR | 1 | XTAL1 | Crystal 16MHz |
 | 12 pin header | 2 | "IC3" | Male machined pin headers. 2.54mm pitch. To fit DIL-24 socket. |
 | 6 pin header right-angled | 1 | JP1 | Optional 2.54mm pitch. For ISP programmer. |
