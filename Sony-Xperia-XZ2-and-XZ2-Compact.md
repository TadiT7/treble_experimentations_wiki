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
> info about camera support/workarounds

* Speaker / Microphone
> info about Speaker & Microphone support/workarounds

* Bluetooth
> info about Bluetooth support/workarounds

* Wifi
> info about Wifi support/workarounds

* SIM / Mobile Data / ingoing voice calls / outgoing voice calls
> info about SIM / Mobile Data / Voice support/workarounds

* VoLTE
> info about VoLTE support

* Fingerprint Reader
> info about Fingerprint Reader support

* 3.5mm audio jack
> info about 3.5mm audio jack support

***
## Additional Notes

_Put any additional info/notes regarding treble support for this device._


***


## Tested By:
* https://github.com/jamuir, 2018-07-26
