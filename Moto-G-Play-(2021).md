# Moto G Power (2021) - codename "guamna"

## Installing the GSI
**NOTE: this will remove all your data!**
**Make sure you do not set a pin on your device before flashing any of the GSI files! This will make it impossible to pass the initial device setup.**
**Your Mileage May Vary! I am not responsible for anything that happens when you follow these steps.** 

- Unlock your bootloader (there are many tutorials on how to do this)
- Go into fastbootd (`adb reboot fastboot`, or from recovery `fastboot reboot fastboot`)
- Download vbmeta.img from Google: https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img
- Flash vbmeta.img (`fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`)
- Then flash your system.img (`fastboot flash system <your downloaded system img>.img`)
- Use the volume and power buttons on your phone to navigate to the "Enter system recovery" (or something similar) section
- Navigate to "erase all data (factory reset)" (or something similar) and confirm
- Navigate to "reboot to system" (or something similar
- This should now boot you into a working GSI :)

## Fixing common issues
Read the [Common Issues section of the wiki](https://github.com/phhusson/treble_experimentations/wiki/Common-Issues-and-fixes) to fix common issues like bluetooth, fingerprint reader not working, wired headphones not working

## Features I have not tested
- Sim card (mobile data, calling)

## Further Info
- Tested by @franciskafieh on Aug. 5th, 2022
- Tested both secure-gapps and normal gapps variants (AOSP 12.1 v414)
- Tested on XT2093-4
