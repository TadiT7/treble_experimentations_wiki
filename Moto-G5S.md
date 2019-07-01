# Moto G5S

Suitable for daily usage.

## Steps to install

### Clean flash
* Flash [this TWRP](https://forum.xda-developers.com/moto-g5s/development/recovery-unofficial-twrp-recovery-moto-t3916370) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Data, Cache and Dalvik/ART Cache.
* Flash [this ROM](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-16-0-project-treble-t3932179).
**Optional:**
* Format System.
* Flash a GSI as "System Image". Or alternatively use fastboot to flash the GSI:
```
fastboot flash system path/to/gsi.img
```
* Reboot to system.

### Dirty flash

**Whole system:**
* Reboot to TWRP.
* Flash the latest LineageOS Treble zip.
* Reboot to system.

**Vendor & Boot Images only:**
**Download the latest vendor & boot images [here](https://drive.google.com/folderview?id=1xqfqD4sLJCf6LXsGNFqP-I34qOwPda00)**
**Reboot to TWRP.**
**Flash the images (Install > Install Image > select partition > select image)**.
**Reboot to system.**

[Some more info](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-16-0-project-treble-t3932179)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working                                                   |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | Enabling/disabling navigation bar broken in stock Lineage |
---

Tested By: Leandro Manhaes - XT1792 (Brazil), Firmware Version: Oreo BC12, Date tested: May 22nd, 2019
Also tested by: Tiago, null, The Crimin4l - EmpresaSSH, Anirudh Bhati

Template created by @zguithues and @hackintosh5