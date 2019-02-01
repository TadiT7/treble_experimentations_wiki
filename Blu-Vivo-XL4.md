# Device. Blu vivo XL 4

Summary of what works and doesn't

## Steps to install

* Step 1 enable oem-unlock in Dev options
* Step 2 from fastboot oem ulock
* Step 3. On mine I also ran fastboot flashing unlock
* flash this image with the `fastboot` utility:
    ```
    $ a-command
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data. Only if boot.img is patched for dm-verity , without patch flashing with TWRP gave verity-fail and phone did not boot

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | working                                                   |
| Speaker / Mic             | working                                                    |
| Bluetooth                 | working                                                   |
| WiFi                      | worning                                                   |
| SIM / Mobile Data / Voice | *working*(2 of 4 installs)                                                 |.          | Working out what order makes it work vs not
| VoLTE                     | unknown                                                    |
| Fingerprint               | untested                                                   |
| NFC                       |  NA                                                    |
| Offline Charging          | Status                                                    |
| Other feature             | Status                                                    |
---

Tested By: MrMazakBlu - Model-, Firmware Versions Blu_v0350WW_v8 .1.03.01-Generic_20-09-1018  - Date tested   1-15-2019