# [Nokia 1] - [frt]

## *Last update (Probably)*
- Due to lack of system partition memory, the phone can be flashed within Android 9 (version 108) and Android 8.1 (Version 27).
- But you can spend your time building newer version for this device and starting tinkering it and finding bugs.

## *Hardware Support (From build 00WW_1_40A and above)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera , Microphone, Bluetooth, USB, Graphics, Storage, Secure boot (Android 8.1), GPS and Screen Brightness.
- What doesn't work or work improperly: Wi-Fi (Android 9), Sensors, GPS, Camera ,Secure boot (Android 9), FM Radio, SIM and Built-in GMS (Android 8.1) and Adaptive brightness.

## Screen Brightness:
- The problem fixed. Still no Adaptive brightness.

## GPS:
- Magically works without any Wi-Fi scan or Mobile data help (This is also true with Android 9 too).

## *Hardware Support (From build 00WW_1_33A and below)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera, Microphone, Bluetooth, USB, Graphics, Storage, Secure boot (Android 8.1) and GPS (Android 8.1), Screen Brightness (Android 9).
- What doesn't work or work improperly: Wi-Fi (Android 9), Sensors, GPS, Camera, Secure boot (Android 9), FM Radio, SIM and Built-in GMS (Android 8.1), Screen Brightness (Android 8.1).

## Screen Brightness:
- In Android 8.1. You'll stuck at 1/2 of the screen brightness. You can change it over terminal.
- Android 9 works fine.

## Storage:
- Due to new ROM rebuild. Nokia made Files app show up into home screen (Except stock ROM).
- Showing Internal Storage is no longer crashing the Files app anymore.

## SIM:
- Solved almost everything in previous vendor/kernel build. (Modem is much more stable like stock ROM and no more crashing and unrecognizing SIM).
- Network bands are now showing up in Testing settings.

## Notes:
- Unlisted categories means they have the same behaviors like previous vendor/kernel builds.

## *Hardware Support (From build 00WW_0_39L and below)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera, Microphone, Bluetooth, USB, Graphics and GPS (Android 8.1 only), Screen Brightness.
- What doesn't work or work improperly (TL;DR): Sensors, GPS (Android 9), Camera, FM Radio, Storage, SIM and Built-in GMS (Android 8.1 builds), Adaptive brightness.

## Screen Brightness
- No adaptive brightness

## Sensors
- Can't detect any thermal sensors (example: battery's temp, battery's voltage).

## GPS (Android 9 only):
- No GPS signal. But does when Wi-Fi and Mobile data supports it.

## Camera
- Theoretically works perfectly.
- Unoptimized Camera2 app (Only behaves like that with version since Android 5.0 redesign). Which leads to low-lighting on both front and back camera. Installing Stock ROM's Camera app might help but it won't save pics.
- Camera app from Android 4.x will fix everything.

## Wi-Fi (Android 9):
-  Tethering doesn't work.

## Storage:
- Files app will crash if you trying to show Internal storage. If you made it crashed constantly. Clean up the app data will do the trick.
- By default, the Files app icon on Launcher will be disabled. Go to Storage settings to explore, or use 3rd party app to launch it.
- Use Google's Files app (Previously Files go), it will show you both Internal and SD card storage without any compromises.

## SIM:
- Only notifies 2nd SIM incoming call. The 1st SIM incoming call will be ignored.
- No USSD messages (Common problem).
- 2G networking and LTE/UTMS (auto PRL) aka 4,3,2G mode will make the phone somehow unrecognize the SIM. (Don't try to switch this network). Try LTE/WCDMA instead in Test settings (Very unstable). Or edit build.prop and add this line "ro.telephony.default_network=12" at first boot or somehow you can access networking menu in Android 9's Test settings. That will make the modem stable (Kinda).
- Supports some of Network bands (Better network bands support in Android 8.1).
- You can't change working Network band in Testing settings.
- For 2nd SIM (Non-mobile data SIM). PLEASE choose 2G network and disable Mobile data for that SIM or the phone modem will be confused and there will be no signal from any SIM (Probably modem software crashing too).
- You cannot make 2nd SIM work like 1st SIM acting as a 4G capable Mobile data SIM (No network on both SIM if you try to do that or Modem crash).
- DO NOT PRE-SET SIM LOCK WHEN YOU PERFORM FIRST BOOT OR YOU'LL GET BOOTLOOPED!

## Secure boot (Android 9):
- If you enter the wrong password in the first place. System will forced you to press Reset Phone button because you entered the wrong password "too much". Reboot the phone and try again.

***
## Notes / Other Bugs
- Booting into Android causes screen went out for a few secs. The phone reboots after first boot.
- The phone is still pre-encrypted anyway (Even if you wiped it with TWRP and Not recommended).
- Builds with Google Play Services crashes a lot. Install OpenGapps with the vanilla builds to fix this.
- Please skip setup wizard because it's buggy and if you wanna setup the phone when it's check for update, press back button and then recheck for updates again. (Probably because of Google Play services "fake allowing SMS permission" and "improper android build").
- If you installed Gapps, please edit the ROM build info. (in /system/etc/prop.default, /system/build.prop, /vendor/default.prop and /vendor/build.prop) or every Google app will yell at you that your phone's software isn't "legit".
- The TWRP recovery formats /data partiton in ext4 format. But the phone partition and encryption only works with f2fs format. So don't try to wipe the phone with TWRP. Only use Stock Android recovery or "fastboot -w" (Only works when bootloader unlocked) can wipe the phone's user data properly.
***

## Tested by:
- Kutiz w/ Nokia 1 (TA-1047 Dual-SIM)


## Tested builds:
- Android 8.1 build v26 w/ Google apps and OpenGapps.
- Android 9.0 build v106 w/ no Google apps and OpenGapps.

_**Last updated:** 3:00 AM; February 10th, 2019_