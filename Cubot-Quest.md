# Cubot QUEST

## GSI AOSP 9
GSI AOSP 9 Rom works very well and smooth (all version)

Issues in TWRP, touchscreen doesn't work at all

### Steps to install

* Enable USB Debugging and OEM Unlock

 ```
$ adb reboot bootloader
$ fastboot flashing unlock
 ```

* Now press Vol+ to confirm unlocking
 ```
$ fastboot -w (will erase all data)
$ fastboot flash system GSIimagefile.img
$ fastboot reboot
 ```

* optional nano-openGapps - after first boot
 ```
$ adb reboot recovery
$ adb shell twrp sideload
$ adb sideload nanoOpenGappsFile.zip
$ adb reboot bootloader
$ fastboot erase userdata
$ fastboot -w
$ fastboot reboot
 ```

If anyone could help me making touchscreen works, I think this could be flashed also from TWRP

### Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Seems OK                                                  |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | N/A                                                       |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | N/A                                                       |
| Fingerprint               | OK                                                        |
| NFC                       | N/A                                                       |
| Offline Charging          | OK                                                        |
| Extra button              | Not working at all                                        |
---

## Havoc 2.9, based on AOSP 9 GSI
 Mobile Internet. It works for 30 minutes than it stops. Rebooting will restart Mobile Internet for other 30 minutes.

## GSI AOSP 10

GSI AOSP 10 Rom stucks on initial boot after following the same instruction of AOSP 9 GSI


Tested By: bahamut657 - Cubot-Quest(IT), Firmware Version AOSP 9 GSI- Date tested 2020/03/12 - Template created by @zguithues and @hackintosh5
