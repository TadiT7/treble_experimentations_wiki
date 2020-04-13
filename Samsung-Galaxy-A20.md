# Samsung Galaxy A20

Some of this was taken from [this page.](https://forum.xda-developers.com/galaxy-a20/how-to/gsi-galaxy-a20-t3964546) Please thank [physwizz](https://forum.xda-developers.com/member.php?u=5440376) and not me!
## Steps to install
* Step 0 - Make a backup if what you have on your device is important!
* Step 1 - Make sure you wipe both caches, system and data.
* Step 2 - Unzip the .IMG file and somehow copy it to your device.
* Step 3 - Install the .IMG file as a "System Image"
* Step 4 - Reboot to recovery (remember to do this!)
* Step 5 - [Install Modded Magisk by ianmacd](https://forum.xda-developers.com/attachment.php?attachmentid=4850993&d=1571653427)
* Step 6 - [Install Disable_Dm-Verity_ForceEncrypt](https://forum.xda-developers.com/attachment.php?attachmentid=4850995&d=1571653427)
* Step 7 - [Install Permissiver_v5](https://forum.xda-developers.com/attachment.php?attachmentid=4850997&d=1571653427)
* Step 8 - If you have gapps installed already, skip the next few steps and reboot now.
* Step 9 - Resize the system partition by doing
- Wipe then advanced wipe
- Select the system partition and hit repair or change file system
- Hit resize file system
- If it erorrs out, do it again and it should work.
- Flash gapps and clear the caches and reboot!


## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Yes, but not the 2nd camera                               |
| Speaker / Mic             | Yes                                                       |
| Bluetooth                 | Yes                                                       | 
| WiFi                      | Yes                                                       |
| SIM / Mobile Data / Voice | Yes                                                       |
| VoLTE                     | Not with me                                               |
| Fingerprint               | Yes                                                       |
| NFC                       | N/A                                                       |
| Offline Charging          | N/A                                                       |
---
## If you have problems
* 1. Launcher keeps crashing.
This happened to me and it might happen to you. I haven't tested the latest build but I will later. What you need to do is download gapps and flash it This will put the navigation bar gestures back and you can use the pixel launcher.
* 2. Settings app keeps crashing.
I haven't found a fix to this problem yet. I'll keep searching.


Tested By: os54656 - SM-205G , Firmware Version - treble_arm64_bgS-userdebug 10 QQ2A.200305.003 200314 test_keys - I think it is v214 Date tested - 2020-04-13 Template created by @zguithues and @hackintosh5