# Asus Zenfone Max Pro M2
![](https://www.asus.com/media/global/products/JnIzW5AoKK3JccyH/P_setting_fff_1_90_end_600.png)

## Hardware Support

* Camera
> Working, read below to see how to get it working.

* Fingerprint
> Working

* Wi-Fi
> Working

* SIM/Calling
> Working
 
* Mobile data
> Working

* Speaker/Microphone
> Working

* Flashlight
> Working

To use camera, you'll need to enable following settings in Phh Treble Settings:
* Qualcomm Settings > Use Alternative Camera Profile
* Misc Features > Expose Aux Camera & Force enable Camera2API

Reboot after toggling these settings

## Bugs

None yet.

## Requirements

* [TWRP](https://dl.twrp.me/X01BD/) or any other custom recovery
* Any custom rom that supports treble (In this case I used [LineageOS 18.1](https://download.lineageos.org/X01BD) for testing.)
* Arm64 AB Image

## Installation

* Boot into TWRP and flash the rom
* Wipe Cache, Data and System
* Flash the image as System Image
* Reboot

## Tested GSIs

* [phh AOSP](https://github.com/phhusson/treble_experimentations/releases)
* [CAOS](https://sourceforge.net/projects/treblerom/files/CAOS/)
* [Corvus](https://forum.xda-developers.com/t/gsi-alpha-11-phh-corvusos-v13-0-exalted.4212765/)
* [LineageOS](https://sourceforge.net/projects/andyyan-gsi/files)

Booted:
✓ Phh AOSP v313
✓ Phh AOSP v400.c 
✓ CAOS v315
✓ LineageOS 18.1
✓ LineageOS 19.0
✓ ...and many more

##
Tested by @asrieldashie | Feb 16 2021 | Edited on Jan 30 2022

##