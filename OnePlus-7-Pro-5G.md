## OnePlus 7 Pro 5G <br> <img src="https://www.gizmochina.com/wp-content/uploads/2019/05/OnePlus-7-Pro-5G-500x500.jpg" alt="OnePlus 7 Pro 5G" width="250"/>

## Preliminary information and warnings
You will lose Widevine L1 after unlocking the bootloader, though it's pretty easy to re-flash [stock firmware](https://forum.xda-developers.com/showthread.php?t=3930585) & re-lock the bootloader to regain the functionality.

The device is also on a different branch of OxygenOS being on GM27BA or GM25CC compared to the 4G version of the OnePlus 7 Pro which is on GM21xA. 

This also means the kernel is different due to the different modem which is why it is very important you extract and use files from the OnePlus 7 Pro 5G firmware instead.

And no, it is very unlikely that the 4G OnePlus 7 Pro firmware and files will work without heavy modifications.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Speaker / Mic / Calls     | Works                                                     |
| Bluetooth calls           | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| Bluetooth                 | AAC and SBC tested, other bt accessories should work      |
| VoLTE                     | Untested                                                  |
| NFC                       | Works, GPay tested                                        |
| Camera                    | Works*                                                    |
| Fingerprint               | Untested**                                                |
| Charging                  | Works***                                                  |
| USB-C Earbuds             | Works****                                                 |
| Alert Slider              | Works*****                                                |
| DT2W                      | Works******                                               |
| 90Hz                      | Works*******                                              |
| Offline Charging          | Works********                                             |
---

[*] Camera - All back cameras were tested to be working in Android 11, in Android 12 main camera only seems to work in GCam. Pop-up selfie camera does not pop up at all in the  builds tested.

[**] Fingerprint - untested. The location of the fingerprint isn't defined and says to touch the back of the device.

[***] Charging - WARP Charging does not work. Using WARP Charges does but it charges slower. PD Charging also works just fine. Max current measured was 2000mA in Ampere

[****] USB-C Earbuds - works just fine if you tick Alernative Audio Policy in Qualcomm settings and Use Alernative Way to Detect Headsets in Misc settings. This may break calling in 3rd party apps though, untested.

[*****] Alert Slider - all modes but vibrate are working

[******] DT2W - enable DT2W in OnePlus Settings and Misc Settings

[*******] 90Hz - requires Force FPS in Misc Settings to 1440x3120@90.0. This breaks brightness so you also have to tick Force Alternative Backlight Scale.

[********] Auto brightness and battery stats - not working due to no overlay made.

[********] Offline Charging - works but if you unplug the device, you have to force reboot (power + vol up)

**Most of this was tested with PE but should also work on other phh based GSIs if the options are present**

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
* [Adrian](https://github.com/thechosennopler)
* Tested with the following builds:
    * [Phh-Treble AOSP 400.e](https://github.com/phhusson/treble_experimentations/releases/tag/v400.e) (system-squeak-arm64-ab-gapps) (20220106)
    * [Phh-Treble AOSP 400.d](https://github.com/phhusson/treble_experimentations/releases/tag/v400.d) (system-squeak-arm64-ab-gapps) (20211213)
    * [Phh-Treble AOSP 400.c](https://github.com/phhusson/treble_experimentations/releases/tag/v400.c) (system-squeak-arm64-ab-gapps) (20211126)
    * [Pixel Experience 12.0 v402.1](https://github.com/ponces/treble_build_pe/releases/tag/v402.1) (PixelExperience_arm64-ab-12.0-20220226-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220226)
    * [Pixel Experience 12.0 v400.h](https://github.com/ponces/treble_build_pe/releases/tag/v400.h) (PixelExperience_arm64-ab-12.0-20220119-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220225) and (20220120)
    * [Pixel Experience 12.0 v400.e](https://github.com/ponces/treble_build_pe/releases/tag/v400.e) (PixelExperience_arm64-ab-12.0-20211226-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220225)
    * [LeOS](https://leos-gsi.de/downloads/LeOS-S/Feb/) (LeOS-S-VNDK-arm64-bvS) by [Harvey186](https://t.me/harvey186) (20220212)
    * [OctaviOS 3.2](https://sourceforge.net/projects/yilliee-projects/files/GSIs/Octavi/v3.2/) (OctaviOS-v3.2-arm64_bgN-29122021-Unofficial) by [Yillié](https://github.com/Yilliee) (20211231)
    * [Pixel Experience v313](https://github.com/ponces/treble_build_pe/releases/tag/v313) (PixelExperience_arm64-ab-11.0-20211009-UNOFFICIAL) by [ponces](https://github.com/ponces) (20220104)

**year/month/day**

Template created by [zguithues](https://github.com/zguithues)