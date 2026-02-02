# 🏎️ Real Racing 3 Texture Tools

A complete toolkit for extracting, editing, converting, and repacking Real Racing 3 texture assets.

This toolset allows you to go from original `.z` game files → editable `.png` → game-ready assets → back into the game.

---

## ✨ Features

- Extract `.z` texture files
- Convert DDS ↔ PNG for editing
- Export universal assets (Android & PC)
- Repack textures into `.z` format
- Batch processing support
- Automatic folder organisation
- Built-in Compressonator, Noesis, and Zlib tools

---

## 📁 Folder Structure

See `Directory.txt` for the full file layout.

Important folders:

- `Run_tool/` → All main batch tools  
- `PNG_Universal/` → Put edited PNG files here  
- `Converted to .z assets/` → Final game-ready files  
- `output_dds/` → Temporary DDS output  
- `extracted_dds/` → Extracted textures  
- `universal_assets/` → Platform-specific exports  

---

## 🚀 Quick Start

### 1️⃣ Extract Game Textures
Run:

```bat
Run_tool\run.bat
```

or

```bat
Run_tool\batch_extraction.bat
```

This extracts `.z` files into readable formats.

---

### 2️⃣ Convert DDS to PNG (For Editing)

```bat
Run_tool\dds_to_png.bat
```

Edit the PNG files using any image editor.

---

### 3️⃣ Export Universal Assets

Put your edited PNG files into:

```
Run_tool\PNG_Universal\
```

Then run:

```bat
Run_tool\export_universal.bat
```

This creates:
- Android (ETC2)
- PC (BC3)

versions.

---

### 4️⃣ Convert PNG Back to Game-Ready `.z`

After editing, run:

```bat
Run_tool\png_to_game_ready.bat
```

This converts:

PNG → DDS → ZLIB (.z)

Final files appear in:

```
Converted to .z assets\
```

These can be placed back into the game.

---

## 🛠️ Main Batch Tools

| File | Purpose |
|------|----------|
| `run.bat` | Extract single `.z` file |
| `batch_extraction.bat` | Extract multiple `.z` files |
| `dds_to_png.bat` | Convert DDS → PNG |
| `export_universal.bat` | Create Android & PC assets |
| `png_to_game_ready.bat` | Repack PNG → `.z` |

---

## ⚠️ Important Notes

- Always back up original game files
- Use matching filenames when replacing assets
- Incorrect formats may cause crashes
- Android and PC formats are supported
- iOS support is limited

---

## 📦 Requirements

- Windows 10/11
- Python 3+
- Compressonator CLI (Included)
- Noesis (Included)

All required tools are bundled in the `Tools` folder.

---

## ❓ Troubleshooting

If something does not work:

- Check file paths
- Make sure tools are installed correctly
- Run `.bat` files as Administrator
- See `Support.txt` for help

---

## 📜 Disclaimer

This project is for educational and modding purposes only.

You are responsible for how you use these tools.

---

## ⭐ Credits

- AMD Compressonator
- Noesis Tools
- PVRTexTool
- Python Zlib

Developed for the RR3 modding community.
