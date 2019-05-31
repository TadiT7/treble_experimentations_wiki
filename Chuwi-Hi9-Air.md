# Chuwi Hi9 Air (MTK Helio X20)

Pretty complete feature support and stability.

## Steps to install

* start device with power and vol+ for fastboot mode
* flash [image](https://github.com/phhusson/treble_experimentations/releases/tag/v31) with the `fastboot` utility:
    ```
    $ fastboot oem unlock (must enable in Android developer settings first and confirm onscreen)
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both, front cam upside down)                         |
| Speaker / Mic             | not tested                                                    |
| Bluetooth                 | yes                                                    |
| WiFi                      | yes                                                    |
| SIM / Mobile Data / Voice | yes (but SIM may not reactivate from standby after a while )                                |
| VoLTE                     | no (MTK6797)                                                    |
| Fingerprint               | n/a                                                    |
| NFC                       | n/a                                                    |
| Offline Charging          | not tested                                                    |
| SD Card             | yes                                                    |
| Casting | no, only via Google Home |
---

Tested By: bofh2k - phh-treble 8.1 v31 (gapps/su)- 2019-05-31