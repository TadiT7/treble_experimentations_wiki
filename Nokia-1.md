# [Nokia 1] - [frt]

## *Hardware Support (For vendor from build 00WW_1_)*

* Storage:

Due to new ROM rebuild. Nokia made Files app show up into home screen (Except stock ROM).

Showing Internal Storage no longer crashing the Files app anymore.

* SIM:

Almost fixed everything.

No more SIM unrecognizing, Modem crashing. (You can choose 2G network or 2G only working along side with 4G aka LTE/UMTS (auto PRL)).

Network bands are now can be selected in Testing settings. (star pound star pound 4636 pound star pound star)

You cannot make 2nd SIM work like 1st SIM acting as 4G capable Mobile data SIM like version 00WW_0_* one. Both SIM will have no signal.

Still no USSD messages (Except ones with answering option. This is common problem with the ROM build, not the phone itself).

* Notes:

Unlisted categories means they have behaviors the same with the previous vendor build.

## *Hardware Support (For vendor from build 00WW_0_)*

* Sensors

Can't detect any thermal sensors (example: battery's temp, battery's voltage).

Accelerometer, Light and Proximity sensors works fine.

* GPS:

Works, kind of (No GPS signal, but does when have Wi-Fi and Mobile data connection around).

* Camera / Flashlight

Flashlight works fine.

Unoptimized Camera2 app. Which leads to low-lighting on both front and back camera. Installing stock rom's Camera app might help but won't save pics. Camera2 app from Android 4.4 will fix everything.

Pretty much anything else works fine.

* Speaker / Microphone:

Works.
  
* Bluetooth:

Works.

* Wi-Fi:

Works. Tethering doesn't work with Android 9.

* USB:

Works.

* Storage:

Works. But, Files app doesn't like you showing Internal storage (Constantly crashing app).

You still can show Internal storage over 3rd party app requesting picking file. But go to Files app itself will crash again.

Use a launcher shortcut to launch the app or in Storage settings.

If you made it crashed constantly. Clean up the app data will do the trick.

Use Google's Files app (Previously Files go). It will show you both Internal and SD card storage.

* SIM:

Only notifies 2nd SIM incoming call. The 1st SIM incoming call will be ignored.

2G networking will make the phone somehow unrecognize the SIM. (Don't try to switch this network)

You cannot make 2nd SIM work like 1st SIM acting as 4G capable Mobile data SIM.

If you don't wanna mess with the phone being "No SIM card" or No network receptions: Set phone networking mode to LTE/WCDMA (not LTE/UMTS (auto PRL)) or edit build.prop and add this line "ro.telephony.default_network=12" at first boot or somehow you can access networking menu in Android 9. That will make the modem stable.

Rather don't use 2 SIM in this phone.

Supports some of Network bands (Better network bands support in Android 8.1. It doesn't mean it you will get signal like OG ROM).

You can't change working Network band in Testing settings.

For 2nd SIM (Non-mobile data SIM). Choose 2G network and disable Mobile data for that SIM or the phone modem will confused and there will be no signal from any SIM.

No USSD's messages. But performing USSD menu works fine.

DO NOT PRE-SET SIM LOCK WHEN YOU PERFORM FIRST BOOT OR YOU'LL GET BOOTLOOPED!

* GPU / Video decoding:

Works fine. GPU works smoother in Android 9 only.

* Secure boot (Applies to Android 9):

If you enter the wrong password in the first place. System will force you to press Reset Phone button because you entered the "right" password. (1)

Reboot the phone and try de-encrypt (unlock) the phone again. It should be ok.

Do not use TWRP to wipe data because it will make system fucked up like in (1). Only flashing back to stock recovery will solve the problem.

If you want to wipe data. Go to fastboot mode and do "fastboot -w" if you unlocked bootloader. Or wipe it normally with stock recovery.

* FM Radio:

Not tested and there are no apps for FM Radio to test its functionality. But perhaps it won't work.

***
## Additional Notes / Other Bugs

Booting into Android causes screen went out for a few secs. The phone reboots after first boot.

The phone is still pre-encrypted anyway.

Google Play Services crashed a lot. Install OpenGapps to fix this. But you need to manually remove all Google apps and stock AOSP apps out of system due to lack of space or pick a Non-Gapps Treble build.

You need to skip the Setup Wizard screen without Internet connection and SIM or you'll stuck with Setup Wizard screen (Because you haven't add "ro.setupwizard.mode=OPTIONAL or DISABLED" and stuck at Checking for Updates screen).

If so. You need to register the GSF ID first at g.co/AndroidDeviceRegistration. Get the GSF ID by downloading Device ID app. Using terminal command like in Google website instructions will not do anything. Wipe, reboot or make Google Play services force stopped and try adding your account again.

Alternatively. adb root and then mount /system and go edit prop.default (in /system/etc) and build.prop to match the original fingerprint of the ROM and it should not be detected as a different phone with unofficial fingerprint (You can edit build numbers and Android version).

Definitely not for Daily Driver use.

***


## Tested by:

Kutiz w/ Nokia 1 (TA-1047 DS Vietnam) @ 11/15/2018

## Tested builds:

Android 8.1 build v26 w/ Google apps and OpenGapps (With both vendor 00WW_1_* and 00WW_0_*

Android 9.0 build v106 w/ no Google apps and OpenGapps.
