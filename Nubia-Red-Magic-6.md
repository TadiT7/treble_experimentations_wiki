# Device

AOSP boots, WiFi, cellular data works, sound works

## Steps to install

PWR + VOL+ --> Recovery

PWR + VOL- --> Fastboot

* Unlock bootloader in fastboot mode:
    ```
    $ fastboot flashing unlock
    ```
* Enable ADB from stock ROM
* Enter `fastbootd` mode from adb:
    ```
    $ adb reboot fastboot
    ```
    > This device is unable to enter `fastbootd` mode by `fastboot reboot fastboot`!
* Flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-roar-arm64-ab-vanilla.img
    ```
* Reboot (or wipe device from stock recovery)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                     |
| Speaker / Mic             | Works with "Qualcomm features / Use alternative audio policy"                                |
| Headphone                 | Not tested |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works (may not see 5G wifi at the first time)                                            |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Not working (China Telecom)                                                    |
| Fingerprint               | Not working                                                    |
| Offline Charging          | Works                                                    |
| Fan control               | Works with "Nubia features / FAN speed"                                                    |
| Logo LED                  | Not working |
| RGB LEDs                  | Works with "Nubia features / REDMAGIC RGB" |
| Display Refreshing Rate   | Supports 60/90/120/144/165Hz with "Misc features / Force FPS" |
---

Tested By: notsyncing - NX669J(CN), Firmware Version - 2021/03/12 - Template created by @zguithues and @hackintosh5
