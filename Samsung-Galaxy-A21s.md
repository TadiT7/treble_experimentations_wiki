# Device

Summary of what works and doesn't

## Steps to install

* Step 1
  Reboot to Odin Mode and flash the vbmeta recovery file linked here
* Step 2
  Then reboot to recovery and go to advanced options
* Step 3
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
| Camera                    | Status                                                    |
| Speaker / Mic             | Status                                                    |
| Bluetooth                 | Status                                                    |
| WiFi                      | Status                                                    |
| SIM / Mobile Data / Voice | Status                                                    |
| VoLTE                     | Status                                                    |
| Fingerprint               | Status                                                    |
| NFC                       | Status                                                    |
| Offline Charging          | Status                                                    |
| Other feature             | Status                                                    |
---

Tested By: username - Model-Number(region), Firmware Version - Date tested - Template created by @zguithues and @hackintosh5
