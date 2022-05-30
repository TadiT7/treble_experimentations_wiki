# Huawei P smart 2019 (POT-LX3)
## Requirements for flashing GSI:
* Downgrade to EMUI 9.1.x (see [this guide](https://github.com/ProfessorJTJ/HISuite-Proxy/wiki)).
* Unlock bootloader (**it is a paid service**, click [here](https://hcu-client.com/) for more information).
* After successful bootloader unlock, downgrade to EMUI 9.0 following the guide provided before. **THIS IS AN OBLIGATORY STEP, OTHERWISE WHEN YOU TRY TO FLASH GSI IT WILL TELL YOU THERE'S NOT ENOUGH SPACE AND YOUR PHONE WILL BE BRICKED!**

## Procedure: 
* Get an **arm64-A/B** GSI (it should be 2.6gb or less, otherwise it won't flash)
* Get platform-tools from [this link](https://developer.android.com/studio/releases/platform-tools).
* Get `vbmeta.img` from [this link](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img).
* Reboot to fastboot mode `adb reboot bootloader`.
* Flash the `vbmeta.img` you downloaded executing the following command: 
`fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`
* Flash the GSI you downloaded executing the following command (don't forget to decompress it): `fastboot flash system gsi.img`
* Reboot and enjoy 👍
* As an alternative you can flash via TWRP as "System Image".

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Doesn't works on Android 12.                                                    |
| Speaker / Mic             | ✓                                                    |
| Bluetooth                 | Partially working on Android 12 (can't pair new devices **but** you can transfer files to the phone).                                                     |
| WiFi                      | ✓                                                    |
| SIM / Mobile Data / Voice | need test                                                    |
| VoLTE                     | need test                                                    |
| Fingerprint               | ✓                                                    |                                         |
| Offline Charging          | Not working                                                    |
| Other feature             | Status                                                    |
---
# 
Tested by Angel Castillo :)