# [Nokia 1] - [frt]

## Hardware Support

* Camera:

Flashlight in quick settings doesn't work in Android 8.

But Android 9 works.

* Speaker / Microphone:

Works.
  
* Bluetooth:

Works, tethering not tested.

* Wi-Fi:

Tethering is broken (Probably will make modem fucked up)

* USB:

Works. RNDIS also works.

* Storage:

Works. But, Files app doesn't like you showing Internal storage.

You still can show Internal storage over 3rd party app requesting picking file. But go to Files app itself will crash again.

Use launcher shortcut to launch the app. It will allow you can see files in Internal storage once.

* SIM / Mobile Data / Voice:

Works, unstable. Better when you using 2 SIMs at once.

Supports some of Network bands.

You can't change networking band.

Force the 1st SIM working in 2G first (and reboot) in Mobile network to make the modem software doesn't crashed.

You need to reboot the phone every single time you change network band.

For 2nd SIM/non-mobile data SIM. Choose 2G network.

* GPU/Video codecs:

Decoding video bugged up when using FPS divisor in Phh Treble Settings (Watching a YouTube video in Chromium. May vary because not every YouTube video using the same codec.)

Haven't tested on GPU-side. But I think it will be okay.

* Secure boot:

If you enter the wrong password in the first place. System will force you to press Reset Phone button because you entered the "right" password.

Reboot the phone and try de-encrypt the phone again. It should be ok.

* FM Radio:

You don't need this shit 😂😂😂 (Not tested and there are no apps for FM Radio to test its functionality)

***
## Additional Notes / Other Bugs

Don’t use TWRP on this ROM. The pre-encrypted userdata in /data you used before flashing this ROM will cause boot loop into the TWRP

(Unless you know the password, which is useless because if it was correct or not. It will say wrong anyway.)

Please use the original recovery for this ROM and wipe data.

Booting into Android causes screen went out for a few secs and then booting up again.

The phone is still pre-encrypted anyway.

System apps in Android 8.1 bugs a lot (crash)

Definitely not for Daily Driver use.


***


## Tested by:
* Đức (Kutiz) @ Nokia 1 (TA-1047 DS Vietnam) @ 9/27/2018

## Tested builds:

Android 8.1 build v25 w/ Google apps

Android 9.0 build v105 w/ no Google apps

Template created by @zguithues
