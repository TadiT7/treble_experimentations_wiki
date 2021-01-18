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
| Camera                    | Y                                                         |
| Speaker / Mic             | Y                                                         |
| Bluetooth                 | Y                                                         |
| WiFi                      | Y                                                         |
| SIM / Mobile Data / Voice | Y                                                         |
| VoLTE                     | Y                                                         |
| Fingerprint               | Y                                                         |
| Flashlight                | Y                                                         |
| NFC                       | Status                                                    |
| Offline Charging          | Status                                                    |
---

Tested By: surya580 on firmware 94 with system-roar-arm64-ab-gapps.img.xz (300.l) on 18th January 2021