// LulzBot

The 3D printer that is living in the vault is a LulzBot
Taz.

The Windows desktop this also resides in the vault is the control
center for the printer as well as the CNC router. 
The Vault also contains at least one bin full of filament. 
There is also a drawer drectly below the printer in the vault 
that houses various replacement parts and tools for repairing the printer.

Take special note of the filament that the printer is currently using and
the type a filament you are about to use: using the incorrect printer settings
can cause damage to the extruder.

Filament Guide
--------------
If you are wondering what the difference between ABS, PLA, Nylon, etc...
Check this out:
https://www.lulzbot.com/sites/default/files/v2//LulzBot_3D_Printing_Filament_Guide.pdf

File Prep
---------

Printing Workflow
-----------------
This is assuming that you have a solid, watertight, printable .stl file all
ready to go. If you are not sure, follow the 'File Prep' guide above.

1. Turn on the printer and wake the PC.
2. Check the filament type currently loaded. Make note of the type of filament:
   is it PLA, HIPS, ABS or something else?
3. If this is not your desired filament, switched the filament out following
   the "Switching Filament" guide below.
4. Open Repetier Host on the Windows machine.
5. Click the red "Connect" button in the upper right hand side of the program. 
   If instead you see a green "Disconnect" button you do not need to do anything.
6. Click on the "Manual Control" tab on the top of the right panel in Repetier Host.
7. Turn on the extruder by clicking on the button that looks like a crossed out black
   pencil with the number one. If will be to the left of the lowest temperature gauge
   that corresponds to the first, and only, extruder.
9. Turn on the bed by clicking on the button that looks like a crossed out grid,
   if will be found directly above the extruder button your just pressed.
10. Grab a clean rag and the spray bottle of Alcohol. Spray the bed two or three 
    times and clean off any resedue from the bed. A dirty bed can cause the print
    to separate from the bed, or other issues. Use as much time and alchehol as 
    needed to ensure that the Bed is squeeky clean.
10. While the bed and extruder heat up load the .stl's you would like to print. 
    First naviagate to the 'Object Placement' tab, found to the left of the current 
    'Manual Control' tab we have been working out of.
11. Click on the '+' button on the top of the tab. This will prompt you to
    naviage to your file. Select your file and click the 'open' button.
12. If your object needs to be rotated click on the button that looks like a 
    tree with an arrow going around it.
13. If your object is properly rotated, make sure that it is in the center of the bed.
    If it is not, use the object move tool on the left hand toolbar (looks like a cross
    with a moving truck next to it) to reposition your object in the center.
14. Next click on the 'Slicer' Tab directly to the right of our current 
    'Object Placement' tab.
15. Make sure that the printer settings drop down is set to "Darling"
16. Make sure the Filament settings are set to the appropriate filament type. 
    For instance, if you are using PLA, make sure that the filament settings 
    for Extruder 1 is also set PLA.
17. Likewise, ensure that the Print Setting is set to an appropriate setting. 
    Each filament will have a LQ, MQ, and HQ variant. In general MQ will have 
    the best balence between time and quality, but use LQ for speed and HQ for
    quality. NOTE: You will also find some settings with a sufex of either a D
    or P (e.g. LQD, HQP). The D is for Michael Darling, and those are settings
    that Darling made him self, in general our settings are better for the 
    current state of the printer, but the 'D' settings are equally valid. The
    P is for prototyping, and means that the layer height will be 0.35mm instead of
    0.175mm, resulting in a print that take half as much time, but is much 'rougher'.
18. Do not use a filament type that does not have a corresponding Filament Setting 
    or Print Setting.
19. Once the correct Print Settings, Printer Settings, and Filament Settings 
    have been confirmed click on the "Slice with Slic3r" button on the top of the 
    'Slicer' panel. This will slice your print and create the code needed to 
    actually print the object.
20. Keep an eye on the printer as it prints the perimeters. If any issues are not
    corrected by the time the printer starts printing your actual object, press the
    'Kill Print' button in the main toolbar. Remove the failed print, clean the bed,
    correct the problems and start again.
21. Stay close at least till the printer has printed the 5th or 6th layer. 
22. Once the print is finished, wait for the extruder and bed to cool down 
    before using the X/Y bed movement buttons to position the bed so it is 
    easier to remove your prints. 
23. Most prints can be pried off the bed with your hands, but some might require
the help of a putty knife.
24. Once you have removed your print and thrown away any extra unwanted plastic
    grab a clean rag and the spray bottle of Alcohol and clean the bed 
    in the same manner as before you started your print. For more difficult
    area feel free to use a putty knife to lightly scrape the surface of the bed.
26. Turn off the printer: the printer should never be left on unless in use.
27. Your done!!!

NOTE: If you are having issues with your print separating from the bed during
printing spray a light coat of "Aqua Net" on the bed before printing. The hair
spray will help the first layer to stick to the bed. Just make sure to spend
some extra time cleaning the bed after you print.

Switching Filament
------------------

1. Make sure that the printer and the PC are turned on.
2. Open Repetier Host on the Windows machine.
3. Click the red "Connect" button in the upper right hand side of the program. 
    If instead you see a green "Disconnect" button you do not need to do anything.
4. Click on the "Manual Control" tab on the top of the right panel in Repetier Host.
5. Turn on the extruder by clicking on the button that looks like a crossed out black
   pencil with the number one. If will be to the left of the lowest temperature gauge
   that corresponds to the first, and only, extruder.
6. Using the Z Axis control move the extruder to a Z location of about 100.
7. Using the X/Y control move the extruder to the center of the bed, this should
    be about x=150, y=150.
8. We will remove the preexisting, unwanted filament using the Extruder control 
    found on the right of the Z contol. Click on -50 to reverse the extruders 
    feeder and remove the unwanted filament.
9. Put the old spool away in one of the filament bins immediately, this will 
    help ensure the filament maintains a healthy humidity.
10. Place the new filament on the filament holding arm on the right hand side 
    of the printer. 
11. Trim off about 3 inches from the new filament using wire cutters.
12. Take the exposed end of the newly trimmed filament and hang it over 
    the wooden arm before feeding the filiment into the printer. This 
    prevents the filiment from tangleing with itself while being fed into 
    the printer. We use the wooden arm instead of the typical feeding tube.
13. Loosen but do not unscrew the two black topped finger screws that are 
    towards the top of the extruder. This will allow you to move them upwards, 
    unlocking the feeding mechanism for the extruder.
14. Push the end of the new filament into the feeding mechanism and into the 
    extruder below.
15. Close the latch you just opened, and tighten, by hand, the black topped 
    screws you just loosened.
16. Adjust the temperature on the extruder in Repetier Host to be between 10 
    and 20 degrees hotter than the suggested extrusion temperature of the 
    filament with the HIGHEST extrusion temperature between the new and old 
    filaments.
17. Grab a clean rag, or cloth and keep is close.
18. Using the slower option, extrude '10' at a time. Keep and eye on the extruder,
    if the filiment starts to hook back onto the extruder, stop, and use the rag
    (along with alehol, if needed) to clean the extruder before continueing. 
    Repeat until you start to see a descent flow coming out of the extruder. 
19. Once the flow look good, start extruding '100' at a time. Keep an eye on 
    the filament, and extruder. Repeat until you have extruded at least 400 
    total. NOTE: if you are changing filament types extrude AT LEAST 
    800 before continuing.
20. If the extruder is behaving at this point you are good to go and start 
    your new print. Follow the 'Printing Workflow' guide above. 

NOTE:
If you are more of a visual learner you can follow this YouTube video, it
is for the Taz 5 and some minor details are different, but it is a valid method: 
https://www.youtube.com/watch?v=8bacfSyy3iI 

IMPORTANT
--------


