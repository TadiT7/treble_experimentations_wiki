# Device Info

- Name: Xiaomi Redmi 7A  
- Architecture: arm32_binder64 (a.k.a. a64) and arm64 unofficial @ https://web.telegram.org/#/im?p=@PineOfficial
- System partitions: a-only system partition, but use ab rom
- System-as-root: Yes

## Steps to install
Refer to XDA Thread
https://forum.xda-developers.com/redmi-7a/how-to/custom-gsi-firmware-t3965820

*Some more info*

- Like all Xiaomi's devices, it takes one week to unlock the bootloader.
- If you see insufficient storage when installing gapps resize the system partition on TWRP using the command `resize2fs /dev/block/mmcblk0p57` then try flashing gapps
- If a gsi treble rom does not boot either the rom is not arm 32 binder 64 or your vendor implementation is broken. Try reflashing vendor from MIUI Official Fastboot Rom, links can be found [here](https://mirom.ezbox.idv.tw/en/phone/pine/)
- To root Redmi 7A, patch your boot image by goin to this link https://patcher.yaalex.xyz/ and then flash latest magisk.zip. You may have to manually install magisk manager
- If you want to use 64 bit version or report any bugs try following this telegram link: https://web.telegram.org/#/im?p=@PineOfficial

## Hardware support

| Component                 |      Pie                             |              10                |
|---------------------------|--------------------------------------|--------------------------------|
| Camera                    | Video recording broken after 24 hours| Working from v220 onwards, can be fixed using treble settings from v217 onwards |
| Speaker / Mic             | Working                              | Working                       |
| Bluetooth                 | Working                              | Working                       |
| WiFi                      | Working                              | Working                       |
| SIM / Mobile Data / Voice | Working                              | Working                       |
| VoLTE                     | Working with [Patch]                 | Working with [Patch]          |
| Offline Charging          | Working, hard reboot requried to reach system | Working, hard reboot requried to reach system |
| Magisk           | Working after [patching boot image](https://patcher.yaalex.tk) | Working after [patching boot image](https://patcher.yaalex.tk)                      |
| Root (phh-su) | Working | Working |
| Adoptable Storage         | Working                              | Working                       |
---

Tested By: 
- @KhushrajRathod: VoLTE, Adopted Storage, Camera, Root, Magisk, Offline Charging 
- Ralph Garcia: Other features
   
Tested Roms:
- [10] Phhusson's AOSP 10.0 v222
- [10] Havoc Os 3.8
- [10] Bliss os
        
Template created by @zguithues and @hackintosh5

[Patch]: https://github.com/KhushrajRathod/VoLTE-Fix