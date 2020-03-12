## Steps to install

* [Unlock bootloader](https://c.realme.com/in/post-details/1101401810746212352).
* [Flash TWRP recovery](https://drive.google.com/file/d/15GAzuSXVo45K7OIaPmTsKhS4DMVXzJeh/view?usp=drivesdk).
* Boot TWRP Recovery, mount vendor, flash [decryption zip](https://drive.google.com/file/d/1--7l9ozoSMGN1C7lADQyNoz3TtQXxoTO/view?usp=drivesdk) (Only required on Android 10 GSIs). 
* Flash any phh based GSI as "System Image".
* Flash permissiver v5 (Only required on Android 10 GSIs).
* Format data and reboot.

## What works and what doesn't

| Functions                 |      Status                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                          |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                         |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Calls | Yes / Yes / Yes                                            |
| VoLTE                     | Not Working                                               |
| Fingerprint               | N/A                                               |
| NFC                       | N/A                                                       |
| Offline Charging          | Working                                                   |
| DT2W & OTG                | Working, need to be enable from phh treble settings.  
| Lockscreen                | Working, need to remove keystore libs from vendor on Android 10.                            |
| Wifi Hotspot              | Working                                                   |
| USB Tethering             | Working                                         |
---

Tested by: Priyam Kalra, Model-CPH1859(India), Firmware Version - C.46, Date tested - 3 March 2020

Template created by @zguithues and @hackintosh5