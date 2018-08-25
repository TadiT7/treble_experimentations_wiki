# Xiaomi Mi 6X (wayne)

## Function Availability & Known Bugs

**Bugs and untested items are shown bold. 3rd-party apps untested.**

* Camera
  * Front: OK
  * Rear: Upper one: **Not working**, Lower one: OK
  * **Enabling Do Not Disturb (DND) will cause stock camera app to FC (force close).**

* LED Light: **Always on** *You may not be able to use front camera when LED light is off. Reboot may help.*

* Speaker / Microphone: OK

* Bluetooth
  * Music: OK
  * File Transfer: OK
  * Headset (Calls): **Not working**

* Wi-Fi: OK

* RIL (Calls / SMS / Data):
  * CMCC/CHN-UNICOM: OK, China Telecom: **Untested**
  * Dual SIMs: OK
  * VoLTE: **Untested**
  * **MEID not found**

* Fingerprint Reader: *Varies by the manufacturer*
  * FPC: OK
  * Goodix: **Not working**
  * *You can check the manufacturer using 3rd-party apps, or run `getprop | grep goodix` in adb shell/terminal. If you get any return, you may be using Goodix.  If you are sure you're using FPC, try flashing stock MIUI before flashing the ROM again.*

* Brightness control: **Bad** *The brightness changes too fast, and it flashes when you lock the screen.*

* USB connection: *Varies by Android version*
  * 8.1: Charging/USB Debugging/Network Sharing/MTP/PTP: OK
  * 9.0: Charging/USB Debugging/Network Sharing: OK, MTP/PTP: **Not working**
  * *Quick charge works better than stock MIUI, but the phone didn't show the charging status while quick charging.*

## How To Flash

* Backup your data first
* Unlock your phone
* Flash TWRP
* Boot into TWRP and wipe /data, /cache (factory reset) and /system (Best format /data partition)
* Connect your phone to the computer, and mount /data via MTP
* Copy the image file into your phone
* Flash the image file in TWRP (Flash in fastboot will result unknown error.)

(Flash in TWRP)

````
......
[镜像刷入开始]
刷入镜像：/sdcard/system-arm64-aonly-gapps-su.img
正在计算镜像刷入详情...
I:Image filename is: system-arm64-aonly-gapps-su.img
正在刷入System镜像...
I:Flash command: 'simg2img '/sdcard/system-arm64-aonly-gapps-su.img' '/dev/block/mmcblk0p61''
I:simg2img '/sdcard/system-arm64-aonly-gapps-su.img' '/dev/block/mmcblk0p61' process ended with RC=0
[镜像刷入完成]
I:Set page: 'action_complete'
I:operation_end - status=0
......
````
(Flash in fastboot)

````
>fastboot flash system system-arm64-aonly-gapps-su.img
target reported max download size of 536870912 bytes
erasing 'system'...
OKAY [  0.546s]
sending sparse 'system' (524284 KB)...
OKAY [ 12.064s]
writing 'system'...
OKAY [  0.000s]
sending sparse 'system' (524284 KB)...
FAILED (command write failed (Unknown error))
finished. total time: 13.614s
````
* Reboot and Enjoy!

## Notes

* **After v23, /data partition will be encrypted. Please backup your data before flashing.**
* **Some people reported that phone was muted, not be able to use camera, etc. after flashing 9.0 ROM. Best try flashing stock MIUI before flashing the ROM.**
* Xiaomi Mi 6X (wayne) is similar to Xiaomi Mi A2 (jasmine), but the latter one has A/B partitions, the former one only have A partition.
* Rollback protection will be enabled after MIUI V9.6.4.0 (Stable) / 8.8.6 (Dev), but before flashing, I (suwakowww) was using MIUI 8.7.26 (Dev). You can still flash GSI images, but you should avoid flashing any MIUI ROM before V9.6.4.0 (Stable) / 8.8.6 (Dev), or your phone will be bricked.
* Installing Magisk doesn't affect the encryption, but you can find encryption disabling tools using search engines.

## Tested By

* suwakowww @ AOSP v22 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-07
* suwakowww @ AOSP v23 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-17
* suwakowww @ AOSP v101 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-22
* suwakowww @ AOSP v102 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-23
* best yuan(`16***37@qq.com`), isaacchen(`ti***64@gmail.com`), pipipig(`22***13@qq.com`), stubbom(`29***82@qq.com`), xcxmiku, 墨水淘气包(`17***32@qq.com`), etc. (sort by alphabet, are reported in QQ group) @ AOSP v102, AOSP v101, PixelExperience, etc. , 2018-08-25