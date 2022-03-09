# Samsung Galaxy A20

Summary of what works and doesn't

## Steps to install

1. Update your phone to Android 11 if you haven't already
2. Unlock bootloader
3. Flash [TWRP](https://twrp.me/samsung/samsunggalaxya20.html)
4. Reboot into TWRP and follow these:
    - Backup (its important for if you do something wrong!)
    - Disable file encryption with [this](https://github.com/Zackptg5/Disable_Dm-Verity_ForceEncrypt)
    - Format Data (**you will lose all of your files located in the internal storage**)
    - Wipe Dalvik, Cache, Data and System
5. Download a GSI image. Preferably VNDKlite (Make sure it's an A/B image)
6. Make sure your file extension is ".img" if its a zip, tar or xz (whatever) it probably needs to be extracted
7. Move the system image to your phone and flash it to the "System Partition"
8. If GApps aren't included and you'd like them, firstly resize the system partition through (Wipe>Resize or Format Partition>System>Resize)[if it says failed press repair then resize]. After doing all that you can now flash a GApps zip that's compatible with your Android version. (You can find it easily yourself) 
9. Reboot to System

## Hardware support

### Android 12
| Component                 |      Comment                                                                                 |
|---------------------------|----------------------------------------------------------------------------------------------|
| Camera                    | Yes\*                                                                                        |
| Speaker / Mic             | Yes                                                                                          |
| Headphones                | Yes\*\*                                                                                      |
| Bluetooth                 | Yes                                                                                          | 
| WiFi                      | Yes                                                                                          |
| SIM / Mobile Data / Voice | Yes                                                                                          |
| VoLTE                     | Untested                                                                                     |
| Fingerprint               | Yes                                                                                          |
| NFC                       | Untested                                                                                     |
| Offline Charging          | No                                                                                           |
| MTP & PTP                 | Kernel dependent\*\*\*                                                                       |

[\*] To enable the wide camera go to Phh Treble Settings-> Samsung Features-> Tick "Enable access to all cameras" (**Requires a Q/R vendor**) and reboot. You'll also have to use a camera app that supports it, like Open Camera.

[\*\*] Headphones aren't detected on most versions of AOSP 12. This should have been fixed on AOSP 12.1.

[\*\*\*] Having USB debugging enabled whilst using MTP will crash the device. (Still the same with Eureka Kernel)

***
### Android 11
| Component                 |      Comment                                                                                 |
|---------------------------|----------------------------------------------------------------------------------------------|
| Camera                    | Yes\*                                                                                        |
| Speaker / Mic             | Yes                                                                                          |
| Headphones                | Yes                                                                                          |
| Bluetooth                 | Yes                                                                                          | 
| WiFi                      | Yes                                                                                          |
| SIM / Mobile Data / Voice | Yes                                                                                          |
| VoLTE                     | Possible\*\*   (enable "Request IMS network" and "Force the presence of 4G Calling service") |
| Fingerprint               | Yes                                                                                          |
| NFC                       | Possible\*\*\*                                                                               |
| Offline Charging          | No                                                                                           |
| MTP & PTP                 | Kernel dependent\*\*\*\*                                                                     |

[\*] To enable the wide camera go to Phh Treble Settings-> Samsung Features-> Tick "Enable access to all cameras" (**Requires a Q/R vendor**) and reboot. You'll also have to use a camera app that supports it, like Open Camera.

[\*\*] Unsure whether or not it actually uses VoLTE but it displays as its enable. (TESTING)

[\*\*\*] NFC seems to be really slow and sometimes even unresponsive.

[\*\*\*\*] Having USB debugging enabled whilst using MTP will crash the device. (Still the same with Eureka Kernel)

---

### Test Log
Tested By: os54656 - SM-A205G , Firmware Version - treble_arm64_bgS-userdebug 10 QQ2A.200305.003 200314 test_keys - I think it is v214 Date tested - 2020-04-13

Second Tested By: tristanbollard - SM-A205YN, Firmware Version system-squeak-arm64-ab-vndklite-gapps.img.xz from (AOSP 12.0 v400.c) of treble experiments - since 10/11/2021-18/11/2021 , Template ever so slightly modified from the previous test.

Third Tested By: tristanbollard - SM-A205YN, Firmware Version Pixel_Experience_Plus_11_v313 from [github](https://github.com/ponces/treble_build_pe) which uses the base of phh_treble so it has the same bugs and issues as phh_treble, Since 18/11/2021-prior, Using Eureka-ONEUI3-Kernel-R8.0 as the kernel.

Fourth Tested By: TBM13 - SM-A205G, GSI: phhusson's AOSP 12.0 v400.h (system-squeak-arm64-ab-vndklite-gapps-secure.img.xz), using stock Kernel and Vendor from Android R (11).
***

Template created by @zguithues and @hackintosh5