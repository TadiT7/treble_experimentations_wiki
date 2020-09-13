# Huawei P9
## Project Treble Details
|||
|-----------------|----------| 
| Version         | VNDK 26  | 
| Vendor          | Huawei   |
| Firmware        | EMUI 8.0 |
| O compatibility | Yes      |
| P compatibility | Yes      |
| Q compatibility | Yes      |
| R compatibility | Unknown  |
---

## Feature Status
| Feature                   | Operation state | Comments                                |
|---------------------------|-----------------|-----------------------------------------|
| Bluetooth                 | Working         | Requires flashing                       |
| Camera                    | Working         | Requires flashing                       |
| Face Unlock               | Working         |                                         |
| Fingerprint Sensor        | Working         | Erase fingerprints before factory reset |
| GPS                       | Unknown         | Could not test                          |
| Headphones                | Working         | Requires flashing                       |
| HWComposer                | Working         | Requires flashing for correct behavior  |
| MTP                       | Working         |                                         |
| NFC                       | Working         | Requires flashing                       |
| Offline Charging          | Working         | Requires flashing                       |
| SIM / Mobile Data / Voice | Working         |                                         |
| SD card                   | Working         | Requires flashing for correct behavior  |
| Speaker / Mic             | Working         |                                         |
| VoLTE                     | Unknown         | Could not test                          |
| WiFi                      | Working         |                                         |
---
All the features that say "Requires flashing" can be restored by flashing the ZIPs linked below.

## Installation process for GSIs
### Prerequisites:
- Unlocked bootloader
- Firmware 8.0.0.510 or newer
- Android 10: No Magisk

### TWRP and Encryption: important note
If you didn't follow [this guide](https://forum.xda-developers.com/p9/how-to/guide-easy-decryption-guide-gsi-users-t4115033) to _decrypt your internal storage_ DO NOT factory reset user data using TWRP!** This will break your internal storage! If you need to perform factory reset while maintaining encryption- flash stock Recovery using fastboot and wipe data in it.  

If you will wipe data in TWRP without **decrypting your phone**, your custom ROM will not be able to write to userdata (/data) partition, initial device setup will not finish ever.  

**Decrypted phones CAN factory reset through TWRP!**  

### Installation steps:
* Backup all your internal-storage stuff
* Perform a factory reset
* Flash your GSI image to /system
* Flash the below ZIPs to get correct behavior

### Restoring Camera:
* Flash [this ZIP](https://forum.xda-developers.com/p9/themes/p9-camera-treble-gsi-t4006381) to restore your Camera app and libraries.

### Restoring essential functions:
* Flash [the latest ZIP](https://drive.google.com/drive/folders/1rpCeajjRfozMrTBgSvKELgtb9GwOeXfh). It is highly recommended NOT TO skip this one!

### Google Apps (GApps):
* Flash in TWRP an appropriate package from [OpenGApps](https://opengapps.org/). Choose the correct Android version package for ARM64.