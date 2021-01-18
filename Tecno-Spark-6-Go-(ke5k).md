# Device

Tecno Spark 6 Go is a phone that was launched on 22nd December 2020. The phone comes with a 6.52-inch touchscreen display, Helio A22 and a 5000 mAh battery.

## Steps to install

* Reboot to bootloader/fastboot mode
* Unlock bootloader with `fastboot flashing unlock`
* Reboot to recovery and select enter fastboot (not bootloader)
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-roar-arm64-ab-vanilla.img
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Status                                                    |
| Speaker / Mic             | Status                                                    |
| Bluetooth                 | Status                                                    |
| WiFi                      | Y                                                    |
| SIM / Mobile Data / Voice | Y                                                    |
| VoLTE                     | Y                                                    |
| Fingerprint               | Status                                                    |
| NFC                       | Status                                                    |
| Offline Charging          | Status                                                    |
---

Tested By: surya580 - Firmware: 94 - 18/01/2021