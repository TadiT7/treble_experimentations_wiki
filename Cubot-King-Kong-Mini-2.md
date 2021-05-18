# Cubot King Kong Mini 2
The device generally works fine. The only problem I encountered were occasional instabilities of the WiFi connection: Once or twice a day the WiFi connection dis- and reconnects multiple times. Apart from that, the WiFi connection stays stable.
Thanks to @highbiker for his tip on rebooting to fastboot, taken from [this XDA forum post](https://forum.xda-developers.com/t/installing-custom-rom-on-cubot-kingkong-mini.4050815/page-9#post-84445303).

I successfully installed and tested the following ROMs, all of them work fine:
* [system-roar-arm32_binder64-ab-vanilla.img](https://github.com/phhusson/treble_experimentations/releases) by @phhusson (AOSP 11.0 v307)
* [lineage-18.1-20210512-UNOFFICIAL-treble_a64_bvS.img](https://sourceforge.net/projects/andyyan-gsi/files/lineage-18.x/) by @AndyYan
* [Havoc-OS-v3.8-20200821-Official-a64-ab.img](https://download.havoc-os.com/?dir=a64-ab) (I also tried v4.4 but it didn't boot)

In the end I used lineage-18.1 ([XDA forum thread](https://forum.xda-developers.com/t/gsi-11-lineageos-18-x-gsi-all-archs.4205461/))

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
| WiFi                      | OK (occasionally unstable)                            |
| SIM / Mobile Data / Voice | OK                                                    |
| VoLTE                     | no tested                                             |
| Fingerprint               | N/A                                                   |
| NFC                       | N/A                                                   |
| Offline Charging          | OK                                                    |
| Other feature             | Status                                                |

## Direct link to OEM Firmware
[CUBOT_KINGKONGMINI2_A061C_V07_20201113](https://mega.nz/file/YR9kiCya#iBLECZfQ2JwTVKqm8R4rOjRC8nTg2b6EU45TkeyN-UM)

---
Tested By: @sebastian_de - Firmware Version: CUBOT_KINGKONGMINI2_A061C_V07_20201113 - Date tested: 2021-05-18 - Template created by @zguithues and @hackintosh5
