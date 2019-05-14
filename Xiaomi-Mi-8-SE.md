# MI 8 SE install GSI AOSP 9 PIE phhson
Note: See https://github.com/phhusson/treble_experimentations/issues/398
> Note: This is an A-only device.
### Required files
0. Official bootloader unlocker http://miuirom.xiaomi.com/rom/u1106245679/3.3.1212.33/miflash_unlock-3.3.1212.33.zip
1. Stock fastboot mode latest stable firmware http://update.miui.com/updates/v1/fullromdownload.php?d=sirius&b=X&r=cn&n= . With this, you can go back to stock at anytime if something goes wrong.
2. Stock fastboot mode firmware flashing tool http://bigota.d.miui.com/tools/MiFlash2018-5-28-0.zip
3. LR.team 2019-04-23 unofficial TWRP 3.3.0 with flashing tool https://mailacid-my.sharepoint.com/:u:/g/personal/tsh_mail_ac_id/EXVUGoX4qLlDiXms2ZJDCG0BfZWRfvp5rwNVHavhsz9IYw?e=TgYdHk
4. Latest stable xiaomi.eu ROM. Same version as the downloaded stock firmware recommended. https://sourceforge.net/projects/xiaomi-eu-multilang-miui-roms/files/xiaomi.eu/MIUI-STABLE-RELEASES
5. phhson AOSP systemimg for arm64 A-only devices https://github.com/phhusson/treble_experimentations/releases
6. Following procedure is executed under Windows
### 0. Unlock bootloader
1. Unlock the bootloader here http://en.miui.com/unlock/
### a. Installing TWRP recovery 3.3.0 on Xiaomi MI 8 SE
1. Extract the downloaded file.
2. Run recovery-twrp-one-click-flashing-tool一键刷入.bat
3. Follow the instructions

> Tip: If TWRP does not start then use combination of buttons `(POWER) + (VOLUME +)` to force the device to start from the recovery 

### b. Installing the latest available version of MIUI EU
1. Enter `TWRP` and perform `WIPE > FORMAT DATA` and factory reset
2. Copy the ZIP file (MIUI 10) to `DEVICE / TWRP` from the `Windows Explorer` (Drag and Drop)
3. Next go to `INSTALL > INSTALL ZIP`, enter the directory `/data/media/0/TPWR`, flash ZIP file and finish by pressing `SWIPE TO CONFIRM FLASH`
4. Wait for the installation to finish (the system starts in initial MIUI screen)

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
| Bluetooth in-call         | Not Working                                               |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not working                                               |
| Fingerprint               | Working                                                   |
| Offline Charging          | Status                                                    |
| Other feature             | Status                                                    |
