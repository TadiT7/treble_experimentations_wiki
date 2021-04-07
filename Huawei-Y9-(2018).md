# Huawei Y9 (2018)

Tested both Android 10 and 11 (FLA-LX3). So far the only issue has been 'adoptable storage' on Android 10, which caused the device to reboot and hang. It will boot if manually turned off but will hang on 'loading phone...'
SD as 'external storage' seems to be working fine.

Bluetooth address will show as 'unavailable' on Android 11, aside from that it works alright.

This device has 2 cameras/lens/sensors on each side, yet only one of them on each side is recognised by the OS, both on Android 10/11. I have not been able to find a solution for this.

## Requirements

* As of 2020, thanks to mashed-potatoes, this device can be unlocked through [PotatoNV](https://github.com/mashed-potatoes/PotatoNV/wiki/How-to-use-PotatoNV), please refer to the instructions in that git repository.

(This guide will assume you have installed, or know how to install and use, ADB and Fastboot. Please search for a guide on how to do this depending on your OS)

- ADB and Fastboot
- AOSP PHH ROM (others could work but this is the one I have tested) - unzip the xz file to obtain the img file.
- **Important** use the A/B partition style, as it will not boot on A-only!
- **Keep in mind that on Android 11, [the system partition mounts as read only](https://github.com/phhusson/treble_experimentations/issues/1613#issuecomment-741897195).** Yet, if you need to remove 'root/super su' (for example, for 'basicIntegrity / SafetyNet' reasons), you will need to mount the '/system' partition as r/w. Although the 'vndk-lite' version is r/w, I was not able to write it on the device due to what I reckon is 'storage/partition space issues'. [Partition resizing might be a solution](https://github.com/phhusson/treble_experimentations/issues/1732) yet I have not tried this, nor will do in the foreseeable future. Moreover, I was not able to mount the system partition as r/w through TWRP-3.5.1 (P20 lite version).
- **This will delete all your data. Do a back up before starting this process.**
- **Also important** The device was on EMUI 9.1 prior unlocking it and flashing these ROMs.

## Steps to install

1. After unlocking the bootloader, enable 'developer options' by tapping 7 times on the build number.
2. Inside 'developer options' enable 'oem unlock' and 'USB debugging'. Connect your device to your computer and allow debugging on your phone.
3. Open a terminal window and type `adb devices` on to check your phone is properly connected. Then type 'adb reboot bootloader' to boot in fastboot mode.
4. Once in fastboot mode, type `fastboot flash system system-arm64-aonly-gapps-su.img`. Replace `system system-arm64-aonly-gapps-su.img` with the name of the .img file you have downloaded. You could drag and drop the file on the terminal.
5. Once it is done writing the .img, type `fastboot reboot` to exit fastboot mode.
6. Enter 'eRecovery' by pressing the volume up button for 3 seconds when the yellow warning appears.
7. On 'eRecovery' select 'Wipe data/factory reset', type yes and confirm.
8. It will boot into 'recovery' and wipe the data. Reboot. (Stock recovery is required!)


## Hardware support

Android 10

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working / only one lens in each side                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not tested                                                |
| Fingerprint               | Working                                                   |
| NFC                       | Not tested                                                |
| Offline Charging          | Working                                                   |
| Micro SD         | Working as external storage only / adoptable storage does not work!|

Android 11

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working / only one lens in each side                                                  |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not tested                                                |
| Fingerprint               | Working                                                   |
| NFC                       | Not tested                                                |
| Offline Charging          | Working                                                   |
| Micro SD         | Only tested as external storage |

---

Tested By: arturoguzmanp - FLA-LX3(Latam), From EMUI 9.1 to Android 10/11 - 7th April 2021 - Template created by @zguithues and @hackintosh5