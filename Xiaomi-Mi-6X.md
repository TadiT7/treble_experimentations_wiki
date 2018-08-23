# Xiaomi Mi 6X - wayne

## Hardware Support

* Camera
> Front: OK, but flashlight is ALWAYS ON.

> (Update v23: When you found the light is OFF, you may not use front camera until next boot.)

> Rear: Upper one is not working, but lower one works well. (3rd-party app untested)

* Speaker / Microphone
> OK

* Bluetooth
> Music, File transfer are OK, Headset (calling) NOT WORK.

* Wi-Fi
> OK 

> <strike>(9.0 is NOT WORK, and MAC address is LOST)</strike> Fixed in v102.

* SIM / Mobile Data / Voice
> CMCC and CHN-UNICOM are OK. Dual SIMs are OK, too.

> China Telecom untested, but can't find MEID in device (stock rom has MEID).

* VoLTE
> Untested

* Fingerprint Reader
> OK

* Brightness control
> BAD, the brightness value changes too fast, and cause some flashes when locking screen. 

> (v23 update: higher brightness, faster flashes.)

* USB
> <strike>BAD, it can charge only ,charge will show normally except quick charge.</strike> Fixed in v23.

> (9.0 can't use MTP and PTP, but you still can use USB debug and network sharing)

> Quick charge works better than stock rom, it just not show charging status.

> <strike>Maybe you can use MTP in TWRP.</strike> (You can use "adb push" or "adb pull" to transfer files in 9.0)


## How to flash
* Backup your data first
* Unlock your phone
* Flash TWRP
* Boot into TWRP and wipe /data, /cache (factory reset), /system.
* Connect you phone to computer, and mount drive via MTP
* Copy image file into your phone
* Flash img files in TWRP. (Flash in fastboot will result unknown error.)

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

## Additional Notes
* Maybe Mi 6X (wayne) is same as Mi A2 (jasmine), but Mi A2 has A/B partitions, Mi 6X have only A partition.
* Mi 6X will enable rollback protection after V9.6.4.0 (Stable) / 8.8.6 (Dev), but before flashing, my phone rom is 8.7.26 (Dev)
* (Somebodies reported they can flash after enabling rollback protection)
* After v23, /data partition will be encrypted. Please BACKUP YOUR DATA BEFORE FLASHING.  
* (Flash Magisk is NOT affect to finished encryption.)

## Tested By:
* suwakowww @ AOSP v22 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-07
* suwakowww @ AOSP v23 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-17
* suwakowww @ AOSP v101 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-22
* suwakowww @ AOSP v102 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-23