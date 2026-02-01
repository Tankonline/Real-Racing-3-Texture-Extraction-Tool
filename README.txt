=================================================
RR3 TEXTURE TOOLS – USER GUIDE
=================================================

Author: RETR0
Project: RR3 Texture Tools

Purpose:
This toolset allows you to extract, edit, convert,
and repack Real Racing 3 texture assets into
game-ready .z files.


-------------------------------------------------
REQUIREMENTS
-------------------------------------------------

Before using this tool, make sure these are installed:

✔ AMD Compressonator CLI
✔ Noesis
✔ PVRTexTool CLI
✔ Python 3
✔ Zlib Scripts

All tools must be placed in the Tools folder.


-------------------------------------------------
BASIC WORKFLOW
-------------------------------------------------

This tool follows a simple pipeline:

1) Extract → 2) Convert → 3) Edit → 4) Rebuild → 5) Install


-------------------------------------------------
STEP 1 – EXTRACT GAME FILES
-------------------------------------------------

Place original .z files in:

Run_tool/

Run:

run.bat

This removes zlib compression.


-------------------------------------------------
STEP 2 – CONVERT TO PNG
-------------------------------------------------

Open extracted files using:

- Noesis
- PVRTexTool

Export them as PNG.

Save them into:

Run_tool/PNG_Universal/


-------------------------------------------------
STEP 3 – EDIT TEXTURES
-------------------------------------------------

Edit PNG files using:

- Paint.NET
- GIMP
- Photoshop

Rules:

✔ Do NOT resize
✔ Do NOT rename
✔ Keep alpha channel
✔ Keep same format


-------------------------------------------------
STEP 4 – EXPORT UNIVERSAL ASSETS (OPTIONAL)
-------------------------------------------------

Run:

export_universal.bat

This creates:

- Android textures
- PC textures

Used for testing and previewing.


-------------------------------------------------
STEP 5 – BUILD GAME FILES
-------------------------------------------------

Run:

png_to_game_ready.bat

This converts:

PNG → DDS → ZLIB

Final files are placed in:

Converted to .z assets/


-------------------------------------------------
STEP 6 – INSTALL MOD
-------------------------------------------------

Copy the generated .z files back into
the Real Racing 3 game directory.

Replace the original files.


-------------------------------------------------
BATCH FILES
-------------------------------------------------

run.bat
 → Extracts .z files

batch_extraction.bat
 → Batch extractor

export_universal.bat
 → Platform exports

png_to_game_ready.bat
 → Creates game-ready files


-------------------------------------------------
USING PYTHON SCRIPTS
-------------------------------------------------

Manual usage (advanced):

Unpack:
python Universal.py file.z

Pack:
python pack_zlib.py file.dds


-------------------------------------------------
COMMON ERRORS
-------------------------------------------------

"File not found"
 → Wrong folder

"No valid zlib blocks"
 → Already unpacked

"Invalid format"
 → Wrong codec

"CLI not found"
 → Tool missing

"No output"
 → No PNG files found


-------------------------------------------------
BEST PRACTICES
-------------------------------------------------

✔ Always back up original files
✔ Work on copies only
✔ Test offline
✔ Keep naming identical
✔ Verify sizes


-------------------------------------------------
LEGAL NOTICE
-------------------------------------------------

For educational and personal modding only.

You are responsible for how this tool is used.

Do not use for cheating or online abuse.


-------------------------------------------------
CREDITS
-------------------------------------------------

AMD Compressonator
Noesis
PowerVR Tools
Python
ChatGPT


-------------------------------------------------
END OF README
-------------------------------------------------
