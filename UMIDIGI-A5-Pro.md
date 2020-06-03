# UMIDIGI A5 Pro
Helio P23 (MT6763V)

Works pretty good. Some issues here and there, some missing features, but mostly usable day-to-day.

## Steps to install
Three possibilities :

### Install using TWRP (Doesn't require unlock) [RECOMMENDED]
1. [Install TWRP](https://sourceforge.net/projects/umidigi-mt6763-dev/files/TWRP/) into ``recovery`` using SPFT method
2. Boot into TWRP : Shut down the phone, press power + vol up. It will bring a menu, you can navigate using vol+ and select using vol-
3. Use "install image" to install system.img into ``system``
4. Use [install image](https://androidfilehost.com/?fid=6006931924117944358) to install vendor_treble_encryptable_a5PRO.img into ``vendor``
5. Clear data partition in TWRP

### Install using SPFT (Doesn't require bootloader unlock)
1. Download [SP Flash Tool](https://spflashtool.com/)
2. You'll also need the [stock ROM](https://community.umidigi.com/forum.php?mod=forumdisplay&fid=221) for it's ``scatter`` file (maps areas in the phone's eMMC)
3. Run SPFT, ``Download`` tab, select the scatter file, untick everything except ``system``, ``vendor_1.4_treble_encryptable_a5PRO`` and ``userdata`` (userdata will format ``data`` partition) and on the right, you can click on the path to choose the correct GSI instead of the stock ROM's system.img .
4. Press Download an plug your phone which in powered down state (not booted, not in recovery).

### Install using fastboot
Unrecommended, shorter to do, but requires a bootloader unlock.
[Needs documentation !]

## Recommended mods
If you choose to format ``data``, before first boot of the GSI, you might want to install ``disable-forceencrypt-treble`` to be able to access ``data`` with TWRP. [Link to it](https://androidfilehost.com/?fid=6006931924117935374) (flashable .zip in TWRP)

You can install Magisk if wanted https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | untested              |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK     |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK SIM1 (SIM2 untested)                                                   |
| VoLTE                     | Untested                                                  |
| Fingerprint               | OK                                                        |
| Offline Charging          | OK                                                        |
| Hotspot / Tethering       | Wifi / Bluetooth|
---

Tested By: @Hadenix - A5 Pro (EU), PHH AOSP 9.0 v119, Havoc-OS-v2.8-20190811-phhgsi_arm64_ab-Official, RR-190406-arm64-ab-vanilla-nosu, AOSP 10.0 v218