# Samsung Galaxy A51

Summary of what works and doesn't
# Works
- Bluetooth
- WiFi
- Always on display availability
- Dual sim
- Correct status bar height, punchhole, and rounded corners
- SDCard as Portable Storage
- Fingerprint (As of v400.e)

## Doesn't work (from what I've tested)
- VoLTE
- Lower megapixels on cameras

# Bluetooth issues
If you are experiencing crashes when Bluetooth is connected on certain GSIs, please disable media recommendations.

## Steps to install

* Step 1: Download & Install TWRP [this guide](https://forum.xda-developers.com/t/installing-twrp-and-root-for-samsung-galaxy-a51-with-video.4212205/) if the TWRP provided boot loops after flashing GSI, try [this updated version](https://t.me/dev_yilliee/145)
* Step 2: Download dynapatch [here](https://t.me/dev_yilliee/125), disable-dm-verity [here](https://drive.google.com/file/d/1mZeg-ZgrUGqWo_Y0Q2nNcINx-WURBTGg/view?usp=sharing), and a GSI from [probably here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)
* Step 3: Flash dynapatch in twrp to map super partitions and reboot recovery, flash dm-verity-disabler, then flash the gsi image as "system image" 
* Step 4: Reboot System, enjoy.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                     |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working, 5 & 2.4 GHz                                      |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not Working                                               |
| Fingerprint               | Working                                             |
| NFC                       | Working                                                   |
---

Tested By: ItsLynix - SM-A515F(NEE), A515FXXU5EUJ4 - 7/12/2021
Updated By: Yillié - A515FXXU5EUG2 - 16/12/2021

Note: The availability of other camera sensors ( Macro, Wide-Angle and Depth sensor ) depends on the camera app you're using. You can access the extra sensors using a camera app that supports multiple sensors ( for example open camera ).

Template created by @zguithues and @hackintosh5