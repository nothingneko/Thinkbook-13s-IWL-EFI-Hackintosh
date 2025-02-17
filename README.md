# I HAVE MADE MAJOR CHANGES TO THE CONFIGURATION, I WILL UPLOAD THE UPDATES SOON

# Hackintosh EFI for First Generation Lenovo ThinkBooks
Thanks for checking out my EFI! I hope it'll be helpful to you too. Before you get started, do your research! Is your configuration compatible with this EFI? Use the [official guide](https://dortania.github.io/OpenCore-Install-Guide/) to familiarize yourself with the process. If you have questions or comments please feel free to file an issue! Pull requests are always accepted too!

### macOS Version:
- macOS Monterey

### OpenCore Version: 
- ?

### Compatible ThinkBooks:
- Thinkbook 13s IWL (Designed for)
- Thinkbook 14s IWL (Quite possibly will work, upstream reports it does)

### My Hardware Configuration
| Hardware | Info |
| ------ | ------ |
| CPU | Intel(R) Core(TM) i5-8265U CPU @ 1.80GHz |
| MEMORY | 8 GiB DDR4 |
| GRAPHICS | Intel UHD Graphics 620 |
| DISK | Western Digital Blue SN570 250GiB |
| SOUND | Intel Cannon Point-LP High Definition Audio Controller |
| Network | Intel Cannon Point-LP CNVi |

### Hardware Status
| Name | Comment |
| ------ | ------ |
| Graphics Acceleration |Working fully|
| Trackpad |Working, Force Touch must be turned off|
| Keyboard |Working fully, Super is recognized as Cmd|
| Internal Speaker |Working fully|
| Internal Microphone |Working fully|
| Headphone jack |Full quality audio|
| USB Type-A |Working fully|
| USB Type-C |Working for Audio and Video|
| Camera |Working fully|
| Battery |Working, mildly degraded life|
| Brightness |Changeable in software and with hardware keys|
| Wi-Fi |Works with performance relative to Linux IWLWiFi|
| Bluetooth | Does not work in Monterey |
| HDMI |Working fully|

### Known Issues
| Name | Comment |
| ------ | ------ |
| Sleep | Closing the Lid will not trigger sleep, and leaving the lid open during manual sleep causes issues. Additionally the timed Turn Off Display option may cause issues - Working on Fixes |
| Fingerprint |Doesn't work on Linux either, there is a effort for Linux drivers though.|


## Installation Instructions for Linux
### Pre-requisites
- [GNOME Disk Utility](https://apps.gnome.org/app/org.gnome.DiskUtility/)
- A file manager (Anything works)
- [balenaEtcher](https://etcher.io)

### Instructions

1. Download the [Olarila image](https://www.olarila.com/topic/6278-hackintosh-and-macintosh-olarila-vanilla-images-macos/)

Note: Olarila is generally hated in the community, don't use the forum or provided EFI, it's just a means to an end for a full installer image.

2. Clone this repo (Use this command: `git clone https://github.com/jadeastar/Thinkbook-13s-IWL-EFI-Hackintosh.git`)
2. Flash the image to a removable drive using Etcher (I've only tested Etcher, so play it safe and use it)
3. After the drive is flashed, mount the EFI partition with GNOME Disks
4. Remove the EFI folder and replace it with the EFI folder from this repo
5. Use GenSMBIOS to generate a new SMBIOS for your install (I recommend MacBookPro15,1)
6. Boot from the drive and install macOS
7. Copy the EFI from the installer to the internal disk
8. Profit



## Useful Links
[GenSMBIOS]: <https://github.com/corpnewt/GenSMBIOS>
[ProperTree]: <https://github.com/corpnewt/ProperTree> 
[OpenCore Install Guide]: <https://dortania.github.io/OpenCore-Install-Guide/>
[OpenIntelWireless]: <https://github.com/OpenIntelWireless>
[Acidanthera]: <https://github.com/acidanthera>
[VoodooI2C]: <https://github.com/VoodooI2C/VoodooI2C>
[ECEnabler]: <https://github.com/1Revenger1/ECEnabler>
[ws839750375]: <https://github.com/ws839750375>
