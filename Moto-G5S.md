# Moto G5S

Suitable for daily usage.

## Steps to install (TWRP)

* Flash [this TWRP](https://forum.xda-developers.com/moto-g5s/development/recovery-unofficial-twrp-recovery-moto-t3916370) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Data, Cache and Dalvik/ART Cache.
* Flash [this ROM](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-16-0-project-treble-t3932179).
* Format System.
* Flash a GSI as "System Image" and format data.
* Reboot to system.

## Steps to install (Fastboot)

* Format System, Data, Cache, Boot, and OEM/Vendor. **This will erase internal storage.**
    ```
    $ fastboot format system
    $ fastboot format userdata
    $ fastboot format cache
    $ fastboot format boot
    $ fastboot format oem
    ```
* Flash this [vendor image](https://drive.google.com/open?id=183G4b5InwwLMBtRQxOtEcBDyvRjud9hK) and [boot image](https://drive.google.com/open?id=1UTgTMEYvRSXY4aY6kHmkVYEQTbTFLQLn).
    ```
    $ fastboot flash oem path/to/vendor.img
    $ fastboot flash boot path/to/boot.img
    ```
* Flash a GSI.
    ```
    $ fastboot flash system path/to/gsi.img
    ```
* Reboot.
    ```
    $ fastboot reboot
    ```

[Some more info](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-16-0-project-treble-t3932179)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working, on GSIs install Moto Camera                      |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not working                                               |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Haven't tested                                            |
| Other feature             | N/A                                                       |
---

Tested By: Leandro Manhaes - XT1792 (Brazil), Firmware Version: Oreo BC12, Date tested: May 22nd, 2019
Also tested by: Tiago, null, The Crimin4l - EmpresaSSH, Anirudh Bhati

Template created by @zguithues and @hackintosh5