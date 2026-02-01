=================================================
        RR3 TEXTURE TOOLS – USER GUIDE
=================================================

This toolkit allows you to extract, edit, and
recompress Real Racing 3 texture files.

It supports both:

• Single-file extraction
• Batch folder extraction


-------------------------------------------------
SUPPORTED FILE TYPES
-------------------------------------------------

The tool works with compressed files such as:

- .dds.z
- .etc.dds.z
- .pvr.z
- .ptc.pvr.z
- .rgb.pvr.z
- Other zlib-compressed formats


-------------------------------------------------
REQUIREMENTS
-------------------------------------------------

1) Windows PC
2) Python 3.x or newer
3) RR3 Texture Tools package

Make sure Python is installed before use.


-------------------------------------------------
FOLDER STRUCTURE
-------------------------------------------------

RR3 Texture tools
│
├── Run_tool
│   ├── run.bat              (Single file tool)
│   └── batch_extract.bat    (Batch tool)
│
├── Tools
│   └── Zlib
│       └── Universal.py     (Extractor engine)
│
├── Original files           (Store .z files here)
├── extracted_dds
├── png_edit
├── output_dds
└── output_z


-------------------------------------------------
SINGLE FILE EXTRACTION
-------------------------------------------------

Use this mode to extract one file at a time.

1) Place your .z file anywhere inside
   "RR3 Texture tools"

2) Open:
   Run_tool → run.bat

3) Type ONLY the file name

   Example:
   sprites_0.etc.dds.z

4) Press ENTER

5) The extracted file will be saved
   next to the original file


-------------------------------------------------
BATCH EXTRACTION (FOLDER MODE)
-------------------------------------------------

Use this mode to extract many files at once.

1) Place all .z files inside a folder

   Example:
   C:\RR3_Dump\Textures

2) Open:
   Run_tool → batch_extract.bat

3) Paste the FULL folder path

   Example:
   C:\RR3_Dump\Textures

4) Press ENTER

5) The tool will:

   - Scan the folder
   - Find all .z files
   - Extract them
   - Create an "extracted" folder
   - Save all output inside it


Example result:

Textures\
   ui.z
   menu.z
   cars.z
   extracted\
      ui
      menu
      cars


-------------------------------------------------
OPENING EXTRACTED FILES
-------------------------------------------------

After extraction, use these tools:

• Noesis – Preview and export
• PVRTexTool – PVR textures
• Paint.NET – PNG editing
• Compressonator – ETC/DDS encoding


Recommended workflow:

.z → Extract → DDS/PVR → PNG → Edit → Recompress


-------------------------------------------------
BACKUP SYSTEM
-------------------------------------------------

If an output file already exists, the tool
automatically creates a backup:

filename.dds → filename.dds.bak

This prevents data loss.


-------------------------------------------------
PERFORMANCE & LIMITS
-------------------------------------------------

• No file limit (practically unlimited)
• Files processed one at a time
• Stable for large batches

Limits depend on:

- Disk space
- File size
- System speed


-------------------------------------------------
TROUBLESHOOTING
-------------------------------------------------

If file is not found:
- Check spelling
- Check extension
- Make sure file is inside project folder

If Python errors appear:
- Reinstall Python
- Enable "Add to PATH"

If output is broken:
- File may be corrupted
- Try another tool
- Re-extract game data


-------------------------------------------------
ADVANCED USERS
-------------------------------------------------

Universal.py supports:

python Universal.py input.z
python Universal.py input.z output_folder

You may customise the script for special formats.
Use ChatGPT for assistance.


-------------------------------------------------
BEST PRACTICES
-------------------------------------------------

✔ Always keep backups
✔ Work on copies
✔ Test small batches first
✔ Keep filenames unique
✔ Organise folders


-------------------------------------------------
DISCLAIMER
-------------------------------------------------

This toolkit is for educational and
modding purposes only.

Use responsibly.

=================================================
