## Short summary
Tested by @e5u on MIUI 12.5.5 (Android 10)

Bugs: FOD only works above 70% brightness and aliasing around the screen.

GSI's not tested maybe or you should fill it in
***
# **GSI Installation :-**

_**DO NOT JUST COPY & PASTE COMMANDS , SHOULD HAVE KNOWLEDGE PRIOR TO FIDDLING WITH DEVICE.**_

1. adb reboot to bootloader
2. fastboot devices
4. fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img (USE VBMETA.img FROM STOCK ROM OF MI CC 9E)
5. fastboot erase system
6. fastboot flash system name-of-gsi.img
7. fastboot format metadata
8. fastboot fotmat userdata
9. fastboot reboot

# **Another way
Flash system.img via TWRP and wipe data

**System should BOOT now.**

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | work                                                    |
| Speaker / Mic             | work                                                    |
| Bluetooth                 | work                                                    |
| WiFi                      | work                                                    |
| SIM / Mobile Data / Voice | work                                                    |
| VoLTE                     | work                                                    |
| Fingerprint               | bug                                                    |                     
| Offline Charging          | work                                                    |                                  
---

***
Tested GSI images -
1. AOSP 12.0 v402 by phh
2. Pixel Experience 12.0 v402.1 by ponces
***
