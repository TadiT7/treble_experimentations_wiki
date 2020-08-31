## Short summary
Tested by @asuvoro on Pixel Experience [Xiaomi Mi A3 - Android Q 10](https://download.pixelexperience.org/laurel_sprout#collapse-0)
All works. Nothing special at this time known.

GSI's not tested maybe or you should fill it in
***
**GSI Installation**

1. adb reboot to bootloader
2. fastboot devices
3. fastbooot getvar current-slot (CHECK FOR ACTIVE SLOT)
4. fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img (USE VBMETA.img FROM STOCK ROM OF MI A3)
5. fastboot erase system
6. fastboot flash system name-of-gsi.img
7. (WHILE HOLDING VOLUME+ KEY) fastboot reboot
8. In stock recovery , you should see NO COMMAND.
   Now , while holding POWER key press VOLUME+ key and you should see Recovery commands > Choose Wipe data/Factory reset > Reboot to system.

**System should BOOT now.**
***
Tested GSI images -
1. AOSP v222 by Phh - Vanilla & Gapps
2. [microG ufOfficial](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/aosp-10-0r40-microg-ufofficial-cve-aug-t4147899)
***
