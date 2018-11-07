# [Nokia 1] - [frt]

## Hardware Support

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

* SIM:

Only notifies one SIM incoming call. The 2nd random SIM incoming call will be ignored (Fucked up Dual SIM-Dual Standby mode).

If you don't wanna mess with the phone being "No SIM card" all the time: In Android 8, go to Mobile data settings, make only one SIM slot have Mobile data enabled. Other wise modem will be crashed. Reboot to take effects.

I didn't find any obvious way to fix this yet in Android 9. But let the phone booted up after 2 mins will make the Modem software stable but Mobile data have to turned on.

Supports some of Network bands (Better network bands support in Android 8.1).

You can't change networking band in Testing settings.

For 2nd SIM/non-mobile data SIM. Choose 2G network or the phone modem will confused and crashed.

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

You don't need this shit 😂😂😂 (Not tested and there are no apps for FM Radio to test its functionality).

But I bet it won't work.

***
## Additional Notes / Other Bugs

Booting into Android causes screen went out for a few secs. The phone reboots after first boot.

The phone is still pre-encrypted anyway.

Google Play Services crashed a lot. Install OpenGapps to fix this. But you need to manually remove all Google apps and stock AOSP apps out of system due to lack of space or pick a Non-Gapps Treble build.

You need to skip the Setup Wizard screen without Internet connection and SIM or you'll stuck with Setup Wizard screen (Mostly because it didn't show skip button when selecting network and spamming unofficial phone ROM detection).

You need to register the GSF ID first at g.co/AndroidDeviceRegistration. Get the GSF ID by downloading Device ID app. Using terminal command like in Google website instructions will not do anything.

Wipe, reboot or make Google Play services force stopped and try adding your account again.

Definitely not for Daily Driver use.

***


## Tested by:

Kutiz w/ Nokia 1 (TA-1047 DS Vietnam) @ 11/07/2018

## Tested builds:

Android 8.1 build v26 w/ Google apps and OpenGapps.

Android 9.0 build v106 w/ no Google apps and OpenGapps.
