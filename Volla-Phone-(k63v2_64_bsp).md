# Volla Phone
Seems to work great. 

## Steps to install

* Make sure you are on last Volla OS build, not Ubuntu Touch. You can download [here](https://ota.volla.tech/builds/).  
* Unlock bootloader type `fastboot flashing unlock` in terminal.
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-roar-arm64-ab.img
    ```
    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works, both front and rear                                |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works (untested with audio devices)                      |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Untested                                                  |
| Fingerprint               | Works                                                    |
| NFC                       | Untested                                                  |
| Offline Charging          | Untested                                                  |
| Other feature             |                                                           |
---

Tested By: lukapanio - Volla Phone, volla-9.0-20200702-nightly-k63v2_64_bsp-signed (AOSP 10.0 v221) - July 24, 2020 - Template created by @zguithues and @hackintosh5

