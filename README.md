Switch NSP Forwarder Builder — by The Other Side

A Windows GUI application to create NSP forwarders for:

Nintendo Switch with firmware 21.1.0 support

Standard Homebrew NROs

RetroArch ROM Forwarders

This tool builds fully functional NSPs that appear on the Nintendo Switch HOME menu and launch directly into:

Any .nro homebrew

RetroArch core + ROM

📥 Requirements

Windows 10/11

Python 3.10+ (only if running .py instead of .exe)

prod.keys (place inside /tools)

hacbrewpack.exe (included)

📂 Folder Structure

Your project folder must contain:

switch_forwarder_gui.exe
/tools
    hacbrewpack.exe
    prod.keys <---- (you have to add this)
    /template_forwarder
/output
/work

🚀 How to Use
STANDARD NRO FORWARDER

Open the program

Select Standard NRO Forwarder tab

Enter Title Name

Generate or enter Title ID

Enter sdmc path for the .nro
Example:

/switch/myapp/myapp.nro


Choose an icon (drag/drop or browse)

Click Build Forwarder NSP

Output goes to /output

RETROARCH ROM FORWARDER

Open RetroArch Forwarder tab

Enter Title and Title ID

Enter Core NRO path, example:

/retroarch/cores/snes9x_libretro_libnx.nro


Enter ROM path, example:

/roms/snes/Donkey Kong Country 2.sfc


Add icon

Build NSP

Install on Switch

🎮 Supported
✔ Any RetroArch Core

All .nro cores work

✔ Any ROM type

Examples:

.sfc, .smc, .gba, .zip, .nes, .md, .cue/.bin, .z64, .v64 ...

✔ Any ROM folder
/roms/
/retroarch/downloads/
/games/
/media/
/anything/

🛠 Build EXE (Developer)

Use:

pyinstaller --noconfirm --onefile --windowed switch_forwarder_gui.py
