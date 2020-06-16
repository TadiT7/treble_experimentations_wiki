Device: EVA-L09  
ROM: [Phh-Treble AOSP 9.0](https://github.com/phhusson/treble_experimentations/releases/tag/v119)  
Vendor: EVA-AL10 B540, with baseband patches for international usage (credit: Tecalote & zgfg)  
EMUI 8.0 vendor, VNDK 26, ARM64 A-only  
  
## Software Support
* Android Support
>Most Oreo and Pie ROMs work.  
>**Android 10 ROMs won't boot for now**, they won't get past the boot logo.  
* SafetyNet
>SafetyNet fails both checks, no way found to amend this for now. Magisk Hide is required
* Other quirks
>A sizable portion of Play Store's apps are missing (reported incompatible) on non-OpenKirin ROMs. No fix for now.  
>Opening Connections menu crashes Settings  
>MTP doesn't work.  
>Offline charging requires a patch  
>Enabling USB debugging will cause adbd to hog all the CPU, causing severe battery drain  
## Hardware Support
* Decoding and GPU acceleration
> Working perfectly
* RIL
> Incoming/outgoing calls, emergency calls, 3G/4G mobile data, SMS send/receive are all working perfectly (Single SIM tested only)
* WiFi
> Working perfectly
* Hotspot
> Working perfectly
* Bluetooth
> Can pair, send, receive and stream audio. Opening the Bluetooth/NFC settings from the Settings app crashes it, but can be accessed from quick settings.
* NFC
> Not working out of the box, requires a Magisk module (NFC4PRA-GSI), even then it seems to not work well. Further testing needed.

* Camera
> Camera doesn't work...but a flashable ZIP in XDA Developers can restore EMUI 8.0 camera functionality. Fully functioning photo and video recording when restored.
* Speakers
> Working perfectly
* Headphone Jack
> Works, but sound is not routed to the headphones automatically upon connection/disconnection and requires manual intervention. Also audio effects are broken on headphones and Bluetooth audio but EMUI 8.0 vendor drivers seem to be the culprit. Attempting to use bass boost effects will result in a high pitched whine that is annoying. Sound quality on headphones is mediocre and soulless compared to EMUI 5.

* Fingerprint Reader
> Working perfectly

* Face unlock
> Working perfectly

## Installation process for GSIs

Tested ROMs: Phh-Treble, AndyYan LineageOS
### Prerequisites:

* Unlocked bootloader
* For international models, rebrand to Chinese model
* EMUI 8.0 firmware, B540 revision.
* Vendor image patches for Face Unlock and international GSM radio support (IMPORTANT!)

### TWRP and Encryption: important note

**If you didn't follow [this guide](https://forum.xda-developers.com/p9/how-to/guide-easy-decryption-guide-gsi-users-t4115033) to _decrypt your internal storage_ DO NOT factory reset user data using TWRP!** This will break your internal storage! If you need to perform factory reset while maintaining encryption- flash stock Recovery using fastboot and wipe data in it.  

If you will wipe data in TWRP without **decrypting your phone**, your custom ROM will not be able to write to userdata (/data) partition, initial device setup will not finish ever.  

**Decrypted phones CAN factory reset through TWRP!**  

### Installation steps:
* Backup all your internal-storage stuff
* Perform a factory reset, **remember to use your stock recovery if you HAVEN'T decrypted your device.**
* Flash your GSI image to /system. This can be done with fastboot or TWRP. **The latter is recommended because it's less prone to errors with ROMs bigger than 450 MB**.

### Restoring Camera:
* Install TWRP in fastboot by flashing it to recovery_ramdisk.
* Reboot to TWRP by executing `fastboot reboot recovery`
* In TWRP: flash [this ZIP](https://forum.xda-developers.com/p9/themes/p9-camera-treble-gsi-t4006381) to restore your Camera app and libraries.

### Restoring Offline Charging:
* Install TWRP in fastboot by flashing it to recovery_ramdisk.
* Reboot to TWRP by executing `fastboot reboot recovery`
* In TWRP: flash [Offline_charging_fix_for_GSIs-Hi6250.zip](https://forum.xda-developers.com/attachment.php?attachmentid=4771494&d=1559676926) to restore offline charging abilities.

### Google Apps (GApps):
* Flash in TWRP an appropriate package from [OpenGApps](https://opengapps.org/), **it MUST be Android 9.0 for ARM64 devices**.

#### Note: OpenGapps for Android 9.0 (Pie) is now working for Pie GSIs.
