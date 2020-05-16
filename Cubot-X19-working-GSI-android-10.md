# Cubot X19 
 Havoc Os android 10 with gapps partition A/B.(https://sourceforge.net/projects/havoc-os/files/arm64-ab/)
 use the option with pico gapps included- works fine.


All features work with no bugs at all.
After installation you need to edit your apn settings if mobile data does not work, but otherwise all features are working exclusive of VoLte

## Steps to install

* Enable debugging and enable oem unlock under developer options.
* $ adb reboot bootloader
* flash this image with the `fastboot` utility:
    ```
    $ fastboot devices
    $ fastboot flash system system-arm64-aonly-gapps-nosu.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.This will work if your twrp

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                   |
| Speaker / Mic             | OK                                                   |
| Bluetooth                 | OK                                                   |
| WiFi                      | OK                                                    |
| SIM / Mobile Data / Voice | OK                                                    |
| VoLTE                     | N/A                                                    |
| Fingerprint               | OK                                                    |
| NFC                       | N/A                                                    |
| Offline Charging          | N/A                                                    |
| Other feature             | OK                                                    |
---

Tested By: vincentchege12 -CUBOT_X19_9021C_1_V12_20191219(EA),  - 16/05/2020 - Template created by @zguithues and @hackintosh5

