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
-----------------------------------
If you are wondering what the difference between ABS, PLA, Nylon, etc...
Check this out:
https://www.lulzbot.com/sites/default/files/v2//LulzBot_3D_Printing_Filament_Guide.pdf

File Prep (stl or obj)
-----------------------------------

1. Open Meshmixer on the Windows computer and import the .obj or .stl that you want 
    to print using the "import" button on the left tooldbar.
2. Use the Analysis tools in Meshmixer to run any relevant checks using the Taz preset
    when needed. All prints should at least run the 'Units/Dimentions' check to double check that 
    the object is the correct size. It is also a good idea to always run the 
    'Overhangs' test to make sure everything is printable. Run as many
    tests as you think make sence for your particular print. It will save you time
    in the long run to catch any issues now and not 3 hours into the print.
    If there are issues you can either correct them in Meshmixer or the 
    program that was used to create the file.
3. If the file was modified, or is in any format other than .stl, use 
    Meshmixers 'Export' button to export the file as a .stl. Ensure that 
    'STL ASCII FORMAT' is selected in the 'save as type' drop down menu 
    (.obj is the default).
4. Open your newly created .stl file in Netfabb, this can be done by going to 
    'Project->Add Part' and selecting your file in the file browser.
5. Run the part repair tool by going to 'Extras->Repair' part. A 'Part Repair' 
    object will be added to your part. You will also have access to the repair 
    part menu in the lower right panel.
7. Click on the 'Automatic Repair' button, select 'default repair', 
    and click on 'execute' to run the repair script on your object.
8. Apply the repair to your object by clicking on the "Apply Repair" 
    button in the lower right hand corner. You might see a window that asks 
    "You have modified your part. Which action would you want to perform?", 
    if you do click on 'Remove old part'.
9. Export the repaired part using 'Part->Export part->as STL'. 
10. You are all done and ready to print your .stl file, continue on to the "Printing
    Workflow" guide below.

Printing Workflow
-----------------
This is assuming that you have a solid, watertight, printable .stl file all
ready to go. If you are not sure, follow the 'File Prep' guide above.

1. Turn on the printer and wake the PC.
2. Check the filament type currently loaded. Make note of the type of filament:
   is it PLA, HIPS, ABS or something else? If your desired filament is not 
   loaded into the printer, you can learn how to replace the filament by 
   following the "Switching Filament" guide below.
3. Open Repetier Host on the Windows machine.
4. Click the red 'Connect' button in the upper right hand side of the program. 
   If instead you see a green 'Disconnect' button, continue to the next step.
5. Click on the "Manual Control" tab in the top right panel of the program.
6. Turn on the extruder by clicking on the button that looks like a crossed out black
   pencil beside the number one. It is to the left of the lowest temperature gauge
   that corresponds to the first, and only, extruder.
7. Turn on the bed by clicking on the button that looks like a crossed out grid,
   it will be found directly above the extruder button your just pressed.
8. Grab a clean rag and the spray bottle of Alcohol. Spray the bed two or three 
    times and clean off any resedue from the bed. A dirty bed can cause the print
    to separate from the bed, or other issues. Use as much time and alchehol as 
    needed to ensure that the Bed is squeeky clean. This usually takes a few minutes.
9. Load the .stl's you would like to print. First navigate to the 
    'Object Placement' tab, found to the left of the current 
    'Manual Control' tab we have been working out of.
10. Click on the '+' button on the top of the tab. This will prompt you to
    naviage to your file. Select your file and click the 'open' button.
11. If your object needs to be rotated click on the button that looks like a 
    tree with an arrow going around it and rotate your object.
12. If your object is properly rotated, make sure that it is in the center of the bed.
    If it is not, use the object move tool on the left hand toolbar (looks like a cross
    with a moving truck next to it) to reposition your object in the center.
13. Click on the 'Slicer' Tab directly to the right of our current 
    'Object Placement' tab.
14. Make sure that the printer settings drop down is set to "Darling".
15. Make sure the 'Filament settings' are set to the appropriate filament type. 
    For instance, if you are using PLA, make sure that the filament settings 
    for 'Extruder 1' is also set PLA.
16. Likewise, ensure that the 'Print Setting' is set to an appropriate setting. 
    Each filament will have a LQ, MQ, and HQ variant. In general MQ will have 
    the best balence between time and quality, but use LQ for speed and HQ for
    quality. NOTE: You will also find some settings with a sufex of either a D
    or P (e.g. LQD, HQP). The D is for Michael Darling, and those are settings
    that Darling made him self. In general, our settings are better for the 
    current state of the printer, but the 'D' settings are equally valid. The
    P is for prototyping, and means that the layer height will be 0.35mm instead of
    0.175mm, resulting in a print that take half as much time, but is much 'rougher'.
17. Do not use a filament type that does not have a corresponding 'Filament Setting' 
    or 'Print Setting'.
18. Once the correct 'Print Settings', 'Printer Settings', and 'Filament Settings' 
    have been confirmed, click on the 'Slice with Slic3r' button on the top of the 
    'Slicer' panel. This will slice your print and create the code needed to 
    actually print the object.
19. Click on the 'start' button in the main toolbar to begin your print. You might
    have to wait a moment or two as the bed and extruder reach the correct 
    temperature.
20. Keep an eye on the printer as it prints the perimeters. If any issues are not
    corrected by the time the printer starts printing your actual object, press the
    'Kill Print' button in the main toolbar. Remove the failed print, clean the bed,
    correct the problem(s), and start again.
21. Stay close; at least till the printer has printed the 5th or 6th layer. 
22. Once the print is finished, wait for the extruder and bed to cool down 
    before using the X/Y bed movement buttons to position the bed so it is 
    easier to remove your print(s). 
23. Most prints can be pried off the bed with your hands, but some might require
    the help of a putty knife.
24. Once you have removed your print and thrown away any extra unwanted plastic,
    grab a clean rag and the spray bottle of Alcohol. Clean the bed
    in the same manner as before you started your print. For more difficult
    aread feel free to use a putty knife to lightly scrape the surface of the bed.
25. Turn off the printer: the printer should never be left on unless in use.
26. Your done!!!

NOTE: If you are having issues with your print separating from the bed during
printing spray a light coat of "Aqua Net" on the bed before printing. The hair
spray will help the first layer to stick to the bed. Just make sure to spend
some extra time cleaning the bed after you print.

Switching Filament
------------------

1. Make sure that the printer and the PC are turned on.
2. Open Repetier Host on the Windows machine.
3. Click the red 'Connect' button in the upper right hand side of the program to 
    connect the computer with the 3d printer. If instead you see a green 
    'Disconnect' button you do not need to do anything.
4. Click on the 'Manual Control' tab on the top of the right panel in Repetier Host.
5. Turn on the extruder by clicking the button that looks like a crossed out black
   pencil with the number one. It is to the left of the lowest temperature gauge
   that corresponds to the first, and only, extruder.
6. Using the Z Axis control move the extruder to a Z location of about 100.
7. Using the X/Y control move the extruder to the center of the bed, this should
    be about x=150, y=150.
8. Remove the preexisting, unwanted filament using the Extruder control 
    found to the right of the Z contol. Click on '-50' to reverse the extruders 
    feeder and remove the unwanted filament.
9. Put the old spool away in one of the filament bins immediately; this will 
    help ensure the filament maintains a healthy humidity.
10. Place the new filament on the filament holding arm on the right 
    of the printer. 
11. Trim off about 3 inches from the new filament using wire cutters.
12. Take the exposed end of the newly trimmed filament and hang it over 
    the wooden arm before feeding the filiment into the printer. This 
    prevents the filiment from tangleing with itself while being fed into 
    the printer. We use the wooden arm instead of the typical feeding tube.
13. Loosen, but do not unscrew, the two black-topped finger screws that are 
    towards the top of the extruder. This will allow you to move them upwards, 
    unlocking the feeding mechanism for the extruder.
14. Push the end of the new filament into the feeding mechanism and into the 
    extruder below.
15. Close the latch you just opened, and tighten, by hand, the black topped 
    screws you just loosened.
16. Adjust the temperature of the extruder in Repetier Host to be between 10 
    and 20 degrees hotter than the suggested extrusion temperature of the 
    filament. Make sure you take taking the previous filament into account.
    If you are going from ABS to PLA make sure you flush the extruder at at least
    10 degrees above the extruding temperature for ABS, not PLA.
17. Grab a clean rag, or cloth and keep is close.
18. Using the slower option, extrude '10' at a time. Keep and eye on the extruder,
    if the filiment starts to hook back onto the extruder, stop, and use the rag
    (along with the spray bottle, if needed) to clean the extruder before continueing. 
    Repeat until you start to see a descent flow coming out of the extruder. 
19. Once the flow look good, start extruding '100' at a time. Keep an eye on 
    the filament, and extruder. Repeat until you have extruded at least 400 
    total. NOTE: if you are changing filament types extrude AT LEAST 
    800 before continuing.
20. If the extruder is behaving at this point, you are good to start 
    your new print. Follow the 'Printing Workflow' guide above. 

NOTE:
If you are more of a visual learner you can follow this YouTube video, it
is for the Taz 5 and some minor details are different, but it is a valid method: 
https://www.youtube.com/watch?v=8bacfSyy3iI 

IMPORTANT
--------


