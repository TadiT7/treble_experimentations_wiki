# Samsung Galaxy A51

Summary of what works and doesn't
# Works
- WiFi
- Always on display availability
- Dual sim
- Correct status bar height, punchhole, and rounded corners
- SDCard as Portable Storage

## Doesn't work (from what I've tested)
- VoLTE
- Macro Camera
- Lower megapixels on cameras
- Fingerprint


## Steps to install

* Step 1: Download & Install TWRP [this guide](https://forum.xda-developers.com/t/installing-twrp-and-root-for-samsung-galaxy-a51-with-video.4212205/), if the TWRP provided boot loops after flashing GSI, try [this version](https://t.me/dev_yilliee/145)
* Step 2: Download dynapatch [here](https://t.me/dev_yilliee/125), disable-dm-verity [here](https://drive.google.com/file/d/1mZeg-ZgrUGqWo_Y0Q2nNcINx-WURBTGg/view?usp=sharing), and a GSI from [probably here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)
* Step 3: Flash dynapatch in twrp to map super partitions and reboot recovery, flash dm-verity-disabler, then flash the gsi image as "system image" 
* Step 4: Reboot System, enjoy.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working, except Macro                                     |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not Working                                               |
| Fingerprint               | Not Working                                               |
| NFC                       | Working                                                   |
---

Tested By: ItsLynix - SM-A515F(NEE), A515FXXU5EUJ4 - 7/12/2021
Template created by @zguithues and @hackintosh5