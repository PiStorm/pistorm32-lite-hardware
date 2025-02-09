# PiStorm32-lite
## An Opensource, Raspberry Pi based, Amiga A1200 Accelerator

This repository holds all hardware design and fabrication files



---


PiStorm32-lite is compatible with 
- PI3A
- PI3B
- PI4B
- PiZero2 (could be very tight around the HDMI connector...)

- Raspberry CM4 (Recommended Version : CM4 Lite, 2GB RAM with WIFI and no eMMC) trough a adapter
  https://github.com/PiStorm/cm4board

And soon there will be a custom made CM4 adapter for PiStorm32-lite.
The custom made adapter will offer the best cooling in the constrained space available and convenient access to all IOs (HDMI,USB,Ethernet)
through the A1200 Module Slot near the Joystick/Mouse ports without modifications to the Amiga case.


![image](https://user-images.githubusercontent.com/16537586/209653456-0dadc99d-8447-41e0-b1e9-c29c1a3ce5f9.png)

## Direct links
- [Schematics (and assembly drawing)](PDF/ps32_lite_rev_a_public_schematic.pdf)
- [Altium project](Altium/)
- [Fabrication files](Fabrication%20Files/)
- [Fabrication files for JLCPCB Assembly (With small ordering Howto)](JLCPCB/)

---

The community around the PiStorm Project is best reached on Discord

[![](https://dcbadge.vercel.app/api/server/vyHr6nQeGn)](https://discord.gg/vyHr6nQeGn)

---
> IMPORTANT NOTE: `Isolate the PI GPIO and Ethernet Pins from the A1200 Keyboard, that can be done by 2  or 3 layers of tape attached to the keyboard backside where the Pi pins would touch the metal`
If you don't do that, you likely fry your Pi ! Sorry couldn't design it an other way, there is not much space in the A1200 trapdoor bay 
---

Beside the PCB you also need following parts:

| Designator  | Part | Quantity | Notes
| ------ | ------ | ----- | ----- |
| C1 to C16, C23, C24 | 100nF 0603 | 18 | X7R 
| C17, C18, C19, C20, C21, C22 | Tantalum 10uF 16V Size B| 6 | --
| D1 | BAT54C | 1 | --
| EXT | 2.54mm Pin Header 2x5 10 Pins | 1 | Expansion header for the future :) e.g.  B-2100S10P-B110
| M1,M2,M3 | SMD M2.5 NUT | 3 | e.g. Sinhoo SMTSO2515CTJ
| LED_1.2, LED_3.3, LED_FPGA, LED_PI | RED LED 0805 | 4 | Indicate not Illuminate!
| PI | SMD 40Pin 2x20 - bottom entry | 1 | e.g. Liansheng FH-00369 
| CN1 | A1200 Edge connector | 1 | see links and notes
| Q1 | IRML6401 | 1 | --
| Q2, Q3, Q4, Q5, Q6 | BC847B | 5 | --
| R2, R4, R5, R6, R7, R8, R9, R10, R19 | Resistor 0603 10kOhm | 9 | --
| R3, R13, R16, R17, R18 | Resistor 0603 1kOhm | 5 | --
| RN1, RN2, RN3, RN4, RN5, RN6, RN7, RN8, RN9| Resistor Array 0603x4 10kOhm | 9 | e.g. YAGEO YC164-JR
| RN10 | Resistor Array 0603x4 1kOhm | 1 | e.g. YAGEO YC164-JR
| U1 | FPGA Efinix Trion T8Q144C4 (or C3) | 1 | see links and notes
| U2, U3, U4, U5, U6, U7 | 74CBTD3384 TSSOP-24 | 6 | TI or NXP
| U8, U9, U10, U11 | 74LVC573A TSSOP-20 | 4 | TI or NXP
| U12 | AMS1117-3.3 3.3V LDO | 1 | --
| U13 | AMS1117-3 1.2 1.2V LDO | 1 | --

> Note: A1200 Edge Connectors can be purchased at [retroready.one](https://retroready.one/products/amiga-1200-genuine-expansion-card-edge-connector-brand-new?_pos=1&_sid=b7b91e722&_ss=r)(UK based, highly recommended) or [amigastore.eu](https://amigastore.eu/en/738-amiga-1200-accelerator-connector-for-the-edge-expansion-port.html)(EU based) or [Sordan](https://sordan.ie/product/670/150-pin-90-degrees-amiga-1200-edge-expansion-card-connector/)(Ireland/EU based)

> Note: JLCPCB does not stock the Efinix FPGA, but can source that part trough their [global parts sourcing service](https://jlcpcb.com/help/article/60-How-to-use-JLCPCB-Global-Sourcing-Parts-Service). If you want to assemble the PCB by yourself, or order a partially assembeld PCB without the FPGA then here is a link to Digikey [Digikey FPGA](https://www.digikey.com/short/zh3ph422)

For mechanical assembly you need :

- 3 M2.5 Screws with 8mm thread length (M2.5x8)
- 3 Spacers ID=2.6mm Length=3.0mm 
- 1 Thermal Pad with 1mm thickness, just needs to be big enough to cover the PI CPU 

There are also some [pictures here](Pictures/) how to attach the thermal pad and screws

---

If you like this project and want to support me (Claude Schwarz, PiStorm Hardware) with a donation, I finally setup a donate button :)

The donations will go into further development of open source PiStorm hardware.

   [![](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=JQC4M73U9KKPG)
