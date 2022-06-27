# Retroninja 1541 Switchless Multi-ROM
<img src="rev1.1\images\render-top.png" alt="Render top" width="800"/><br/>
A microcontroller based switchless ROM switcher for the Commodore 1541 disk drive.
Switch between stock CBM DOS, JiffyDOS and other ROMs by issuing commands from Basic.
No computer modifications or drive enclosure modifications needed. Completely reversible drive modification.

Read the user's guide for more information. 

# A new revision of this board has been released under the more generic name [Switchless Multi-ROM for 2364](https://github.com/RetroNynjah/Switchless-Multi-ROM-for-2364)


## WARNING!
There's a bug in the current revision of this design. The A16 address pin is incorrectly connected to a pure analog input on the ATmega and can't be controlled. This causes the address pin on the flash chip to float and the upper half of the ROM can't be used. If you are using this version you can only use the lower half of the ROM and the contents in the upper half needs to be an exact copy of the lower half. Another workaround could be to tie pin 2 of the flash chip or pin 19 of the ATmgea to GND using a bodge wire.
  
  
<img src="rev1.1\images\3Dpcb-top.png" alt="Render top" height="800"/>  <img src="rev1.1\images\3Dpcb-bottom.png" alt="Render bottom" height="800"/><br/>

## BOM
 |Component|Pcs |Name|Comment|
 |:--------|---:|:---|:------|
 | SST39SF010A | 1 | IC1 | Flash. SST39SF020/040 should work too. PLCC-32 |
 | ATMEGA328P-AU | 1 | IC2 | Or compatible ATmega8/48/88/168/328 variants. TQFP-32 |
 | 74AHCT273NSR | 1 | IC4 | Flip-Flop SO-20 (5.3mm width) |
 | 74AHCT1G04 | 1 | IC5 | Inverter single gate SOT-23 |
 | 100nF ceramic capacitor | 4 | C1, C2, C3, C4 | 0805 |
 | 30pF ceramic capacitor | 2 | C5, C6 | 0805 - 22pF works too |
 | 10k resistor | 1 | R1 | 0805 |
 | 560R resistor | 1 | R2 | 0805 - LED current limiting resistor|
 | LED | 1 | D1 | 0805 |
 | ECS-160-20-3X-TR | 1 | XTAL1 | Crystal 16MHz |
 | 12 pin header | 2 | "IC3" | Male machined pin headers or flat headers. 2.54mm pitch. To fit DIL-24 socket. |
 | 6 pin header right-angled | 1 | JP1 | Optional 2.54mm pitch. For ISP programmer. |
