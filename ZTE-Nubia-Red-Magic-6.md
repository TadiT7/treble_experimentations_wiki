# Device

AOSP boots, WiFi, cellular data works, sound works

## Steps to install

PWR + VOL+ --> Recovery

PWR + VOL- --> Bootloader

* Unlock bootloader in fastboot mode:
    ```
    $ fastboot flashing unlock
    ```
    **WARNING: Unlocking will VOID YOUR WARRANTY and make fingerprint UNUSABLE! You may try this to recover fingerprint: https://forum.xda-developers.com/t/guide-for-calibration-finger-print-after-loss-data-calibration.4132961/ WITH STOCK ROM, to see if it worked!**
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
| Headphone                 | Not working |
| USB DAC                   | Works |
| Type-C DP Alt mode        | Works |
| GPS                       | Works |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works (may not see 5G wifi at the first time)                                            |
| SIM / Mobile Data / Voice | Works                                                    |
| Tethering                 | Not working |
| Proximity Sensor          | Works |
| Accelerometer / Gyroscope | Works |
| VoLTE                     | Not working (China Telecom)                                                    |
| Fingerprint               | Not working                                                    |
| Brightness                | Works without auto brightness (light sensor works) |
| Offline Charging          | Works                                                    |
| Quick Charging            | Not tested |
| Fan control               | Works with "Nubia features / FAN speed"                                                    |
| Logo LED                  | Not working |
| RGB LEDs                  | Works with "Nubia features / REDMAGIC RGB" |
| Display Refreshing Rate   | Supports 60/90/120/144/165Hz with "Misc features / Force FPS" |
| Shoulder Buttons          | Not working |
| Side Switch               | Not working |

## Tweaks

| Name | Comment |
|------|---------|
|Rounded corners|Set "Misc features / Set rounded corners diameter" to 30~50 and reboot|
---

Tested By: notsyncing - NX669J(CN), AOSP 11.0 v302 - 2021/03/12 - Template created by @zguithues and @hackintosh5
