# Device

Overall useable. This device is misreported as A-only in some utilities. Use the AB image for it, or it will bootloop. 

## Steps to install

* Step 1 - unlock your bootloader by enabling **OEM unlocking** in developer settings
* Step 2 - Reboot to DOWNLOAD mode. On the warning about flashing ROMs hold down the volume up button
* Step 3 - Downgrade to Android 11, OneUI 3.1
* Step 4 - **IMPORTANT!** Setup phone, connect to the internet and wait 15 minutes. If this is skipped you'll be in PRENORMAL state and you will not be able to flash TWRP.
* Step 5 - Flash the modified TWRP image, you'll find it on the internet. It'll have november in the file name.
* Step 6 - Download and extract the **AB image**. Flash using TWRP, do a standard wipe
* Step 7 - Boot! It may take a little longer than normal and it may appear as if it's stuck on the "Note20 Ultra" screen. Be patient!

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Only one of the back cameras is working (middle) Front camera works fine   |
| Speaker / Mic             | Working                                                                    |
| Bluetooth                 | Working                                                                    |
| WiFi                      | Working                                                                    |
| SIM / Mobile Data / Voice | Working, mobile data can be a little stubborn, turn it off and on to fix   |
| VoLTE                     | Not working                                                                |
| Fingerprint               | Not working                                                                |
| NFC                       | Working                                                                    |
| Offline Charging          | Working albeit slowly                                                      |
| Other feature             | Battery seems to lose charge faster than factory, still usable. SPen works.|
---

Tested By: thenxguy - SM-N986B (POLAND), Firmware Version - v402, Date tested 3/10/2022, Template created by @zguithues and @hackintosh5