# Device

Mi10 (UMI)

# Tested Image
AOSP 10.0 v220

## Steps to install
* Unlock bootloader
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash recovery stock-recovery.img (using official miui recovery)
    $ fastboot reboot fastboot
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
| VoLTE                     | Didn't test                                               |
| Fingerprint               | Not work                                                  |
| NFC                       | Work                                                      |
| Offline Charging          | Work                                                      |
| 90hz screen               | Not work                                                  |
| Volume scale              | Not display correctly                                     |
| 5G                        | Didn't test                                               |
---

Tested By: yukikwi - Mi 10(global), Based on xiaomi.eu 20.6.18 - 2020/07/03 - Template created by @zguithues and @hackintosh5
