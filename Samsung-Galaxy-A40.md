# Samsung Galaxy A40

Summary of what works and doesn't

## Steps to install

* Step 1 - unlock bootloader
* Step 2 - install latest firmware version
* Step 3 - flash [TWRP](https://twrp.me/samsung/samsunggalaxya40.html)
* Step 4 - reboot into TWRP and follow these:
- Disable encrypt with this [patch](https://4pda.ru/forum/dl/post/17584143/Encrypt.zip)
- Format Data (you will lose all files)
- Wipe Davlik, Cache, Data and System
* Step 5 - choose a GSI image and flash it in System
* Step 6 - reboot

## Hardware support

## Android 11
| Component                 |      Works?                                               |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Yes                                                       |
| Speaker / Mic             | Yes                                                       |
| Bluetooth                 | Yes                                                       |
| WiFi                      | Yes                                                       |
| SIM / Mobile Data / Voice | Yes                                                       |
| VoLTE                     | No                                                        |
| Fingerprint               | Yes                                                       |
| NFC                       | Yes                                                       |
| Offline Charging          | No                                                        |
| MTP/PTP                   | Kernel dependent                                          |
| Bluetooth calls           | Yes                                                       |
---

## Android 10
| Component                 |      Works?                                               |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Yes                                                       |
| Speaker / Mic             | Yes                                                       |
| Bluetooth                 | Yes                                                       |
| WiFi                      | Yes                                                       |
| SIM / Mobile Data / Voice | Yes                                                       |
| VoLTE                     | No                                                        |
| Fingerprint               | Yes                                                       |
| NFC                       | Yes                                                       |
| Offline Charging          | No                                                        |
| MTP/PTP                   | Kernel dependent                                          |
| Bluetooth calls           | No                                                        |
---

## Android Pie
| Component                 |      Works?                                               |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Yes                                                       |
| Speaker / Mic             | Yes                                                       |
| Bluetooth                 | Yes                                                       |
| WiFi                      | Yes                                                       |
| SIM / Mobile Data / Voice | Yes                                                       |
| VoLTE                     | No                                                        |
| Fingerprint               | Yes                                                       |
| NFC                       | Yes                                                       |
| Offline Charging          | No                                                        |
| MTP/PTP                   | Kernel dependent                                          |
| Bluetooth calls           | No                                                        |
---
## Tested GSI's
AOSP 9/10/11, Lineage OS 16/17/18.1, Pixel Experience 9/10/11, Havoc OS.
## Tested by:
LittleCherryFox, Iddqd228 and other guys from 4PDA 
# Info
- Model number: A405FM and A405FN
- Latest firmware version: A405FNXXU3CUD3
Template created by @zguithues and @hackintosh5 and updated by @ponces