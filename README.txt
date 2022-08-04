How to use Lazy Room to generate JSONs with orders:

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

8. To import images for your units:
- save any image as .png,
- name it EXACTLY as your unit is named in types.csv. You can add "_view" after the name (for BP-bot).
E.g.: URC_Billboard.png, Hornybird_view.png
- put this file in the Sprites folder ( see (4)),
- this image will represent your unit in the unit selection menu.

9. To import models from FtD for your units:
- load your BP,
- delete all planar shields,
- put Origin block to where you want the center of the model to be (recommended: at the bottom of the geometrical center),
- in V-menu "Create STL file",
- import STL file in Blender (or any other 3d-modeling software of your choosing) and convert it to OBJ format.
- name result EXACTLY as your unit is named in types.csv.
- put OBJ and MTL files with the model in the OBJ folder ( see (4)),
E.g.: URC_Billboard.mtl + URC_Billboard.obj
- this model will represent your unit.

10.
Current limitations, that i can remember: 
- no support whatsoever for carriers,
- no range checks for amphibious units,
- Evade order will ignore its settings and will generate "Evade everything".

Incoming in the next version:
- carriers,
- icons on units for moves that were ordered,
- full support for Evade.