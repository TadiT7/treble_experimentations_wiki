What's working?

* Telephony (Phone, SMS)
* Dual SIM
* Wi-Fi
* Bluetooth
* Fingerprint
* Camera
* OTG
* etc.

What's not working?
* MTP
* VoLTE, video calling (Samsung devices isn't expected to run VoLTE within GSI)
* Camera focus (only in certain apps; happened if you're using Android 11 GSIs on Android 10 vendor)


GSI Build Tested : 
* AOSP 10 v222 A/B arm32_binder64 gapps
* AOSP 11 v300.l A/B arm32_binder64 gapps
* AOSP 12.1 v416 A/B arm32_binder64 vanilla and gapps
* AOSP 13 r35 A/B arm32_binder64 vanilla
* LineageOS 17.1 20210114 A/B arm32_binder64
* LineageOS 18.1 20210111 and 20210212 A/B arm32_binder64 vndklite
* LineageOS 19.1 20230223 A/B arm32_binder64
* LineageOS 20.0 20230218 A/B arm32_binder64
* xdroidOSS 12.1 20221217 A/B arm32_binder64
* OctaviOS v3.2 202201-- A/B arm32_binder64

Baseband version : 
* A107FXXU7BTI8 (Android 10 vendor, Binary 7, Indonesian firmware)
* A107FXXUBTK3 (Android 10 vendor, Binary 7, Indonesian firmware)
* A107FXXU8BUC2 (Android 10 vendor, Binary 8, Indonesian firmware)
* A107FXXU8CUG1 (Android 11 vendor, Binary 8, Indonesian firmware)

Installation Guide : 
1. Unlock the bootloader (it's not that hard. ALL OF YOUR DATA IN INTERNAL STORAGE WILL BE ERASED!)
2. Flash the empty vbmeta.img and TWRP recovery. (You can get it from [here](https://t.me/a107X) or [here](https://t.me/shirayuki_plygrnd/41519)
3. Flash A10s-encryption-disabler.zip if you want to full decrypt of your /data partition
4. Wipe Data, Dalvik, Cache, System
5. Flash the image
6. Flash the GApps if you're using vanilla build. If you're using GApps build, skip to Step 7
7. Reboot

Note :
* If you flash Android 13 GSI image with Encryption Disabler, lockscreen didn't working. So, restore stock vendor, and format data to get back the lockscreen