# Sony Xperia XZ2, "akari", H8296 (dual-sim variant)

**Factory image:** 51.1.A.4.265

**phh-image:** `release/180723/system-arm64-ab-vanilla-nosu.img.xz`\
This is an 8.1 image built on 2018-07-23 using the phh script build.sh.\
The android tag is `android-8.1.0_r36`

**flashing instructions:**  you must adjust the contents of the vbmeta partition before the the XZ2 will boot a GSI (just like the Pixel 2).  This can be done using `fastboot`, but only if the bootloader permits flashing of the vbmeta partition.  Note that the bootloader included with version 51.1.A.2.213 **did not permit vbmeta to be flashed**.

It is probably easiest to flash the "no-op" vbmeta image that phh created (although I think it is possible to build your own "no-op" vbmeta image using aosp).  A link to this file can be found in M. Rahman's XDA article:  
[How to flash a Generic System Image (GSI) on Project Treble supported devices](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)

## Hardware Support

* Camera:
> camera does not work.  The aosp camera app is not responsive -- it just shows a black screen with a camera icon in the middle.

* Speaker / Microphone
> working (tested YouTube, in-call audio).  Strangely, the built-in audio player reports that it does not support mp3.

* Bluetooth
> working (tested device pairing and file transfer).

* Wifi
> working

* SIM / Mobile Data / ingoing voice calls / outgoing voice calls
> Outgoing voice calls are working.  Incoming calls were not tested. Mobile-data was not tested.

* VoLTE
> note tested

* Fingerprint Reader
> working

* 3.5mm audio jack
> the XZ2 does not have a 3.5mm audio jack.  You need a usb-c to audio-jack adapter.

***
## Additional Notes

The screen-backlight flickers.  If you adjust the screen brightness, it is very noticeable.


***


## Tested By:
* https://github.com/jamuir, 2018-07-26
