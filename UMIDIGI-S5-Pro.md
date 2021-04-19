# UMIDIGI S5 Pro
Component Type | Details
-------:|:-------------------------
Platform | Mediatek MT6785 Helio G90T (12 nm)
GPU     | Mali-G76 MC4 (Arm Mali-G76 3EMMC4)
Architecture | 64 bit (A/B)
Memory  | 6 GB RAM
Shipped Android Version | 	Android 10 Q (VNDK29)
Screen resolution | 1080 x 2340 pixels (403 PPI) , AMOLED Ultra FullView
Sensors | Fingerprint (In-display fingerprint sensor), Accelerometer, Gyro, Proximity, Compass

Works pretty good and seems to be usable day-to-day. In terms of customisation the rom even perfomes better than stock rom.

Known Issues are:
* fingerprint scanner not working correctly
* dark mode is not optimized for the amoled display
* Magisk install currently broken (bootloops) [ Seems to be a well known Issue for Magisk on Android 11 ]

## Steps to install

> Step 1: Preperation Oem unlock (only needs to be done once for GSI installs)
> * 1.0 In developer options enable "Oem unlocking" & "USB debugging"
> * 1.1 adb reboot bootloader
> * 1.2 fastboot flashing unlock and then fastboot flashing unlock_critical

> Step 2: Disable Android verification
> * 2.0 fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img (vbmeta from the stock rom)
> * 2.1. fastboot --disable-verity --disable-verification flash vbmeta_system vbmeta_system.img (also from the stock rom)


> Step 3: Flash GSI (in fastbootd)
> * 3.0 fastboot reboot fastboot
> * 3.1 fastboot erase system
> * 3.2 fastboot delete-logical-partition product
> * 3.3 fastboot flash system (insert your desired arm64 A/B GSI)
> * 3.4 fastboot reboot bootloader

> Step 4: Disable Android verification (just to be save)
> * 4.0 fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img (from the stock rom)
> * 4.1 fastboot --disable-verity --disable-verification flash vbmeta_system vbmeta_system.img (from the stock rom)

> Step 5: Factory reset (recomended for clean GSI install)
> * 5.0 fastboot -w (!!! Erases userdata and cache !!!)

> Reboot device + Gapps device certification
> * fastboot reboot
> * On Error message: "Device not Certified"
>   * Go To: https://www.google.com/android/uncertified/ and follow the instructions
    * Longpress on a "Device not Certified" error message
    * reboot (if it still shows up after reboot longpress the notification and in notification settigs turn of the highlighted option)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works as expected (choppy like original ROM)                                                    |
| Speaker / Mic             | OK                                                    |
| Bluetooth                 | OK                                                    |
| WiFi                      | OK                                                    |
| SIM / Mobile Data / Voice | Untested but seems to work fine                                                    |
| VoLTE                     | Untested                                                    |
| Fingerprint               | Broken, thinks it is a scanner at the back of the phone                                                    |
| NFC                       | Untested but seems to work fine                                                    |
| Offline Charging          | Broken, display shows boot screen indefinenty untill unplugged or turned on                                                    |
| Hotspot / Tethering       | Ok                                                   |
| TWRP                      | Currently worked on                                                   |
---

##Related links & repositories

* TWRP Device Tree: https://github.com/lopestom/device_Umidigi_S5-Pro
* Official Umidigi device forum: https://community.umidigi.com/forum.php?mod=forumdisplay&fid=232
* Official Umidigi device Roms: https://community.umidigi.com/forum.php?mod=forumdisplay&fid=234
* XDA Root Guide for S5 Pro: https://forum.xda-developers.com/t/guide-rooting-the-umidigi-s5-pro-magisk.4151183/
* XDA Universal GSI flash Guide: https://forum.xda-developers.com/t/how-to-flash-gsis-on-devices-with-dynamic-super-partition.4256667/
* XDA fix "Device not Certified" error: https://www.xda-developers.com/how-to-fix-device-not-certified-by-google-error/

Tested By: @4ctiv - S5 Pro(EU), PHH AOSP 11.0 v305 system-roar-arm64-ab-gapps.img
 - 18/19.Apr.2021 - Template created by @zguithues and @hackintosh5