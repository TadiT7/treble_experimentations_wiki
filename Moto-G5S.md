# Moto G5S

Suitable for daily usage.

## Steps to install

### Clean flash
* Flash [this TWRP](https://forum.xda-developers.com/moto-g5s/development/recovery-unofficial-twrp-recovery-moto-t3916370) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Flash [this ROM](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-16-0-project-treble-t3932179).

**Optional:**
* Reboot to TWRP.
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
* Format system and reinstall your GSI.
* Reboot to system.

<!--**Vendor & Boot Images only:**
* Download the latest vendor & boot images [here](https://drive.google.com/folderview?id=1xqfqD4sLJCf6LXsGNFqP-I34qOwPda00).
* Reboot to TWRP.
* Flash the images (Install > Install Image > select partition > select image).
* Reboot to system.-->

### Android 10
* Flash [this TWRP](https://forum.xda-developers.com/moto-g5s/development/recovery-unofficial-twrp-recovery-moto-t3916370) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Flash [these images](https://github.com/montanadevelopment/releases/releases/tag/Android10Beta5-1), respectively to Boot, System Image and Vendor Image.
* Reboot to system.

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
| Other feature             | Encryption - Not Working                                  |

## GSI support

<details><summary>Booting:</summary>
<p>

`Syberia Project`

`Resurrection Remix`

`Android Open Source Illusion Project`

`Pixel Experience`

`ArrowOS`

`BlissROM`

`MIUI`

`Android Open Source Project`

`PixelDust`

`LegionOS`

`LLuviaOS`

`LiquidRemix`

`CarbonROM`

`Evolution X`

`NitrogenOS`

`OxygenOS`

`HydrogenOS`

`ZUI`

`ZenUI`

`Android 10 Beta 5`
</p>
</details>

<details><summary>Not Booting:</summary>
<p>

`OmniROM`

`Havoc-OS`

`LiquidRemix - Other developer`

`Nubia`

`RedMagic`

`Xperia`

`One UI - GSI is too big for /system`
</p>
</details>

---

Tested By: Leandro Manhaes - XT1792 (Brazil), Firmware Version: Oreo BC12, Date tested: May 22nd, 2019

Also tested by: Tiago, null, The Crimin4l - EmpresaSSH, Anirudh Bhati

Template created by @zguithues and @hackintosh5