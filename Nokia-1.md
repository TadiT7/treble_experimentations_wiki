# [Nokia 1] - [frt]

## Hardware Support

* Camera
> Flashlight in quick settings doesn't work in android 8, 9 works.
> Works. But poorly. (Try Google Camera v3.x or any version of AOSP Camera2 app w/ Material Design on stock ROM to see).
> Use the Camera2 app made by evenwell (the ROM builder for this phone/aka stock camera app from og ROM) might fix all problem, like lack of lighting for example, or Open Camera.

* Speaker / Microphone
> Works.
  
* Bluetooth
> Works, tethering not tested.

* Wi-Fi
> Tethering not work (Probably will make whole system cucked up)

* USB
> Works. RNDIS also works.

*Storage:
> Works. But, Files app doesn't like you showing Internal storage.

* SIM / Mobile Data / Voice
Android 8.1:
> Unable to recognize any SIM (When in 3/4G mode, 2G Works and stable.)
> Go to Android’s Test mode “*#*#4636#*#*” to force GSM network. And then reboot the device. That will make modem Software stable and kept the SIM recognized.
> You can’t change Network band. (Sill applied to Android 9.0)

Android 9.0:
> Works like charm. But for the 2nd SIM/Preferred Mobile data SIM. You have to force that SIM to 2G network because it must work that way, even OG software would make modem act like that.

***
## Additional Notes/Other Bugs
Don’t use TWRP on this ROM. The pre-encrypted userdata in /data you used before flashing this ROM will cause boot loop into the TWRP (Unless you know the password, which is useless because if it was correct or not. It will say wrong anyway.)

Please use the original recovery for this ROM and wipe data.

Booting into Android causes screen went out for a few secs and then booting up again.

The phone is still pre-encrypted anyway.

System apps in Android 8.1 bugs a lot (crash)

Definitely not for Daily Driver use. But Android 9 has potential.

Haven't tested on GPU-side. But I think it will be okay.


***


## Tested by:
* Đức (Kutiz) @ Nokia 1 (TA-1047 DS) @ 9/26/2018

## Tested builds:
Android 8.1 build v25 w/ Google apps
Android 9.0 build v105 w/ no Google apps

Template created by @zguithues
