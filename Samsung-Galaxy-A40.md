# Samsung Galaxy A40

Summary of what works and doesn't

## Steps to install

* Step 1 - Unlock Bootloader
* Step 2 - Install frimware version ASJ1 (temporarily)
* Step 3 - Flash TWRP (https://4pda.ru/forum/dl/post/18167443/recovery.tar) By Ponces
* Step 4 - Reboot into TWRP and follow these points
- Format DATA (lost all files)
- Do Wipe these points(Davlik/ART,Cache,Cache,Data,System)
- Disable Encrypt by this patch (https://4pda.ru/forum/dl/post/17584143/Encrypt.zip)
* Step 5 - Choose GSI and flash it into System partion
* Step 6 - Reboot into TWRP and follow these points
- Mount - System
- Wipe - Advanced Wipe - System - Repair or Change File System - Resize File System - Swipe
* Step 7 - Flash Magisk

## Hardware support

## Android Q
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work                                                      |
| Speaker / Mic             | Work                                                      |
| Bluetooth                 | Work                                                      |
| WiFi                      | Work                                                      |
| SIM / Mobile Data / Voice | Work                                                      |
| VoLTE                     | ?                                                         |
| Fingerprint               | Work                                                      |
| NFC                       | Work                                                      |
| Offline Charging          | Not work                                                  |
| MTP/PTP                   | Not work(Reboot to TWRP and Enable MTP)                   |
| Bluetooth calls           | Not work                                                  |
| Other feature             | Work                                                      |
---

## Android Pie
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work                                                      |
| Speaker / Mic             | Work                                                      |
| Bluetooth                 | Work                                                      |
| WiFi                      | Work                                                      |
| SIM / Mobile Data / Voice | Work                                                      |
| VoLTE                     | ?                                                         |
| Fingerprint               | Work                                                      |
| NFC                       | Work                                                      |
| Offline Charging          | Not work                                                  |
| MTP/PTP                   | Work(?)                                                   |
| Bluetooth calls           | Not work                                                  |
| Other feature             | Work                                                      |
---
Tested GSI's - Lineage OS 16/17,AOSP 9/10,Piexl Expirience 9/10,Havoc OS.
Tested By: LittleCherryFox,Iddqd228 and other guys from 4PDA - Model-Number(A405-FM,A405-FN), Firmware Version A405XXXXU2ASJ1 - Date tested - December 2019  Template created by @zguithues and @hackintosh5