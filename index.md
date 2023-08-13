![SkyEmu](https://github.com/skylersaleh/SkyEmu-website/assets/7118296/9f1da564-8d08-40f1-a483-bf6a36e70ea1)

SkyEmu is a low level GameBoy, GameBoy Color, Game Boy Advance, and Nintendo DS emulator whose primary focus is to provide a good user experience through a good mixture of tradeoffs of accuracy, performance, features and usability.

# Features

- [Highly accurate Game Boy Advance emulation](docs/Accuracy.md)
- Game Boy and Game Boy Color Emulation
- Nintendo DS Emulation (Beta Quality)
- High Quality Upscaling Shaders, Color Correction, and Screen Ghosting
- Cross Platform: Windows, MacOS, Linux, FreeBSD, iOS, Android, and Web
- Game Controller and Rumble Support with configureable keybinds
- 4x Persistent Save State Slots with screenshot preview
- Game fastforward and rewind support (supporting [very long rewind times](https://www.youtube.com/watch?v=Sfc_1NKbiKg))
- Action Replay Cheat Code Engine 
- Localization in Armenian, Chinese, Danish, Dutch, English, German, Greek, Italian, and Russian
- Support for emulating the Real Time Clock and Solar Sensor
- CPU, MMIO, and Memory Debuggers
- Support for loading official BIOS and Boot ROM dumps
- Support for loading roms compressed in .zip archives
- [REST-like API for asynchronous scripting and other automation](docs/HTTP_CONTROL_SERVER.md)

## Download / Usage

Native builds can be downloaded at: https://github.com/skylersaleh/SkyEmu/releases

The latest version of the emulator can also be played without installing at the following address as a progressive web app:

https://web.skyemu.app/

On Mobile platforms it is recommended to add this to the home screen and launch from there. This will prevent the web browser from auto deleting save files and will make the app full screen. 

Note: Platform BIOS/Firmware files are not required as SkyEmu bundles open source replacement BIOS/stubs. However, it is strongly recommended to dump official BIOS/firmware as the open source replacements lack many of the features of the native firmware/BIOS (such as colorizing GB games and the startup splashes) and are not as accurate. 

## Discord Server

<a href="https://discord.gg/tnUEtmJgA5" rel="Join Discord Server">![Discord Banner 2](https://discordapp.com/api/guilds/1131322341645893783/widget.png?style=banner2)</a>

## Default Controls:

- WASD: D-Pad
- J: A button
- K: B button
- ': Select button
- Enter: Start button
- U: L shoulder
- I: R shoulder

On mobile platforms an onscreen touch screen controller is provided. 

## Loading save files and BIOSs

On web builds save files and the BIOS can be loaded by dragging them onto the page or loading them using the ROM file picker. The GBA BIOS must be named `gba_bios.bin` for the emulator to pick it up. Save files must be named the name of the rom file with the extension `.sav`. So for example if the ROM was `MyRomFile.gba` the save file must be called `MyRomFile.sav`. 

On native builds the above naming convention still applies, but the save/BIOS files must be instead located in the same folder as the ROM file, instead of being dragged or loaded in the emulator itself.

## Native Build Instructions

Native builds are experimental currently but can be built using the following commands:

```
mkdir build
cd build
cmake .. 
cmake --build . 
```

The output binaries should be in the build/bin folder

Native builds support loading roms through the command line by specifying the path to the ROM as the first argument: 

```
./SkyEmu path/to/rom.gba
```
