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
* LineageOS 17.1 20210114 A/B arm32_binder64
* LineageOS 18.1 20210111 and 20210212 A/B arm32_binder64 vndklite

Baseband version : 
* A107FXXU7BTI8 (Android 10 vendor, Binary 7, Indonesian firmware)
* A107FXXUBTK3 (Android 10 vendor, Binary 7, Indonesian firmware)
* A107FXXU8CUG1 (Android 11 vendor, Binary 8, Indonesian firmware)

Installation Guide : 
1. Unlock the bootloader (it's not that hard. ALL OF YOUR DATA IN INTERNAL STORAGE WILL BE ERASED!)
2. Flash the empty vbmeta.img and TWRP recovery. (You can get it from [here](http://t.me/a107X)
3. Wipe Dalvik, Cache, System
4. Flash the image
5. Reboot

Note :
If you flash Android 12 GSI image with TWRP, you HAVE TO reflash stock recovery and perform factory reset from there since the current TWRP is yet to support Android 12.