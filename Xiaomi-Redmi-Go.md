**Follow this link **:https://forum.xda-developers.com/android/software/redmi-aosp-9-t3922192
Preliminary information and warnings
Your warranty is now void, though it's pretty easy to re-flash stock firmware & re-lock the bootloader.

Hardware Support
* Camera: 
> Works out of the box (Both back and front)
* Speaker / Microphone : 
> Needs further testing but looks good
* Bluetooth : 
> Works out of the box
* Wi-Fi : 
> Works out of the box
* SIM / Mobile Data / Voice : 
> Works out of the box
* VoLTE : 
> Device supports VoLTE, but can't test at this moment. My provider does not offer VoLTE.
* Google apps : not certified fix by this 
> https://www.xda-developers.com/how-to-fix-device-not-certified-by-google-error/
***

### Bootloader unlocking 

* Flashing procedure for Redmi Go Global feb 1 2019 (verified on July 2019)
* Enable USB debugging and OEM unlock in developer options
* `adb reboot bootloader`
* `fastboot oem unlock-go` works for EU variant
>  These did not work for EU variant: `fastboot oem unlock or fastboot flashing unlock` 

### Flashing direct image

* `fastboot flash system _your_gsi_path_`
* `fastboot format userdata `
* `fastboot reboot`

### flash it via twrp as system image

* Note I used only internal storage for copying files.
* Get the recovery from https://forum.xda-developers.com/android/development/recovery-twrp-3-3-0-redmi-t3929282
* `fastboot flash recovery twrp-3.3.0-0-tiare.img`
* Hold Volume Down + Power Key to boot to TWRP
* Make a backup of stock ROM
* Copy the TWRP backup to your computer just in case
* Copy `system-arm-aonly-gapps-su.img` to internal storage (after` unxz filename` from  https://github.com/phhusson/treble_experimentations/releases
* Flash as 'system image'
* "Format data" (I do not know why, but if I did not do it system did not boot).
* Reboot to System

***

### AOSP 9 graphics glitches
* Edit `/system/build.prop` and add` debug.hwui.renderer=opengl` 
* There are other optimisations on the link on top of the page (I do not know if it is recommended)
***

### Working GSI builds 

* Tested July 2019 AOSP 9.0 v115 https://github.com/phhusson/treble_experimentations/releases   
* Aosp 8 go
* RR oreo go 
* Havoc os pie
* Lineageos 15 go 


