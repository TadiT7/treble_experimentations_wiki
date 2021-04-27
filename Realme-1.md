## Steps to install

* Unlock [bootloader](https://c.realme.com/in/post-details/1101401810746212352).
* Flash [TWRP recovery](https://realmeone.glitch.me/TWRP).
* Boot to the TWRP Recovery, mount vendor, flash [Decryption zip](https://t.me/Realme1Community/393605) (Only required on Android 10 GSIs). 
* Flash any phh based GSI as "System Image".
* Flash [permissiver v5](https://t.me/Realme1Community/270720) (Only required on Android 10 GSIs).
* Format data and reboot.

## What works and what doesn't

| Functions                 |      Status                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                          |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                         |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Calls | Yes / Yes / Yes                                            |
| VoLTE                     | Working, Need to install ims apk and request ims from treble app                                         |
| ViLTE                     | Working                                            |
| VoWIFI                    | Working                                            |
| Fingerprint               | N/A                                               |
| NFC                       | N/A                                                       |
| Offline Charging          | Working                                                   |
| DT2W & OTG                | Working, need to be enable from phh treble settings.  
| Lockscreen                | Working, need to remove keystore libs from vendor on Android 10/R                          |
| Wifi Hotspot              | Working                                                   |
| USB Tethering             | Working                                         |
---

Tested by: Priyam Kalra, CyberJalagam,
Model-CPH1859/CPH1861(India),
Firmware Version - C.49,
Date tested - 27 April 2021

Template created by @zguithues and @hackintosh5