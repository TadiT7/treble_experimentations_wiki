# [Nokia 1] - [frp]

## Hardware Support

* Camera
> Works. But poorly. (Try Google Camera v3.x or any version of AOSP Camera2 app w/ Material Design on stock ROM to see).
> Use the Camera2 app made by evenwell (the ROM builder for this phone/aka stock camera app from og ROM) might fix all problem, like lack of lighting for example.

* Speaker / Microphone
> Works. Mic haven’t tested yet. But it should Works.
  
* Bluetooth
> Kinda? Also tethering mobile data over Bluetooth is impossible.

* Wi-Fi
> Tethering might not work.

* SIM / Mobile Data / Voice
> Unable to recognize any SIM (When in 3/4G mode, 2G Works.)
> Go to Android’s Test mode “*#*#4636#*#*” to force GSM network. And then reboot the device. That will make modem Software stable and kept the SIM recognized.
> In 2G networking. No PDP caching (No internet connection whatsoever).
> You can’t change Network band.

***
## Additional Notes
Don’t use TWRP on this ROM. The pre-encrypted userdata in /data you used before flashing this ROM will cause boot loop into the TWRP (Unless you know the password, which is useless because if it was correct or not. It will say wrong anyway.)

Please use the original recovery for this ROM.

Booting into Android causes screen went out for a few secs and then booting up again.

The phone is still pre-encrypted anyway.

Tested on 1st SIM slot. Haven’t tested on 2nd SIM slot yet.

Google Play services crashes a lot.

On Files app (In storage settings). When showing Internal storage cause the app force stop once or many times. Once is when I reinstalled the ROM and wiped it.

Definitely not for Daily Driver use.

You can't wipe data on TWRP? You better using stock recovery.

Some of my claims are might not true because I went to Nokia and asked them to reinstall the stock ROM the next day, so I can't remember exactly what I've experienced.


***


## Tested By:
* Đức (Kutiz) @ Nokia 1 (TA-1047 DS) @ 7/15/2018

Template created by @zguithues
