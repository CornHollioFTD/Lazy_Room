How to use Lazy Room to generate JSONs with orders:


0. Use Super Lazy Launcher.


As the name implies it will:
- check for and install new release of LZR,
- download and unzip fresh validator from your War Room,
- setup settings.txt with paths, etc.


How to use this:
1. Put Super Lazy Launcher.exe in your WAW folder.
2. Run it.

3. At first start, it will download new LZR and will warn you that it cannot download validator.
4. You need to enter your secret code from War Room. It's a bunch of numbers and letters in the link.
5. Do not share this code with anyone.
6. After entering the code - press "Download validator" to try it again.
7. If all worked as it should - press "Start LZR". And form orders as usual.
Important!
New structure for folders ⚠️ 

\WAW\Super Lazy Launcher.exe
\WAW\Lazy Room\Lazy Room.exe
\WAW\Turns\order_validation_3_MOVE\urc_turn_3_MOVE.json
\WAW\OBJ\
\WAW\Sprites\








1. Create a folder for files with turn information and other WAW stuff.
E.g.: C:\WAW\

2. Download and unrar the latest version of Lazy Room.

3. If you want to import your models or images, create folders for them.
E.g.: C:\WAW\OBJ\ and C:\WAW\Sprites\

4. In the folder with Lazy Room.exe open and edit settings.txt:
- abriviation of your nation,
- path to your WAW folder,
- path to folder with OBJs (or anything if you don't use them)
- path to folder with Sprites (or anything if you don't use them)
- true - to open folder with JSON after it was generated. Or false - to not do that.

5. Download archive with validator from your War Room. Extract it into your WAW folder. Keep each turn in its own folder, named "order_validation_XX_MOVE", where XX is the number of the turn.
E.g.: C:\WAW\order_validation_1_MOVE\

6. Run Lazy Room and see what will happen.

7. In Lazy Room use:
left click and shift left click - to select units or hex,
right click - will open context menu with orders for selected units, in the clicked hex.
ctrl+Z - undo last order,
shift+ctrl+Z - redo order.
F3 - view JSON with orders that will be generated,
F2 - will save JSON to the validator's folder.
To order Scrap: LeftCtrl + LeftAlt + Right click on the unit to scap (on the right side).
F12 - show FPS


To Load unit:
- select units to load,
- right click on a carrier on the right panel.
or
- select units to load,
- right click on a nearby hex with a carrier,
- click Board to load selected units on the first available carrier.
or
- select carrier,
- right click on a nearby hex with units it can load,
- click Load to load all units in the hex that can be loaded.

To unload units:
- select units to unload,
- right click on their carrier on the right panel.
or
- select carrier,
- right click on a nearby hex,
- click Unload to unload all units into that hex.


8. To import images for your units:
- save any image as .png,
- name it EXACTLY as your unit is named in types.csv. You can add "_view" after the name (for BP-bot).
E.g.: URC_Billboard.png, Hornybird_view.png
- put this file in the Sprites folder ( see (4)),
- this image will represent your unit in the unit selection menu.

9. To import models from FtD for your units:
- load your BP,
- delete all planar shields,
- put Origin block to where you want the center of the model to be (recommended: at the bottom of the geometrical center) (or position model in the scene later),
- in V-menu "Create STL file",
- import STL file in Blender (or any other 3d-modeling software of your choosing) and convert it to OBJ format.
- name result EXACTLY as your unit is named in types.csv.
- put OBJ and MTL files with the model in the OBJ folder ( see (4)),
E.g.: URC_Billboard.mtl + URC_Billboard.obj
- this model will represent your unit.

Video:
https://discord.com/channels/441900435138412554/939263164703449238/1004697364575039548

10.
How to build mobile units:
- select hex with production facility you want to use,
- right click on production facility (on the right side) - menu for build order will open.
- set quantity you want to build,
- click button with the name of model to confirm order.

How to build fortifications:
- right click on a hex where you want to build,
- if there are units capable of construction there - menu for build order will open.
- set quantity you want to build,
- click button with the name of model to confirm order.

11. Current limitations, that i can remember: :

- No Payment or Suspend maintenance orders,
- not enough sanity checks. 

- no range checks for amphibious units

- can't select carrier/units while ordering to nearby hex.
- can't use right click on the same hex.
- movement cost of loading/unloading after units have moved may not be accurate. If you think it's wrong - it probably is - press F11 to make it free and do your own math.

