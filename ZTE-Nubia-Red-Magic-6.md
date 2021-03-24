# Device

AOSP boots, WiFi, cellular data works, sound works

## Steps to install

PWR + VOL+ --> Recovery

PWR + VOL- --> Bootloader

* Unlock bootloader in fastboot mode (`vbmeta.img` and `vbmeta_system.img` are taken from the STOCK ROM, or it will bootloop!):
    ```
    $ fastboot flashing unlock
    $ fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img
    $ fastboot --disable-verification --disable-verity flash vbmeta_system vbmeta_system.img
    ```
    **WARNING: Unlocking will VOID YOUR WARRANTY and make fingerprint UNUSABLE! You may try this to recover fingerprint: https://forum.xda-developers.com/t/guide-for-calibration-finger-print-after-loss-data-calibration.4132961/ WITH STOCK ROM, to see if it worked!**
* Enable ADB from stock ROM
* Enter `fastbootd` mode from adb:
    ```
    $ adb reboot fastboot
    ```
* Or enter `fastbootd` mode from fastboot:
    ```
    $ fastboot reboot fastboot
    ```
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
| VoLTE                     | Not working (China Telecom) (Works with steps in https://github.com/phhusson/treble_experimentations/issues/1681, but not persisted across reboots)                                                    |
| Fingerprint               | Not working                                                    |
| Brightness                | Works without auto brightness (light sensor works) |
| Offline Charging          | Works                                                    |
| Quick Charging            | Works (~5A charging current with stock charger) |
| Fan control               | Works with "Nubia features / FAN speed"                                                    |
| Logo LED                  | Not working |
| RGB LEDs                  | Works with "Nubia features / REDMAGIC RGB" |
| Display Refreshing Rate   | Supports 60/90/120/144/165Hz with "Misc features / Force FPS" |
| Shoulder Buttons          | Not working |
| Side Switch               | Not working |
| Vibration                 | Works |

## Tweaks

| Name | Comment |
|------|---------|
|Rounded corners|Set "Misc features / Set rounded corners diameter" to 30~50 and reboot|

## Notes

1. You can re-lock your bootloader with stock ROM to restore your fingerprint. Backup your persist partition.
2. Nubia is using the test key(external/avb/test/data/testkey_rsa4096.pem) to sign boot, vendor_boot, dtbo and odm partitions. You can create a new `vbmeta.img` with this key from AOSP and keep Magisk with a locked bootloader, also get the working fingerprint.
---

Tested By: notsyncing - NX669J(CN), AOSP 11.0 v302 - 2021/03/12 - Template created by @zguithues and @hackintosh5
