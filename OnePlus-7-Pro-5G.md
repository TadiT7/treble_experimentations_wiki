## OnePlus 7 Pro 5G <br> <img src="https://cdn2.gsmarena.com/vv/bigpic/oneplus-7-pro-r1.jpg" alt="OnePlus 7 Pro" width="200"/>

## Preliminary information and warnings
You will lose Widevine L1 after unlocking the bootloader, though it's pretty easy to re-flash [stock firmware](https://forum.xda-developers.com/showthread.php?t=3930585) & re-lock the bootloader to regain the functionality.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works*                                                    |
| Speaker / Mic / Calls     | Works                                                     |
| Bluetooth                 | AAC and SBC tested, everything else untested              |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Untested                                                  |
| Fingerprint               | Untested**                                                |
| NFC                       | Untested                                                  |
| Bluetooth calls           | Works                                                     |
| Charging                  | Works***                                                  |
| USB-C Earbuds             | Works****                                                 |
| Alert Slider              | Works*****                                                |
| DT2W                      | No                                                        |
| 90Hz                      | Works******                                               |
---

[*] Camera - All back cameras were tested to be working in Android 11, in Android 12 main camera only seems to work in GCam. Pop-up selfie camera does not pop up at all in the  builds tested.

[**] Fingerprint - untested. The location of the fingerprint isn't defined and says to touch the back of the device.

[***] Charging - WARP Charging does not work. Using WARP Charges does but it charges slower. PD Charging also works just fine. Max current measured was 2000mA in Ampere

[****] USB-C Earbuds - works just fine if you tick Alernative Audio Policy in Qualcomm settings and Use Alernative Way to Detect Headsets in Misc settings. This may break calling audio in 3rd party apps though, untested.

[*****] Alert Slider - all modes but vibrate are work

[******] 90Hz - requires Force FPS in Misc Settings to 1440x3120@90.0. This breaks brightness so you also have to tick Force Alternative Backlight Scale.

[*******] Auto brightness and battery stats - not working due to no overlay made.

***
## Additional Notes



### Flashing procedure for OnePlus 7 Pro 5G (guacamoleg and guacamoles) Sprint 5G and EE 5G retail unit (GM1925 and GM1920) running OxygenOS 10.0.15.GM27BA
1. Enable USB debugging and OEM unlock in Developer options (If you are using the Sprint 5G firmware as a base, don't. Use the EU 5G firmware as a base. The OEM Unlock toggle is not greyed out on the EU 5G firmware)
2. `adb reboot bootloader`
3. `fastboot oem unlock` 
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