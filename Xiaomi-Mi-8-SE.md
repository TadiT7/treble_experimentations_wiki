# MI 8 SE install GSI AOSP 9 PIE
Note: See https://github.com/phhusson/treble_experimentations/issues/398
## Requirements:
- Bootloader Unlocked
> Note: This is an A-only device.

### a. Installing TWRP recovery 3.2.3 on Xiaomi MI 8 SE
1. Download from [here](https://forum.xda-developers.com/mi-8-se/development/recovery-twrp-recovery-3-2-3-lr-team-t3828854)
2. Flash in to recovery partition with `fastboot flash recovery [PATH TO THE IMAGE FILE YOU DOWNLOADED]` and then `fastboot reboot`

> Note: If TWRP does not start then use combination of buttons `(POWER) + (VOLUME +)` to force the device to start from the recovery 

### b. Installing the latest available version of MIUI 10 EU
1. Download the latest available version of MIUI 10 EU [here](https://sourceforge.net/projects/xiaomi-eu-multilang-miui-roms/files/xiaomi.eu/MIUI-STABLE-RELEASES)
2. Enter `TWRP` and perform `WIPE > FORMAT DATA` and factory reset
3. Copy the ZIP file (MIUI 10) to `DEVICE / TWRP` from the `Windows Explorer` (Drag and Drop)
4. Next go to `INSTALL > INSTALL ZIP`, enter the directory `/data/media/0/TPWR`, flash ZIP file and finish by pressing `SWIPE TO CONFIRM FLASH`
5. Wait for the installation to finish (the system starts in initial MIUI screen)

> Note: I recommend that, even if the device already has a version of MIUI previously installed, the installation process described above **(b)** is carried out to avoid unforeseen results 

### c. Installing GSI AOSP PIE 9
1. Download the latest version of the GSI from this repo
2. Extract the contents of the `.xz` file with 7-zip download [here](https://www.7-zip.org/) 
3. Enter `TWRP` and perform `WIPE > SWIPE TO FACTORY RESET`
4. Copy the IMG file (GSI AOSP) to `DEVICE / TWRP` from the `Windows Explorer` (Drag and Drop)
5. Next go to `INSTALL > IMAGES`, enter the directory `/data/media/0/TWRP`, flash file `IMG` then select partition `SYSTEM IMAGE` and finish by pressing `SWIPE TO CONFIRM FLASH`
6. Restart to `SYSTEM` (Normal restart)
7. Wait for the installation to finish and the system will start the initial screen of `AOSP 9 PIE`

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth media           | Working                                                   |
| Bluetooth in-call         | Not Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not working                                               |
| Fingerprint               | Working                                                   |
| Offline Charging          | Status                                                    |
| Other feature             | Status                                                    |
