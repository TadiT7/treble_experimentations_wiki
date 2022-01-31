# Samsung Galaxy A20
|Custom Rom                 |Daily Drive-able|
|---------------------------|:--------------:|
|Pixel Experience Plus (11) |✅              |
|phh_treble_experiments (12)|✅              |

## Steps to install
1. Make a backup (Usually of everything except recovery, its important for if you do something wrong!)
2. Wipe Data, Dalvik, Cache and System. If you've had encryption on you'll have to "Format Data" (**This wipes Internal Storage too**)
3. Download the system image or Phh_treble supported system image. Preferably VNDKlite (taking note of the treble support [A/B, A-Only])
4. Make sure your file is an ".img" if its a zip, tar or xz (whatever) it probably needs to be extracted.
5. Move system image to your phone. And Flash system image to the "System Partition"
6. Reboot to recovery after flashing to System Partition
7. Flash Disable_DM_Verity which can be obtained [here](https://github.com/Zackptg5/Disable_Dm-Verity_ForceEncrypt) sometimes it's included in the system image but not always so it's best to just flash it.
8. Permissiver_v5 should be flashed if you would like SELinux Status to be Permissive. (**Not recommended!**)
9. If GApps or (GCore) aren't included and you would like them. Firstly resize the system partition through (Wipe>Resize or Format Partition>System>Resize)[if it says failed press repair then resize]. After doing all that you can now flash a GApps zip that's compatible with your android version. (You can find it easily yourself) 
10. You're now ready to boot into the system. Reboot. (It might take a while 'approx 1-6 mins' as it's setting up it's environment for the first time.)
11. Set up the device how you would like it.
12. Install custom kernel, if you would like to do so.
13. If you would like to install Magisk, Open settings > Phh_settings > misc settings and press securize, this should remove SuperSU if installed, Reboot into recovery and flash Magisk.
14. You're Done (Hopefully!)

## Hardware support

| Component                 |      Comment                                                                                 |
|---------------------------|----------------------------------------------------------------------------------------------|
| Camera                    | Yes\*                                                                                        |
| Speaker / Mic             | Yes                                                                                          |
| Headphones                | No\*\*                                                                                       |
| Bluetooth                 | Yes                                                                                          | 
| WiFi                      | Yes                                                                                          |
| SIM / Mobile Data / Voice | Yes                                                                                          |
| VoLTE                     | Possible\*\*\* (enable "Request IMS network" and "Force the presence of 4G Calling service") |
| Fingerprint               | Yes                                                                                          |
| NFC                       | Possible\*\*\*\*                                                                             |
| Offline Charging          | No                                                                                           |
| MTP & PTP                 | Kernel dependent\*\*\*\*\*                                                                   |

[\*] To enable the wide camera go to Phh Treble Settings-> Samsung Features-> Tick "Enable access to all cameras" (**Requires a Q/R vendor**) and reboot. You'll also have to use a camera app that supports it, like Open Camera.

[\*\*] Headphones aren't detected on AOSP 12 (Android R Vendor). Phh Treble Settings don't help.

[\*\*\*] Unsure whether or not it actually uses VoLTE but it displays as its enable. (TESTING)

[\*\*\*\*] NFC seems to be really slow and sometimes even unresponsive.

[\*\*\*\*\*] Having USB debugging enabled whilst using MTP will crash the device. (Still the same with Eureka Kernel)

## Fixed Issues
* Launcher keeps crashing: This happened to me and it might happen to you. I haven't tested the latest build but I will later. What you need to do is download gapps and flash it This will put the navigation bar gestures back and you can use the pixel launcher. ~ [os54656]
* Overlay issues such as UI going off the Display: Installing a vendor_hardware_overlay will fix this. Device fingerprint must contain the device's details to activate the overlay which will be placed in /system/product/overlay. My overlay patch isn't currently available but soon it'll be placed on github along with the source code feel free to help once it's available. [Source](https://github.com/tristanbollard/vendor_hardware_overlay)

## Present Problems (More like to-do list)
- [ ] Solve the gpsd fatal crash (hasn't really affected me but looking to fix)
- [ ] Hyper-HAL's constant nagging of "Couldn't Open Sysfs -- /sys/power/cpufreq_min_limit" and "Couldn't Open Sysfs - /sys/power/cstate_control" (custom kernel doesn't help)
- [x] Upload vendor_hardware_overlay to github and being pushed to source. [Commit](https://github.com/phhusson/vendor_hardware_overlay/pull/417)
---

### Test Log
Tested By: os54656 - SM-A205G , Firmware Version - treble_arm64_bgS-userdebug 10 QQ2A.200305.003 200314 test_keys - I think it is v214 Date tested - 2020-04-13 Template created by @zguithues and @hackintosh5

Second Tested By: tristanbollard - SM-A205YN, Firmware Version system-squeak-arm64-ab-vndklite-gapps.img.xz from (AOSP 12.0 v400.c) of treble experiments - since 10/11/2021-18/11/2021 , Template ever so slightly modified from the previous test.

Third Tested By: tristanbollard - SM-A205YN, Firmware Version Pixel_Experience_Plus_11_v313 from [github](https://github.com/ponces/treble_build_pe) which uses the base of phh_treble so it has the same bugs and issues as phh_treble, Since 18/11/2021-prior, Using Eureka-ONEUI3-Kernel-R8.0 as the kernel.

Fourth Tested By: TBM13 - SM-A205G, GSI: phhusson's AOSP 12.0 v400.h (system-squeak-arm64-ab-vndklite-gapps-secure.img.xz), using stock Kernel and Vendor from Android R (11).
***
