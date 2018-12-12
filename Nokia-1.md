# [Nokia 1] - [frt]

## *Hardware Support (For vendor from build 00WW_1_40A)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera (Explain below), Microphone, Bluetooth, USB, Graphics, Storage, Secure boot (Android 8.1) and GPS (Android 8.1), Screen Brightness.
- What doesn't work or work improperly: Wi-Fi (Android 9), Sensors, GPS, Camera (Explain below),Secure boot (Android 9), FM Radio, SIM and Built-in GMS (Android 8.1).

## Screen Brightness:
- The problem fixed. Still no Adaptive brightness.

## *Hardware Support (For vendor from build 00WW_1_33A)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera (Explain below), Microphone, Bluetooth, USB, Graphics, Storage, Secure boot (Android 8.1) and GPS (Android 8.1), Screen Brightness (Android 9).
- What doesn't work or work improperly: Wi-Fi (Android 9), Sensors, GPS, Camera (Explain below),Secure boot (Android 9), FM Radio, SIM and Built-in GMS (Android 8.1), Screen Brightness (Android 8.1).

## Screen Brightness:
- In Android 8.1. You'll stuck at 1/2 of the screen brightness. You can change it over terminal.
- Android 9 works fine.

## Storage:
- Due to new ROM rebuild. Nokia made Files app show up into home screen (Except stock ROM).
- Showing Internal Storage no longer crashing the Files app anymore.

## SIM:
- No more SIM unrecognizing, Modem crashing. (You can choose 2G network or 2G only working along side with 4G aka LTE/UMTS (auto PRL)).
- Network bands are now can be selected in Testing settings. (star pound star pound 4636 pound star pound star)
- You cannot make 2nd SIM work like 1st SIM acting as 4G capable Mobile data SIM like version 00WW_0_* one. Both SIM will have no signal.

## Notes:
- Unlisted categories means they have behaviors the same with the previous vendor build.

## *Hardware Support (For vendor from build 00WW_0_)*

## TL;DR
- What works flawlessly: Wi-Fi (Android 8.1), Sensors (Except internal thermal sensors), Flashlight, Speaker, Camera (Explain below), Microphone, Bluetooth, USB, Graphics and GPS (Android 8.1 only), Screen Brightness.
- What doesn't work or work improperly (TL;DR): Sensors, GPS (Android 9), Camera (Explain below), FM Radio, Storage, SIM and Built-in GMS (Android 8.1), Screen Brightness.

## Screen Brightness
- No adaptive brightness

## Sensors
- Can't detect any thermal sensors (example: battery's temp, battery's voltage).

## GPS (Android 9 only):
- No GPS signal, but does when have Wi-Fi and Mobile data connection around.

## Camera
- Theoretically works perfectly.
- Unoptimized Camera app. Which leads to low-lighting on both front and back camera. Installing Stock ROM's Camera app might help but won't save pics.
- Camera app from Android 4.x will fix everything (Not Gallery app from MediaTek, Must be Stock Google Gallery or Camera ones).

## Wi-Fi (Android 9):
-  Tethering doesn't work.

## Storage:
- Files app will crash if you trying to show Internal storage. If you made it crashed constantly. Clean up the app data will do the trick.
- By default, the Files app icon on Launcher will be disabled. Go to Storage settings to explore.
- Use Google's Files app (Previously Files go). It will show you both Internal and SD card storage without any compromises.

## SIM:
- Only notifies 2nd SIM incoming call. The 1st SIM incoming call will be ignored.
- No USSD messages (Except ones with answering option. This is common problem with the ROM build, not the phone itself).
- 2G networking and LTE/UTMS (auto PRL) aka 4,3,2G mode will make the phone somehow unrecognize the SIM. (Don't try to switch this network). Try LTE/WCDMA instead in Test settings. Or edit build.prop and add this line "ro.telephony.default_network=12" at first boot or somehow you can access networking menu in Android 9's Test settings. That will make the modem stable.
- Supports some of Network bands (Better network bands support in Android 8.1, but it doesn't mean it you will get good signals like OG ROM).
- You can't change working Network band in Testing settings.
- For 2nd SIM (Non-mobile data SIM). Choose 2G network and disable Mobile data for that SIM or the phone modem will confused and there will be no signal from any SIM.
- You cannot make 2nd SIM work like 1st SIM acting as a 4G capable Mobile data SIM (No network on both SIM if you try to do that).
**_DO NOT PRE-SET SIM LOCK WHEN YOU PERFORM FIRST BOOT OR YOU'LL GET BOOTLOOPED!_**

## Secure boot (Android 9):
- If you enter the wrong password in the first place. System will force you to press Reset Phone button because you entered the "right" password. **_(1)_**
- Reboot the phone and try de-encrypt (unlock) the phone again. It should be ok.
**_Do not use TWRP to wipe data or use it as main recovery when resetting phone because it will make system fucked up like in (1) and then bootlooped. Only flashing back to stock recovery will solve the problem._**
- If you want to wipe data. Go to fastboot mode and do "fastboot -w" if you unlocked bootloader. Or wipe it normally with stock recovery.

***
## Notes / Other Bugs
- Booting into Android causes screen went out for a few secs. The phone reboots after first boot.
- The phone is still pre-encrypted anyway (Even if you wiped it with TWRP and Not recommended).
- Google Play Services crashed a lot. Install OpenGapps to fix this. But you need to manually remove all Google apps and stock AOSP apps out of system due to lack of space or pick a Non-Gapps Treble build.
- You need to skip the Setup Wizard screen without Internet connection and SIM or you'll stuck with Setup Wizard screen (Because you haven't add "ro.setupwizard.mode=OPTIONAL or DISABLED" and stuck at Checking for Updates screen).
- If so. You need to register the GSF ID first at g.co/AndroidDeviceRegistration. Get the GSF ID by downloading Device ID app. Using terminal command like in Google website instructions will not do anything. Wipe, reboot or make Google Play services force stopped and try adding your account again.
- Alternatively. adb root and then mount /system and go edit prop.default (in /system/etc) and build.prop to match the original fingerprint of the ROM and it should not be detected as a different phone with unofficial fingerprint (You can edit build numbers and Android version).

***

## Tested by:
- Kutiz w/ Nokia 1 (TA-1047 Dual-SIM)


## Tested builds  (With both vendors 00WW_1_x and 00WW_0_x):
- Android 8.1 build v26 w/ Google apps and OpenGapps.
- Android 9.0 build v106 w/ no Google apps and OpenGapps.

_**Last updated:** 1:44 AM; November 15, 2018_