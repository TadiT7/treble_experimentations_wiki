What's working?

Telephony (Phone, SMS), Dual SIM, Wi-Fi, Bluetooth, Fingerprint, Camera, OTG, etc.

What's not working?
MTP (kernel-related problem)
VoLTE, video calling (settings is disabled in *#*#4636#*#*)

GSI Build Tested : AOSP 10 v222 A/B arm32_binder64 gapps

Baseband version : A107FXXU7BTI8 (Android 10 vendor, Binary 7, Indonesian firmware)

Installation Guide : 
1. Take the stock boot.img then patch it with Magisk.
2. Unlock the bootloader.
3. Flash empty vbmeta.img (you can get in on Google)
4. Flash patched boot.img
5. Re-unlock the bootloader (I don't know why the bootloader is locked again after flashing boot.img)
6. Flash system with GSI image, make sure that auto-reboot in Odin is checked.
7. Enter recovery mode, then do factory reset.
8. Reboot system. You will see your device won't boot. It's okay. Let it for a while, around a minute, then enter recovery mode again.
9. Mount /system and reboot system.
10. Your phone should boot now.

Note : You should compress clean vbmeta.img, patched boot.img, and GSI system.img with lz4¹ and build tar.md5² from it, then put in on "AP" section on Odin.

How to compress with lz4 and build tar.md5 : [here](https://forum.xda-developers.com/t/guide-custom-how-to-install-custom-rom-using-odin-without-twrp-phh-lineageos.4114435/)
(Step 5 - 23)