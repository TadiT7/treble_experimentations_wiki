# Realme Q2 Pro


You need to download arm64 and ab gsi image

## Steps to install

* Step 1 Unlock device using realme unlock app and command "fastboot flashing unlock"
* Step 2 flash this image with the `fastbootd` utility and format data:
    ```
    $ a-command
    $ fastboot reboot fastboot
    $ fastboot flash system system-arm64-ab-gapps-su.img
    $ fastboot reboot bootloader
    $ fastboot -w
    ```
* Step 3 Reboot 

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | × Not working                                                    |
| Speaker                   | ✓                                                          |
| Bluetooth                 | ✓                                                    |
| WiFi                      | ✓                                                    |
| SIM / Mobile Data / Voice | ✓                                                   |
| VoLTE                     | × Not working                                                    |
| Fingerprint               | × Not working                                                    |
| Offline Charging          | × Rapid Charge not working,only slow charge working                                                    |
| Notch and rounded corners detection            | × Not working                                                     |
---

Tested By: 寒词ZhuoFan - Realme Q2 Pro, RMX2175_11_OTA_0190_all_4Dv3zsrUtg0a - 9/12/2020 - Template created by @zguithues and @hackintosh5
