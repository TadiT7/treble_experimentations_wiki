# Device

Xiaomi Redmi 7A arm32_binder64 (a.k.a. a64) ab

## Steps to install
Refer to XDA Thread
https://forum.xda-developers.com/redmi-7a/how-to/custom-gsi-firmware-t3965820

    Some more info

    Like all Xiaomi's devices, it takes one week to unlock the bootloader.

    If you have some bugs (quick settings broken, user /data files) with Android 10, first install AOSP 9.0 (v121 recommended), configure your Google account and install latest AOSP 10.0 (only wipe system needed for update).
    If you see insufficient storage when installing gapps try resizing the system partition on twrp (Use the command resize2fs /dev/block/mmcblk0p57) then reboot to recovery and reflash gapps
    If a gsi treble rom does not boot either the rom is not arm 32 binder 64 bit or flash mokee rom first then flash the gsi rom
    To root Redmi 7a flash the correct file according to your system version! http://www.mediafire.com/folder/zx01...a_patched_boot then flash latest magisk zip and install magisk manager (you might need to format your phone)

## Hardware support

| Component                 |      Pie                             |              10                |
|---------------------------|--------------------------------------|--------------------------------|
| Camera                    | Video recording broken after 24 hours| Video recording can be fixed using treble settings from v217|
| Speaker / Mic             | Working                              | Working                       |
| Bluetooth                 | Working                              | Working                       |
| WiFi                      | Working                              | Working                       |
| SIM / Mobile Data / Voice | Working                              | Working                       |
| VoLTE                     | Working with [Patch]                 | Working with [Patch]          |
| Offline Charging          | Working                              | Working                       |
| Root and MAGISK           | Working                              | Working                       |
| Adoptable Storage         | Working                              | Working                       |
| Other feature             | N/A                                  | N/A                           |
---

Tested Roms:

- [10] AOSP 10.0 v216 system-quack-arm32_binder64-ab by phhusson
- [10] AOSP 10.0 v200.d system-quack-arm32_binder64-ab by phhusson
- [10] AOSP 10.0 v214.d system-quack-arm32_binder64-ab by phhusson
- [10] Havoc OS
- [9] Aosp 9
- [9] xiaomi.eu_multi_HM7A_V11.0.2.0.PCMCNXM_v11-9 by ingbrzy
- [9] MK90.0-pine-202002191544-NIGHTLY by GuaiYiHu
- [9] lineage-16.0-20190910-UNOFFICIAL-treble_a64_bvN by AndyYan

Tested By: @KhushrajRathod - VoLTE, Adopted Storage, Camera - Ralph Garcia - Global version
           
Template created by @zguithues and @hackintosh5

[Patch]: https://github.com/KhushrajRathod/VoLTE-Fix