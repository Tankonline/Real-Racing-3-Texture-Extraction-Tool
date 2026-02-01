# 🚗 RR3 Texture Tools

RR3 Texture Tools is a complete toolkit for extracting, converting, editing, and rebuilding **Real Racing 3** textures into universal assets for Android, iOS, and PC.

It provides automated `.z` decompression, format conversion, batch processing, and universal export using industry-standard tools.

---

## ✨ Features

- ✅ Remove `.z` compression (single & batch)
- ✅ Support for DDS, ETC, and PVR formats
- ✅ PNG master workflow for safe editing
- ✅ Universal asset export (Android / iOS / PC)
- ✅ Batch extraction & batch conversion
- ✅ Organized folder structure
- ✅ Beginner-friendly documentation

---

## 📁 Folder Structure

RR3 Texture Tools/
│
├── universal_assets/
│ ├── master_png/
│ ├── android/
│ ├── ios/
│ └── pc/
│
├── Run_tool/
│ ├── run.bat
│ └── batch_extraction.bat
│
├── Tools/
│ ├── AMD Compressor
│ ├── Noesis
│ ├── PVRTexTool
│ └── Python
│
├── Directory.txt
├── README.txt
└── Support.txt


---

## ⚙️ Requirements

- Windows 10 / 11
- Python 3.10+
- Noesis
- AMD Compressonator
- PVRTexTool

All required tools are included in the `Tools` folder.

---

## 🚀 Basic Workflow

### 1️⃣ Remove `.z` Compression

Use:

Run_tool\run.bat


Or for multiple files:

Run_tool\batch_extraction.bat


This removes `.z` compression from files.

---

### 2️⃣ Convert to PNG (Master Asset)

Open extracted files using:

- Noesis
- PVRTexTool
- Compressonator

Export them as PNG.

Save to:

universal_assets\master_png\


⚠️ This is your MASTER file. Never delete it.

---

### 3️⃣ Edit Textures (Optional)

Use Paint.NET or similar editors to:

- Fix colors
- Adjust alpha
- Improve quality

Save again as PNG.

---

### 4️⃣ Universal Export

Run:

Run_tool\universal_export.bat


This automatically creates:

| Platform | Format |
|----------|---------|
| Android  | ETC2 |
| iOS      | ASTC |
| PC       | BC3 |

Files are placed into:

universal_assets\android
universal_assets\ios
universal_assets\pc\


---

## 📦 Universal Asset System

Each texture follows this system:

PNG (Master)
↓
Android (ETC2)
iOS (ASTC)
PC (BC3)


Example:

car_diffuse.png ← Master
car_diffuse_etc2.dds ← Android
car_diffuse_astc.ktx ← iOS
car_diffuse_bc3.dds ← PC


---

## 🧠 Best Practices

✅ Always keep PNG as master  
✅ Never edit compressed files  
✅ Backup original assets  
✅ Match original resolution  
✅ Keep naming consistent  

---

## ⚠️ Legal Notice

- This project is for educational and modding purposes only.
- Original game files are not included.
- You are responsible for complying with game and platform terms.

---

## 📈 Future Plans

- One-click GUI exporter
- Automatic repacking
- Texture preview system
- Cross-platform scripts
- Mod installer support

---

## 🤝 Contributing

Contributions are welcome!

If you improve scripts, automation, or documentation, feel free to submit a pull request.

---

## 📬 Support

See:

Support.txt


Or open an issue on GitHub.

---

## ⭐ Credits

Created by the RR3 modding community.

Special thanks to:
- Noesis
- AMD Compressonator
- PVRTexTool
- Python

---

Enjoy modding! 🚀
