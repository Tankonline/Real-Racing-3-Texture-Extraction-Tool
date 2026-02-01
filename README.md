# RR3 Texture Tools

An all-in-one toolkit for extracting, editing, converting, and repacking Real Racing 3 texture assets.

This tool allows you to:
- Extract `.z` compressed assets
- Convert textures to PNG
- Edit textures
- Rebuild game-ready files
- Export universal assets for Android and PC

Designed for Windows users.


---

## Features

✔ Extract `.z` compressed game files  
✔ Convert DDS / PVR textures to PNG  
✔ Edit textures easily  
✔ Repack PNG → DDS → ZLIB  
✔ Generate Android & PC universal assets  
✔ Batch processing support  
✔ Automated tools using `.bat` scripts  


---

## Supported Platforms

| Platform | Status |
|----------|---------|
| Android  | Supported (ETC2) |
| PC       | Supported (BC3) |
| iOS      | Experimental / Limited |


iOS uses PVRTC/PVR formats and may require manual conversion.


---

## Folder Overview

See `Directory.txt` for the full project structure.

Main working folders:

- `Run_tool/` → All main batch files
- `PNG_Universal/` → Put editable PNG files here
- `Converted to .z assets/` → Final game-ready files
- `Tools/` → Required third-party software
- `universal_assets/` → Exported platform textures


---

## Requirements

Before using this tool, make sure you have:

- Windows 10 / 11
- Python 3.10+
- AMD Compressonator CLI
- Noesis
- PVRTexTool CLI (optional, for iOS)


All required tools should be placed inside the `Tools/` folder.


---

## Setup

1. Download or clone this repository
2. Extract to any folder
3. Verify tools are inside `Tools/`
4. Install Python (enable "Add to PATH")
5. Open CMD in project folder
6. Test with one file first


---

## Usage Guide

### 1. Extract Game Files

Use:

Run_tool\run.bat


or

Run_tool\batch_extraction.bat


This removes `.z` compression.


---

### 2. Convert to PNG

Use Noesis or PVRTexTool to export extracted files to PNG.

Place edited PNG files into:

Run_tool\PNG_Universal\



---

### 3. Export Universal Assets

Run:

Run_tool\export_universal.bat


This creates:

- Android → ETC2
- PC → BC3

Output goes to:

universal_assets\



---

### 4. Convert PNG to Game-Ready Files

Run:

Run_tool\png_to_game_ready.bat


This converts:

PNG → DDS → ZLIB

Final files appear in:

Converted to .z assets\



---

### 5. Replace in Game Files

1. Back up original files
2. Replace `.z` files with new ones
3. Keep original filenames
4. Test offline first


---

## Batch Processing

To extract multiple files:

Run_tool\batch_extraction.bat


To convert multiple PNG files:

Run_tool\export_universal.bat
Run_tool\png_to_game_ready.bat



---

## File Rules

Important:

✔ Do NOT change resolutions  
✔ Keep original names  
✔ Preserve alpha channels  
✔ Do not resize textures  
✔ Always keep backups  


Wrong formats may cause crashes.


---

## Troubleshooting

See:

- `Support.txt`
- `README.txt`
- `Directory.txt`

Common fixes:

- Check tool paths
- Verify Python installation
- Confirm PNG folder location
- Use original `.z` files only


---

## Limitations

- iOS support is limited
- Some formats are device-specific
- Not all textures are editable
- Encrypted files cannot be extracted


---

## Compatibility

Tested On:

✔ Windows 10  
✔ Windows 11  

Not Supported:

✘ Linux  
✘ macOS  


---

## Legal Disclaimer

This project is for educational and modding purposes only.

All game assets belong to their respective owners.

Use at your own risk.


---

## Credits

- AMD Compressonator
- Noesis
- PowerVR Tools
- Python
- Open Source Community


---

## Author

Created by **RETR0**

If you use this project, please credit the author.
