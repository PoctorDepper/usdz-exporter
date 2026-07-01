# USDZ Exporter
This repository contains the source code for the USDZ exporter used in 
[Kintsugi3DBuilder](https://github.com/michaelt919/Kintsugi3DBuilder/). This requires being compiled into applications and
dropped into an included folder for the Kintsugi3DBuilder exports and is consequently
required by the builder to export into USDZ file formats.

## Prerequisites
- Python3 (3.13 is used during testing, >3.9 is required)
- PyInstaller (if building executable)

## Build Instructions
If you're looking to make an executable, simply run:
```bash
pyinstaller scripts/converter.py --collect-all pxr -y --onefile
```
and the executable will be located in `dist/`