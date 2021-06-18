# Samsung Galaxy A40

Summary of what works and doesn't

## Steps to install

1. Unlock bootloader
2. Install latest firmware version
3. Flash [TWRP](https://twrp.me/samsung/samsunggalaxya40.html)
4. Reboot into TWRP and follow these:
    - Disable file encryption with this [patch](https://4pda.ru/forum/dl/post/17584143/Encrypt.zip)
    - Format Data (you will lose all files)
    - Wipe Davlik, Cache, Data and System
5. Choose a GSI image and flash it in System
6. Reboot to System

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
- AOSP 9/10/11
- Lineage OS 16/17/18.1
- Pixel Experience 9/10/11
- Havoc OS
## Tested by:
- LittleCherryFox
- Iddqd228
- Other guys from 4PDA
# Info
- Model number: A405FM and A405FN
- Latest firmware version: A405FNXXU3CUD3

***

Template created by @zguithues and @hackintosh5 and updated by @ponces