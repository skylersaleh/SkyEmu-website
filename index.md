
SkyEmu is a low level GameBoy, GameBoy Color and Game Boy Advance emulator. Its primary focus is to provide a good user experience through a good mixture of tradeoffs of accuracy, performance, features and usability.

[<img width="1015" alt="SkyEmu App Screenshot" src="https://user-images.githubusercontent.com/7118296/175430669-20c8079a-bf5c-44b6-b7da-270aca51f216.png">](https://web.skyemu.app/)

# Features

- Highly accurate Game Boy Advanced emulation
- Game Boy and Game Boy Color Emulation 
- Experimental Nintendo DS support (only capable of running homebrew currently)
- Cross Platform: Windows, MacOS, Linux, Web App (with touch screen controls for iOS and Android)
- Game Controller and Rumble Support with configureable keybinds
- 4x Save Slots with screenshot preview
- Game fastforward and rewind support (supporting [very long rewind times](https://www.youtube.com/watch?v=Sfc_1NKbiKg))
- Support for emulating the Real Time Clock
- CPU, MMIO, and Memory Debuggers
- Dark and Light Themes
- Support for loading official BIOS dumps

## Web App Based Build (Desktop/iOS/Android)

The latest version of the emulator can be played at the following address as a progressive web app:

[https://web.skyemu.app/](https://web.skyemu.app/)

On Mobile platforms it is recommended to add to the home screen and launch from there. This will prevent the web browser from auto deleting save files and will remove the browsers UI. 

Nightly native builds can be downloaded at the following links: 

- [Windows](https://nightly.link/skylersaleh/SkyEmu/workflows/deploy_win/main/WindowsRelease.zip)
- [macOS](https://nightly.link/skylersaleh/SkyEmu/workflows/deploy_mac/main/MacOSRelease.zip)
- [Linux](https://nightly.link/skylersaleh/SkyEmu/workflows/deploy_linux/main/LinuxRelease.zip)

Drag and drop a rom in to load it or click on the Load .GB/.GBC/.GBA button to open a menu to select a rom. 

Note: A GBA BIOS is not required as SkyEmu bundles an open source replacement BIOS. However, a dump of an official GBA BIOS should be used if you want to maximize accuracy or you like seeing the GBA intro.
