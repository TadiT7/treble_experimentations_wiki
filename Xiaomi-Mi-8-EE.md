# Device

Mi8EE (URSA)

# Tested Image
AOSP 10.0 v220/v221

## Steps to install
* Unlock bootloader
* flash this image with the `fastboot` utility:
    ```
    $ fastboot erase system
    $ fastboot flash system system-quack-arm64-ab-gapps.img
    $ fastboot -w (wipe userdata)
    $ fastboot reboot
    ```
    Some more info

    Fix for Type c audio output -> Fixed by enable "using alternate audio policy" in phh setting->qualcomm feauture
    Fix for Media sound-> Fixed by enable "disable audio effects" in phh setting -> misc features

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work                                                      |
| Speaker / Mic             | Work                                                      |
| Bluetooth                 | Work(except Bluetooth media audio)                        |
| WiFi                      | Work                                                      |
| SIM / Mobile Data / Voice | Work                                                      |
| VoLTE                     | Work, flash https://github.com/KhushrajRathod/VoLTE-Fix   |
| Fingerprint               | work, need miui12 image                                   |
| NFC                       | Not tested                                                |
| Offline Charging          | Work                                                      |
| Volume scale              | Not display correctly                                     |

