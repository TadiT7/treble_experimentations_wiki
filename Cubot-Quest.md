# Cubot QUEST

## TWRP 
Issues in TWRP, touchscreen doesn't work at all

**If anyone could help me making touchscreen works, I think this could be flashed also from TWRP**

## GSI AOSP 9
GSI AOSP 9 ROM works very well and smooth (all version). The only issue is Mobile Internet. 
It works for 1 hour than it stops. Rebooting will restart Mobile Internet for other hour.

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



### Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Seems OK                                                  |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | N/A                                                       |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK Voice, Mobile data works for max 1 hour                |
| VoLTE                     | N/A                                                       |
| Fingerprint               | OK                                                        |
| NFC                       | N/A                                                       |
| Offline Charging          | OK                                                        |
| Extra button              | Not working at all                                        |
---

 

## GSI AOSP 10

GSI AOSP 10 ROM works very well and smooth (all version). 


### Steps to install

* Enable USB Debugging and OEM Unlock

 ```
$ adb reboot bootloader
$ fastboot flashing unlock
 ```

* Now press Vol+ to confirm unlocking
 ```
$ fastboot -w (will erase all data)
$ fastboot flash boot <STOCKBOOT.img>
$ fastboot flash system GSIimagefile.img
$ fastboot --disable-verity --disable-verification flash vbmeta <VBMETA.img>
$ fastboot reboot
 ```

* optional nano-openGapps - after first boot (flashing from TWRP with adb - because the touchscreen doesn't work for me)
* after the first reboot the ROM says that the device is encrypted, reboot again in fastboot and perform ```fastboot -w``` (or simply press factory reset if the ROM permits it)
### Hardware support

| Component                 |      Comment                                                                              |
|---------------------------|-------------------------------------------------------------------------------------------|
| Camera                    | OK                                                                                        |
| Speaker / Mic             | OK                                                                                        |
| Bluetooth                 | Not tested yet                                                                            |
| WiFi                      | OK                                                                                        |
| SIM / Mobile Data / Voice | OK Voice, Mobile data works, but sometimes stop (it could be resolved rebooting the phone)|
| VoLTE                     | Not tested yet                                                                            |
| Fingerprint               | Works until the first reboot. After that it not works anymore                            |
| NFC                       | Not tested yet                                                                            |
| Offline Charging          | OK                                                                                        |
| Extra button              | Not working at all                                                                        |
---

I have a working HavocOS 3.6 also, based on GSI Android 10 maade by phusson

Tested By: bahamut657 - Cubot-Quest(IT), Firmware Version AOSP 9 GSI- Date tested 2020/07/09 - Template created by @zguithues and @hackintosh5
