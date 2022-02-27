## OnePlus 7 Pro 5G <br> <img src="https://cdn2.gsmarena.com/vv/bigpic/oneplus-7-pro-r1.jpg" alt="OnePlus 7 Pro" width="200"/>

## Preliminary information and warnings
You will lose Widevine L1 after unlocking the bootloader, though it's pretty easy to re-flash [stock firmware](https://forum.xda-developers.com/showthread.php?t=3930585) & re-lock the bootloader to regain the functionality.

## Hardware Support

* Camera: Works out of the box. All back cameras were tested to work (Google Camera). The front pop-up camera did not pop up

* Speaker / Microphone : Works out of the box

* Bluetooth : Works out of the box

* Wi-Fi : Works out of the box

* SIM / Mobile Data / Voice / SMS : Works out of the box

* VoLTE : Device supports VoLTE, but is untested

* Fingerprint Reader : Fingerprint sensor is not defined on tested GSI builds. Untested past this point

***
## Additional Notes
### Flashing procedure for OnePlus 7 Pro 5G (guacamoleg and guacamoles) Sprint 5G and EE 5G retail unit (GM1925 and GM1920) running OxygenOS 10.0.15.GM27BA
1. Enable USB debugging and OEM unlock in Developer options
2. `adb reboot bootloader`
3. `fastboot oem unlock` (You may have to use a MSMDownloadTool to force the unlock if you are coming from the Sprint 5G firmware. If you're coming from EU 5G and are SIM Unlocked, this toggle should be toggleable)
4. `fastboot flash system_a  _your_gsi_path_`
5. `fastboot flash system_b  _your_gsi_path_`
6. `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img` (stock vbmeta.img extracted from official update package using Payload Dumper)
7. `fastboot -w (Skip this step if you are wiping in in-built recovery)`
8. `fastboot reboot`
***

## Tested By:
* [TheChosenNopler](https://github.com/thechosennopler)
* Tested with the following builds:
    * [Phh-Treble AOSP 400.e](https://github.com/phhusson/treble_experimentations/releases/tag/v400.e) (system-squeak-arm64-ab-gapps.img) (20220106)
    * [Pixel Experience 12.0 v402.1](https://github.com/ponces/treble_build_pe/releases/tag/v402.1) (PixelExperience_arm64-ab-12.0-20220226-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220226)
    * [Pixel Experience 12.0 v400.h](https://github.com/ponces/treble_build_pe/releases/tag/v400.h) (PixelExperience_arm64-ab-12.0-20220119-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220225)
    * [LeOS](https://leos-gsi.de/downloads/LeOS-S/Feb/) (LeOS-S-VNDK-arm64-bvS) by [Harvey186](https://t.me/harvey186) (20220212)
    * [OctaviOS](https://sourceforge.net/projects/yilliee-projects/files/GSIs/Octavi/v3.2/) (OctaviOS-v3.2-arm64_bgN-29122021-Unofficial) by [Yillié](https://github.com/Yilliee) (20211231)


Template created by [zguithues](https://github.com/zguithues)