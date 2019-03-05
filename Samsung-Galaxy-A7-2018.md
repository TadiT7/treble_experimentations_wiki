# Device

Summary of what works and doesn't

## Steps to install

* flash this image with the `fastboot` utility:
    ```
    $ a-command
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Not working                                                    |
| Speaker / Mic             | Working                                                    |
| Bluetooth                 | Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| Dual SIM | Working                                                    |
| VoLTE                     | Not working                                                    |
| Fingerprint               | Working                                                    |
| NFC                       | Working 
| Hotspot / Usb tethering   | Not Working                                           |
---

Tested By: ozon - SM-A750FN(DBT), Firmware Version AOSP 9.0 v110 - Template created by @zguithues and @hackintosh5