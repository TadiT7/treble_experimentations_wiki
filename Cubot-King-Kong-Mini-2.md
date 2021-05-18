# Cubot King Kong Mini 2
The device generally works fine. The only problem I encountered were occasional instabilities of the WiFi connection: Once or twice a day the WiFi connection dis- and reconnects multiple times. Apart from that, the WiFi connection stays stable.
Thanks to @highbiker for his tip on rebooting to fastboot, taken from [this XDA forum post](https://forum.xda-developers.com/t/installing-custom-rom-on-cubot-kingkong-mini.4050815/page-9#post-84445303).

I successfully installed and tested the following ROMs, all of them work fine:
* system-roar-arm32_binder64-ab-vanilla.img by @phhusson (AOSP 11.0 v307)
* lineage-18.1-20210512-UNOFFICIAL-treble_a64_bvS.img by @AndyYan

## Steps to install

* Enable USB debugging and reboot to bootloader
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

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                    |
| Speaker / Mic             | OK                                                    |
| Bluetooth                 | OK                                                    |
| WiFi                      | OK (occasionally unstable)                                                    |
| SIM / Mobile Data / Voice | OK                                                    |
| VoLTE                     | no tested                                                    |
| Fingerprint               | N/A                                                    |
| NFC                       | N/A                                                    |
| Offline Charging          | OK                                                    |
| Other feature             | Status                                                    |

## Direct link to OEM Firmware
[CUBOT_KINGKONGMINI2_A061C_V07_20201113](https://mega.nz/file/YR9kiCya#iBLECZfQ2JwTVKqm8R4rOjRC8nTg2b6EU45TkeyN-UM)

---
Tested By: @sebastian_de - Firmware Version: CUBOT_KINGKONGMINI2_A061C_V07_20201113 - Date tested: 2021-05-18 - Template created by @zguithues and @hackintosh5
