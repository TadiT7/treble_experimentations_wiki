# Huawei Mate 10 (alp)

EMUI8 base - A only ROM - works up to Android 9 Pie

EMUI9 base - AB ROM

## Steps to install

* Step 1
Reboot to fastboot
* Step 2
    flash the image with the `fastboot` utility:
    ```
    $ fastboot flash system system-quack-arm64-ab-vanilla.img
    ```
* Step 3
Unplug from USB. Press and hold volume up + power to boot into EMUI recovery
* Step 4
Perform a factory reset in the EMUI recovery
* Step 5
Reboot

## Hardware support

EMUI8 base with v123 system-arm64-aonly-vanilla-nosu.img
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | AOSP camera Works, Huawei camera app does not work        |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works                                                    |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Unknown                                                    |
| Fingerprint               | Not working                                                    |
| NFC                       | Works                                                    |
| Offline Charging          | Unknown                                                    |

EMUI9 base with v222 system-quack-arm64-ab-vanilla.img
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works        |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works                                                    |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Unknown                                                    |
| Fingerprint               | Works                                                    |
| NFC                       | Works                                                    |
| Offline Charging          | Unknown                                                    |

EMUI9 base with v300.l system-roar-arm64-ab-vanilla.img
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works        |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works                                                    |
| WiFi                      | Works|
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Unknown                                                    |
| Fingerprint               | Works                                                    |
| NFC                       | Works                                                    |
| Offline Charging          | Unknown                                                    |

EMUI9 base with Android 12 v400.a system-squeak-arm64-ab-vndklite-floss.img
|Component | Comment|
|---|---|
|Camera | Not Working|
|Speaker / Mic | Works |
|WiFi | Works|
| SIM / Voice | Works|
|Mobile Data | Not Working|
|VoLTE | Unknown|
|Fingerprint | Works|
|NFC|Works|
|Offline Charging|Works|

---

Tested By: @mingyech - ALP-L29, EMUI8 Base: ALP-L29C636B143 (8.0.0.143) v218575, EMUI9 base: ALP-L29C636E2R1P12B159 (9.0.0.159) - Dec 03 2020 - Template created by @zguithues and @hackintosh5