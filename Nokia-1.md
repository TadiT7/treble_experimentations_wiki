# [Nokia 1] - [frt]

## Hardware Support

* Sensors

Can't detect any thermal sensors (example: battery's temp, battery's voltage).

Accelerometer, Light and Proximity sensors works fine.

* GPS:

Actually works. (Not tested on Android 9).

* Camera / Flashlight

Flashlight works fine.

Unoptimized Camera2 app. Which leads to low-lighting on both front and back camera. Installing stock rom's Camera app might help.

Pretty much anything else works fine.

* Speaker / Microphone:

Works.
  
* Bluetooth:

Works, FTP file transfer doesn't work with files like APK (content not supported) but files like JPG works, tethering works.

* Wi-Fi:

Works.

* USB:

Works.

* Storage:

Works. But, Files app doesn't like you showing Internal storage.

You still can show Internal storage over 3rd party app requesting picking file. But go to Files app itself will crash again.

Use launcher shortcut to launch the app. It will allow you can see files in Internal storage once.

If you made it crashed constantly. Clean up the app data will do the trick.

* SIM / Mobile Data / Voice:

Only Notifies one SIM incoming call. The 2nd SIM incoming call will be ignored.

If you don't wanna mess with the phone being "No SIM card" all the time. Just stick a SIM on the phone when you perform first boot. (Keep the Mobile data turned on).

Supports some of Network bands.

You can't change networking band in Testing settings.

For 2nd SIM/non-mobile data SIM. Choose 2G network or the phone modem will confused.

No USSD's messages. But performing USSD menu works fine.

DO NOT PRE-SET SIM LOCK WHEN YOU PERFORM FIRST BOOT OR YOU'LL GET BOOTLOOPED!

* GPU / Video decoding:

Works fine. GPU works smoother in this ROM.

* Secure boot (Applies to Android 9):

If you enter the wrong password in the first place. System will force you to press Reset Phone button because you entered the "right" password.

Reboot the phone and try de-encrypt (unlock) the phone again. It should be ok.

* FM Radio:

You don't need this shit 😂😂😂 (Not tested and there are no apps for FM Radio to test its functionality).

But I bet it won't work.

***
## Additional Notes / Other Bugs

Keep the bootloader unlocked to Wipe data and cache properly when you using TWRP recovery.

There's a bug when previous userdata from stock ROM using with this GSI ROM will make the pre-encrypted user's data in /data corrupted and make a infinite bootloop into TWRP when you pressed RESET PHONE. So basically. You can't perform Resetting phone over TWRP. Use stock recovery instead.

Booting into Android causes screen went out for a few secs. The phone reboots after first boot.

The phone is still pre-encrypted anyway.

Google Play Services crashed alot. Install OpenGapps to fix this. But you need to manually removes Google apps and stock AOSP apps out of system due to lack of space.

DO NOT SETUP ANY GOOGLE ACCOUNT OR CONNECTING THE PHONE TO THE INTERNET OR GOOGLE PLAY SERVICES WILL SPAM NOTIFICATION.

You need to register the GSF ID first at g.co/AndroidDeviceRegistration. Get the GSF ID by downloading Device ID app. Using terminal command will not do anything.

That means you need to skip the Setup Wizard screen without Internet connection or you'll stuck with Setup Wizard screen.

Wipe or make Google Play services Force stopped and try adding your account again.

Definitely not for Daily Driver use.

***


## Tested by:

Đức (Kutiz) @ Nokia 1 (TA-1047 DS Vietnam) @ 10/12/2018

## Tested builds:

Android 8.1 build v26 w/ Google apps and OpenGapps.

Android 9.0 build v106 w/ no Google apps and OpenGapps.

Template created by @zguithues
