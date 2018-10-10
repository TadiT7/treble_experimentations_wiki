# [Nokia 1] - [frt]

## Hardware Support

* Sensors

Can't detect any thermal sensors (example: battery's temp, battery's voltage).

Accelerometer, Light and Proximity sensors works fine.

* GPS:

Didn't work. If worked. It uses Wi-Fi scanning and Bluetooth scanning. But very inaccurate.

* Camera / Flashlight

Flashlight works fine.

Back camera's exposure is very low and can't be changed with stock Camera2 app (Even on stock ROM when using this app, it's the same. Manual exposure option in settings doesn't do anything). Use Camera app from Stock ROM might helps.

HDR kinda works.

Front camera works fine.

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

Works, unstable.

Supports some of Network bands.

You can't change networking band.

Force the 1st SIM working in 2G first (and reboot) in Mobile network to make the modem software doesn't crashed. Then you will allowed to change any network mode without SIM unrecognizable bug.

For 2nd SIM/non-mobile data SIM. Choose 2G network.

* GPU / Video decoding:

Works fine. You'll get extra 10 FPS out of 50 FPS on stock ROM.

* Secure boot (Applies to Android 9):

If you enter the wrong password in the first place. System will force you to press Reset Phone button because you entered the "right" password.

Reboot the phone and try de-encrypt the phone again. It should be ok.

* FM Radio:

You don't need this shit 😂😂😂 (Not tested and there are no apps for FM Radio to test its functionality).

But I bet it won't work.

***
## Additional Notes / Other Bugs

Keep the bootloader unlocked to Wipe data and cache properly when you using TWRP recovery.

There's a bug when previous userdata from stock ROM using with this GSI ROM will make the pre-encrypted user's data in /data corrupted and make a infinite bootloop into TWRP when you pressed RESET PHONE. So basically. You can't perform Resetting phone over TWRP. Use stock recovery instead.

Booting into Android causes screen went out for a few secs and then booting up again.

The phone is still pre-encrypted anyway.

The phone reboot once after it done with the first boot.

Google Play Services crashed alot. Install OpenGapps to fix this. But you need to manually removes Google apps and stock AOSP apps out of system due to lack of space.

You need to register the phone's ID before you can use any Google services or add Google account onto it. Or any Google app will spam the shit out the notification and you can't use any Google services.

That means you need to skip the Setup Wizard screen without internet connection.

Get the Device's Google ID first (Not Android's ID) by Downloading Device ID app, using terminal adb way will not work at all. Then register it at at g.co/AndroidDeviceRegistration.

Wipe or make Google Play services Force stopped and try adding your account again.

Definitely not for Daily Driver use.

***


## Tested by:

Đức (Kutiz) @ Nokia 1 (TA-1047 DS Vietnam) @ 10/10/2018

## Tested builds:

Android 8.1 build v26 w/ Google apps and OpenGapps.

Android 9.0 build v106 w/ no Google apps and OpenGapps.

Template created by @zguithues
