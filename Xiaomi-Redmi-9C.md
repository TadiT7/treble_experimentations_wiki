# Xiaomi Redmi 9C (angelica)

# Requirements
*Stock Recovery
*[vbmeta.img](https://forum.xda-developers.com/attachments/vbmeta-img.5257631/)
*PC with ADB/fastboot drivers installed
*Coffee

## How to flash a GSI image?

Firstly, choose a GSI image you want to install according to the Android version and the architecture of our device. Redmi 9C uses a64 ab variant (arm32 binder 64 ab) so please make sure you picked the right one. After that, you should extract it to your desired location, then move it to the ADB location and rename the image file as 'system.img'.

Then plug it into your PC and then execute these codes in the command prompt.
```
fastboot devices
fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img
fastboot reboot fastboot
```
Now, your Redmi 9C must boot in yellow fastboot mode (fastbootd). After that, do these steps onward.
```
fastboot getvar is-userspace
fastboot erase system
fastboot flash system system.img
fastboot reboot recovery
```
Voila! You have successfully managed to flash a GSI ROM to your Redmi 9C device! But wait, once it boots into stock recovery, don't forget to wipe or format the data after flashing the GSI image.

### Working GSI builds 

* Tested [CrDroid v313 by eremitein](https://sourceforge.net/projects/treblerom/files/crDRom11/2021.09.21/)
* Tested [Bless v306 by eremitein](https://sourceforge.net/projects/treblerom/files/BLESS11/2021.05.02/)
* Tested [Pixel Experience 10 by ExpressLuke](https://sourceforge.net/projects/expressluke-gsis/files/PixelExperience/Ten/ARM64/AB/)
* Every [eremitein](https://sourceforge.net/projects/treblerom/files/) builds

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √ |
| Audio                     | √× (headphone jack doesn't work, but can be fixed with a simple code on termux) |
| Bluetooth                 | √ |
| Display                   | √ (brightness slider doesn't work) |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √ |
| VoLTE                     | ? (Untested) |
| Fingerprint               | √ |
| Offline Charging          | × |

## Fixes

To fix the earphone issue, execute these lines on any Terminal Emulator then reboot.
```
su
setprop persist.sys.overlay.devinputjack true
```

### Credits
* [Redmi 9C | Angelica Indonesia](https://t.me/Redmi9CID) 
* [Brahm Daniel Verano](https://github.com/liafourte)