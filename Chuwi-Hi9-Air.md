# Device

Pretty complete feature support and stability.

## Steps to install

* start device with power and vol+ for fastboot mode
* flash this image with the `fastboot` utility:
    ```
    $ fastboot oem unlock (must eanble in developer settings first and confirm onscreen)
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both, front cam upside down)                         |
| Speaker / Mic             | not tested                                                    |
| Bluetooth                 | yes                                                    |
| WiFi                      | yes                                                    |
| SIM / Mobile Data / Voice | yes (but SIM may no reactivate from standby after a while )                                |
| VoLTE                     | no (MTK6797)                                                    |
| Fingerprint               | n/a                                                    |
| NFC                       | n/a                                                    |
| Offline Charging          | not tested                                                    |
| SD Card             | yes                                                    |
---

Tested By: bofh2k - phh-treble 8.1 v31 (gapps/su)- 2019-05-31