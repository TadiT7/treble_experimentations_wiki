# Cubot King Kong Mini 2
The device generally works fine.
Thanks to @highbiker for his tip on rebooting to fastboot, taken from [this XDA forum post](https://forum.xda-developers.com/t/installing-custom-rom-on-cubot-kingkong-mini.4050815/page-9#post-84445303).

I successfully installed and tested the following ROMs, all of them work fine:
* [system-squeak-arm32_binder64-ab-vanilla.img](https://github.com/phhusson/treble_experimentations/releases) by @phhusson (AOSP 12.0 v402)
* [lineage-18.1-20210512-UNOFFICIAL-treble_a64_bvS.img](https://sourceforge.net/projects/andyyan-gsi/files/lineage-18.x/) by @AndyYan
* [Havoc-OS-v3.8-20200821-Official-a64-ab.img](https://download.havoc-os.com/?dir=a64-ab) (I also tried v4.4 but it didn't boot)

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
    fastboot flash system system-roar-arm32_binder64-ab-vanilla.img
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

## Issues
* Call echoing when using a bluetooth headset. (AOSP 11 v309)
* Link negotiation fails for WPA3-enabled wifi networks ([fix](https://github.com/phhusson/device_phh_treble/commit/a4d6f5c8d35b61304c8e8dae0e68d243d39e7324))

## Direct link to OEM Firmware
[CUBOT_KINGKONGMINI2_A061C_V07_20201113](https://mega.nz/file/YR9kiCya#iBLECZfQ2JwTVKqm8R4rOjRC8nTg2b6EU45TkeyN-UM)

---
Tested By: @sebastian_de - Firmware Version: CUBOT_KINGKONGMINI2_A061C_V07_20201113 - Date tested: 2021-06-14 - Template created by @zguithues and @hackintosh5
