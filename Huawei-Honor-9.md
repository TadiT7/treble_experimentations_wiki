### Flash instructions:

1. Backup data with [TWRP](https://forum.xda-developers.com/honor-9/development/oreo-t3754483) or other backup tool:
`adb reboot recovery`
_(reboots into your recovery and stock recovery if you haven't installed a custom recovery)_

2. Reboot to eRecovery

3. Wipe (factory reset including data) with stock Recovery (not eRecovery; you will need to reflash a stock recovery through fastboot) (TWRP wipe doesn't currently work)

3.1 Wipe (factory reset) works in this [TWRP-Mod for Huawei/Honor only with EMUI 9](https://4pda.ru/forum/index.php?showtopic=934177&st=60#entry82590973).
[TWRP-Mod for Huawei/Honor only with EMUI 9.1](https://4pda.ru/forum/index.php?showtopic=934177&view=findpost&p=88038324).
Direct download link [TWRP-Mod for Huawei/Honor only with EMUI 9](https://my.pcloud.com/publink/show?code=XZdQCI7ZxsXVkgOqQmX0nb4HpWBQTXoibubV).
Direct download link [TWRP-Mod for Huawei/Honor only with EMUI 9.1](https://my.pcloud.com/publink/show?code=XZIe9QkZaK1MK6QaqImiom7Tm8a97Ht7e2kV).

4. Reboot device `fastboot reboot`

5. Reboot to fastbootmode

5. Flash ROM GSINAME.img to system partition using fastboot
`fastboot flash system GSINAME.img`
_(replace GSINAME.img with the name and location of your GSI image)_

4. Reboot device `fastboot reboot`

5. If your having any problems go back into TWRP and wipe the dalvik cache


### Hardware commands - done with device turned off

#### Need to connect the computer:

- `Fastboot mode`: long press the volume down key + power button.

- `eRecovery mode`: long press the volume up key + power button.

#### Do not need to connect the computer:

- `Recovery mode`: long press the volume up key + power button.

- `Upgrade mode`: long press the volume up key + volume down key + power button.


### Additional infos:

- EMUI 8.0 & 8.1 use ARM64 A Roms.
- EMUI 9.0 & 9.1 use ARM64 AB ROMs due to system as root (if in doubt check [here](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck)).

- GSIs tested and working well: [OpenKirin](https://openkirin.net/download/)
- [Ported stock Camera exists](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/kirin-huawei-camera-android-p-t3840110) and mostly work, keeping original quality.

- Brightness stuck at 40%, both in settings and real life.  
_May be not an issue anymore, started from v19 (2018-06-03), now using v23 (2018-08-07) and never been able to reproduce._

- On-screen navigation buttons can be hidden by adding `qemu.hw.mainkeys=1` to /system/build.prop

- [Home button behavior](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/huawei-disable-fingerprint-navigation-t3801708) can be set to default (to behave as on EMUI) by replacing /system/phh/huawei/fingerprint.kl content with the following line: `key 174 HOME`