# Umidigi One Max
Helio P23 (MT6763T)

Works pretty good. Some issues here and there, some missing features, but mostly usable day-to-day.

## Steps to install
Three possibilities :

### Install using TWRP (Doesn't require unlock) [RECOMMENDED]
1. [Install TWRP](https://twrp.me/umidigi/onemax.html) into ``recovery`` using SPFT method
2. Boot into TWRP : Shut down the phone, press power + vol up. It will bring a menu, you can navigate using vol+ and select using vol-
3. Use "install image" to install system.img into ``system``
4. Clear ``data`` partition in TWRP

### Install using SPFT (Doesn't require bootloader unlock)
1. Download [SP Flash Tool](https://spflashtool.com/)
2. You'll also need the [stock ROM](https://community.umidigi.com/forum.php?mod=forumdisplay&fid=211) for it's ``scatter`` file (maps areas in the phone's eMMC)
3. Run SPFT, ``Download`` tab, select the scatter file, untick everything except ``system`` and ``userdata`` (userdata will format ``data`` partition) and on the right, you can click on the path to choose the correct GSI instead of the stock ROM's system.img .
4. Press Download an plug your phone which in powered down state (not booted, not in recovery).

### Install using fastboot
Unrecommended, shorter to do, but requires a bootloader unlock.
[Needs documentation !]

## Recommended mods
If you choose to format ``data``, before first boot of the GSI, you might want to install ``disable-forceencrypt-treble`` to be able to access ``data`` with TWRP (it cannot decrypt currently). [Link to it](https://github.com/phhusson/treble_experimentations/issues/572#issuecomment-503979784) (flashable .zip in TWRP)

You can install Magisk if wanted. You'll need to do the fix in https://github.com/phhusson/treble_experimentations/issues/572#issuecomment-503979784 to have root prompts.

SafetyNet doesn't pass because of wrong fingerprint. There is a magisk mod for that, look it up. It works then.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works as expected (choppy like original ROM)              |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK. Some disconnects at moments but still very rare.      |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | Outgoing / SMS is flawless. Ingoing sometimes doesn't appear, but still hard to reproduce. Data works on SIM1 (SIM2 untested) but in low-signal uses, will "glitch out" (shows no data, and 0 signal) but still apparently works like 4G.                                                     |
| VoLTE                     | Untested                                                  |
| Fingerprint               | OK                                                        |
| NFC                       | OK with Magisk module [NFC4PRA](https://github.com/Magisk-Modules-Repo/NFC4PRA-GSI), or won't show at all in settings                                                           |
| Offline Charging          | OK                                                        |
| Hotspot / Tethering       | Wifi / Bluetooth / USB tethering not working when data is ON. Works when OFF.|
---

Tested By: @defvs - One Max (EU), PHH AOSP 9.0 v112 - Template created by @zguithues and @hackintosh5

# Suggestion: can you add notes to clarify if/why one should twrp apply patches.zip and if you used system_arm64_aonly_gapps_su.img.xz or system_arm64_aonly_vanilla_nosu.img.xz system image file?