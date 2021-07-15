# Cubot King Kong Mini
The device generally works fine. 
Thanks to @highbiker for his tip on rebooting to fastboot, taken from [this XDA forum post](https://forum.xda-developers.com/t/installing-custom-rom-on-cubot-kingkong-mini.4050815/page-9#post-84445303).

I successfully installed and tested the following ROMs, all of them work fine:
* [system-roar-arm32_binder64-ab-gapps.img](https://github.com/phhusson/treble_experimentations/releases) by @phhusson (AOSP 11.0 v309)

## Steps to install

* Enable USB debugging and OEM unlocking in developer options and reboot to bootloader
    ```
    adb reboot bootloader
    ```
* Unlock device
    ```
    fastboot flashing unlock
    ```
* Reboot to fastboot
    ```
    fastboot reboot fastboot
    ```
* flash image
    ```
    fastboot flash system system-roar-arm32_binder64-ab-gapps.img
    ```

## Hardware support

| Component                 |      Comment                                          |
|---------------------------|-------------------------------------------------------|
| Camera                    | OK                                                    |
| Speaker / Mic             | OK                                                    |
| Bluetooth                 | OK                                                    |
| WiFi                      | OK                                                    |
| SIM / Mobile Data / Voice | OK                                                    |
| VoLTE                     | not tested                                            |
| Fingerprint               | N/A                                                   |
| NFC                       | N/A                                                   |
| Offline Charging          | OK                                                    |

## Direct link to OEM Firmware
[CUBOT_KINGKONG_MINI_9101C_V15_20200609](https://mega.nz/file/JdkwFAjL#IK4ANFAr684U89BdkCmuBHyLyyAHLczx3k1o0wB6nSM)

---
Tested By: @idfake - Firmware Version: CUBOT_KINGKONG_MINI_9101C_V15_20200609 - Date tested: 2021-07-15 - Template created by @zguithues and @hackintosh5
