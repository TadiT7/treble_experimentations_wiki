# Device

Summary of what works and doesn't

## Steps to install

* Flash [TWRP](https://www.androidfilehost.com/?w=files&flid=335166) as AP and [VBMETA Disabler](https://forum.xda-developers.com/attachments/vbmeta_disabled_r-tar.5236537/?hash=f7249adaefe16f3aeac3256a63063f0a) as USERDATA with Odin.

* Reboot to recovery via recovery key combo (Vol up + power + USB connected).

* Open TWRP Terminal, execute "multidisabler" command, then go to Wipe > Format Data > Yes and reboot recovery.

* [ADB](https://developer.android.com/studio/releases/platform-tools) Push [this kernel zip](https://www.androidfilehost.com/?w=files&flid=335167) to /sdcard

* Flash the pushed ZIP (GSI won't boot without it.)

* Flash any GSI image as system image in TWRP, then reboot system and enjoy.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Depends on GSI                                            |
| VoLTE                     | Not Working                                               |
| Fingerprint               | Not Working                                               |
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| 5G                        | Depends on GSI                                            |
| 120Hz Refresh Rate        | Working                                                   |
---

Tested By: ItsLynix - SM-A536B(EUX), A536BXXU4BVJG - 28/11/2022 - Template created by @zguithues and @hackintosh5
