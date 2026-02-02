Real Racing 3 Texture Tools
==========================

Version: Latest
Author: Community Modding Toolkit

----------------------------------
Overview
----------------------------------

This toolkit allows you to extract, edit, convert, and repack
Real Racing 3 texture files.

You can:
- Extract .z files
- Convert textures to PNG
- Edit textures
- Export universal assets
- Rebuild game-ready files

All major actions are handled using automated .bat files.


----------------------------------
Requirements
----------------------------------

- Windows 10/11
- Python 3.x
- Compressonator CLI
- PVRTexTool CLI
- Noesis (included)


----------------------------------
Main Tools
----------------------------------

run.bat
→ Extracts .z files

batch_extraction.bat
→ Extracts multiple .z files

export_universal.bat
→ Converts PNG to Android/PC formats

png_to_game_ready.bat
→ Converts PNG → DDS → ZLIB (.z)


----------------------------------
Basic Workflow
----------------------------------

1. Extract Game Files
   - Use run.bat or batch_extraction.bat

2. Convert to PNG
   - Use Noesis or PVR tools

3. Edit PNG
   - Use any image editor

4. Universal Export (Optional)
   - Use export_universal.bat

5. Repack for Game
   - Use png_to_game_ready.bat

6. Replace in Game Folder


----------------------------------
Folders
----------------------------------

PNG_Universal
→ Put edited PNG files here

Converted to .z assets
→ Final game-ready files

universal_assets
→ Android and PC formats

output_dds
→ Temporary DDS files


----------------------------------
Important Notice
----------------------------------

Always back up original RR3 files
before replacing any assets.

You use this tool at your own risk.


----------------------------------
Credits
----------------------------------

- AMD Compressonator
- Noesis
- PowerVR Tools
- Zlib
- Community Contributors
