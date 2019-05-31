# Chuwi Hi9 Air (MTK Helio X20)

Pretty complete [hardware](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) support and stability.

## Steps to install

* enable OEM unlock in Android developer settings
* reset device to factory settings and power off
* start device with _power_ and _vol+_ for fastboot mode
* flash [image](https://github.com/phhusson/treble_experimentations/releases/tag/v31) with the `fastboot` utility:
    ```
    $ fastboot oem unlock (must enable in Android developer settings before and confirm onscreen then)
    $ fastboot erase system
    $ fastboot -u flash system system-arm64-aonly-gapps-su.img
    ```
    Alternativly, you can flash via TWRP as "System Image" and format data: [Link](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both, but front cam upside down)                     |
| Speaker / Mic             | not tested                                                |
| Bluetooth                 | yes                                                       |
| WiFi                      | yes                                                       |
| SIM / Mobile Data / Voice | yes (SIM1, may not reactivate from standby after a while )|
| VoLTE                     | no (MTK6797)                                              |
| Fingerprint               | n/a                                                       |
| NFC                       | n/a                                                       |
| Offline Charging          | not tested                                                |
| SD Card                   | yes                                                       |
| Casting.                  | no, only via Google Home                                  |
---

Tested By: bofh2k - phh-treble 8.1 v31 (gapps/su) - 2019-05-31