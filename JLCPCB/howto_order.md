
# PiStorm32-lite
## How to place the order at JLCPCB


- Logic or create a account at [JLCPCB](https://jlcpcb.com/)
- Click on `Instant Quote`
- Upload the ZIP File with the Gerbers

----

First the PCB, if you only want a unpopulated PCB you can of course skip the Assembly part :)

----

## PCB

Check if the Gerber upload looks good
![image](https://user-images.githubusercontent.com/16537586/209685556-d3cc3a82-35e2-4e17-a244-9d06ec218159.png)

Check the PCB specs (you can also pick a different color or PCB finish of course)
![image](https://user-images.githubusercontent.com/16537586/209685439-210eebbd-23ba-4b1e-b0ce-1080b9d64838.png)

Check that "Remove Order Number" is set like this
![image](https://user-images.githubusercontent.com/16537586/209685729-41ddc5da-2b60-4a00-9ca9-ae321e570e9a.png)

----

## Assembly

Select "Top Side" for Assembly and set the tooling holes to "Added by Customer"
![image](https://user-images.githubusercontent.com/16537586/209685920-51f3b4be-1853-4205-af90-4a274b0c1dd1.png)

Continue to the next Page to upload the BOM (Bill of Material) and CPL (Pick and Place Machine coordinates) files.
You also need to specify the intended use for the assembled PCB, thats for Tax/Customs reasons only. I usually pick
the Research/DIY/Hobby category.

![image](https://user-images.githubusercontent.com/16537586/209686510-3243b341-27c5-4b67-83ee-78ea4c0cbf0e.png)

On the next Page you can check the BOM upload and matching to JLCPCB part numbers and stock levels.
For all parts you can also select alternatives from JLCPCBs stock (Loupe symbol), or like in the case of the EFINIX FPGA which
isn't yet on the JLCPCBs stock list, select a part you ordred before at the JLCPCB Global Parts Sourcing Service.
Keep in mind that the Parts you ordered that way must first arrive at the JLCPCB warehouse before the assembly and data prepareation can start.
This takes usually around a week, and you get a email notification when the parts arrived.

![image](https://user-images.githubusercontent.com/16537586/209687242-46d7909e-16a0-41c1-ad80-d88bd600b1a9.png)

When all looks good and the parts, or alternative parts you selected, are on stock proceed to the last page.
Here you can check the placement of the parts prior soldering. JLCPCB corrects small errors like rotated parts, but 
they cant correct errors where, for example, a part is selected with the wrong footprint. So check the picture closely and
if in doubt better double check :) The rendering is not perfect, like the FPGA is missing completly in the rendering.
But when you are sure the part is on stock and you selected it in the BOM page then just trust in JLCPCB. They contact you
also if there is a problem they cant fix by themself for you.

![image](https://user-images.githubusercontent.com/16537586/209687752-1985bd95-27e1-48ee-9a14-f137424708e8.png)

Thats it! Now lean back and wait some days for your assembled PiStorm32-lite boards to arrive 




