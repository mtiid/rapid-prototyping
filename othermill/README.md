In the MTIID Masters Room is an Othermill Pro CNC Mill.

![Othermill Pro](https://othermachine.co/images/othermill-pro-square.jpg)

https://othermachine.co/othermill-pro/

Important Notes
---------------
When the machine is not in use, its power cable should be disconnected and it 
should be covered.

The emergency stop is on the right hand side of the unit, press the button 
if anything goes wrong; such as the board separating from the bed.

Make sure to securely attach your material to the bed. If the PCB is not entirely
covered with double sided stick tape, it will detach from the bed in the 
middle of milling.

Measure your material every time you are doing a new mill. There is a large
variance in produce width, length, and depth when it comes to acrylic, PCB's, and
virtually every other type of millable material. The Othermill is a high
precision machine and these variances will make a difference.

NEVER LEAVE A WORKING MILL UNATTENDED. Stay close, and when you start a mill
plan on sticking around for the entire duration.

Tools and Bits
--------------
We currently have two different bits for the mill. If you are unsure which one
is which, get them both: the smaller one will be the 1/64" flat end mill.

1. Flat end mill, 1/32"
2. Flat end mill, 1/64"

Emergency Stop
--------------
After pressing the emergency stop, pull the button back out of its locked 
position. OtherPlan will prompt you to re-home the spindle. This will move the 
spindle back to its home position. After doing so, you are able to move the bed
into the "loading" position by clicking the appropriate button in OtherPlan.


This will move the material to a location that it can be removed. The OtherMill
has been effectively reset and if another job is started, the mill will 
retain no memory of its previous job. Adjust for the mistakes and restart your 
project. 

Machine Specs
-------------
File Support   : EAGLE .brd, Gerbers, .svg and G-code file formats.

Working Volume : 5.5 x 4.5 x 1.6  in
                 140 x 114 x 40.6 mm

Resolution     : 0.001 in
                 0.25  mm

Trace          : 0.006 in

Full tech specs can be found here :
https://othermachine.co/support/tech-specs/othermill-pro/

Materials
---------
Some materials work great all the time, other should only be messed 
with if you know what you are doing. Let this be the guide.

Work Great:

FR-1 circuit boards
Machining wax
Soft and medium-hard wood (birch plywood)
Linoleum
Machinable foam

Soft plastics (for engraving)
Brass (for engraving)
Aluminum (for engraving)
Silver (for engraving)

Need to do some research before using these:

Hard plastics (Delrin, HDPE)
Aluminum
Brass
Hardwood (mahogany)
Soft stone (soapstone)
Leather (for engraving)

NEVER USE THESE:
Steel, stainless or otherwise
Iron
Magnesium
Titanium
Fiberglass
Hard stone
Glass
Silver chloride (or other powdery materials)
Chocolate, cheese, food, etc.

More information about materials can be found here:
https://othermachine.co/support/materials/welcome/

Workflow
--------
The Mill can be used with either the iMAC or with your own personal
Windows or Mac laptop. If you do use your own machine make sure to
download the OtherPlan software from Other Machine Co before proceeding.

https://othermachine.co/otherplan/

1. Design your PCB in EAGLE CAD. The Othermill can handle 
    boards generated from other sources, but we will assume 
    you are using EAGLE.

After you have removed your mill make sure that all tape residue is also
removed form the bed. 

Use the shop vacuum to vacuum up all of the debris from your mill. Make sure
to do this in both the loading as well as the home positions.

Getting Started
---------------

If you have never used the Othermill before and are interested in using the
mill for PCB prototyping, it is recommended that you start
with the "Hello World" project found on the othermachine website :
https://othermachine.co/support/tutorials/hello-world/

If you do not know how to use EAGLE for the design of circuit boards, and want
to learn this tutorial teaches you the fundamentals all in a way that is centric
to the Othermill workflow: https://othermachine.co/support/tutorials/eagle/

Double Sided PCBs
------------------
Use this site as a guide :
https://othermachine.co/support/pcb/double-sided-boards/

1. It is important when milling double sided boards that you install the
   alignment bracket. If you are unsure as how to do this follow the guide here
   : https://othermachine.co/support/techniques/locating-bracket/ 
   The bracket, three screws, and Allen wrench should be found on top or beside
   the othermill on the "Hello World" board.

   NOTE: MAKE SURE TO REVERSE THE TOOL BEFORE LOCATING THE BRACKET! We do not
   have a probe tool and if you do not reverse one of the bits it will be broken
   by the process. 

   NOTE: ONLY USE FR-1 copperclad, if you use FR-4 the bits WILL BREAK!!!! If
   you don't know what type of copperclad you have, most likely it is FR-4, FR-1
   is much rarer.

2. Measure your board with a caliper and enter its dimentions into Otherplan.
3. Run the appropiate DRC on your board in EAGLE. If you have not already
   installed them they can be found here:
   https://othermachine.co/support/pcb/eagle/
4. Once your board passes the DRC in eagle drag the .brd file into Otherplan.
5. Select the bits you want to use.
6. See if Otherplan recognizes any issues with the board, if there are issues
   correct them in EAGLE.
7. Before milling the top of the board ensure that you deselect the "Outline"
   under the "Parts to Mill" section.
8. Add some offset to the X and Y axis under the "Placement" section. 8mm should
   be good.

   TODO

Tips
----
When cutting harder materials, use shallower cuts to protect the machine.

If cutting a small, deep hole, make sure that the flutes on 
the tools is at least as deep as the hole.

When milling large areas sometimes it can be beneficial to 
use large and small tools to increase tooling time.
