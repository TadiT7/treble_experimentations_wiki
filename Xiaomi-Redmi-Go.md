**Follow this link **:https://forum.xda-developers.com/t/xiaomi-redmi-go

Preliminary information and warnings
Your warranty is now void, though it's pretty easy to re-flash stock firmware & re-lock the bootloader.

Hardware Support
* Camera: 
> Works out of the box (Both back and front are working fine but the default camera app takes too long to open)
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
> flash this https://forum.xda-developers.com/attachment.php?attachmentid=4817057&d=1567996750
***

### Bootloader unlocking 

* Flashing procedure for Redmi Go Global feb 1 2019 (verified on July 2019)
* Enable USB debugging and OEM unlock in developer options
* `adb reboot bootloader`
* `fastboot oem unlock-go` works for EU variant
>  These did not work for EU variant: `fastboot oem unlock or fastboot flashing unlock` 

### Flashing direct image

*  Note some expert please add the decryption fix here. as this method does not work.
* `fastboot flash system _your_gsi_path_`
* `fastboot reboot `
* The system will ask for decryption password.
* Just type any random phrase as password. It will say, wrong password - do you like to reset device encryption
* Say yes.
* Phone will reboot. All good.

### flash it via twrp as system image

* Note I used only internal storage for copying files.
* Get the recovery from https://forum.xda-developers.com/android/development/recovery-twrp-3-3-0-redmi-t3929282
* `fastboot flash recovery twrp-3.3.0-0-tiare.img`
* Hold Volume Down + Power Key to boot to TWRP
* Make a backup of stock ROM
* Copy the TWRP backup to your computer just in case
* Now inside TWRP -> Format DATA. Type "yes".
* In the same thread ( https://forum.xda-developers.com/android/development/recovery-twrp-3-3-0-redmi-t3929282 ) there is the "Decryption Fix" file: decrypt.zip
* copy the decrypt.zip to your phone using MTP
* Select install and flash the decrypt.zip
* Now copy `system-quack-arm-aonly-vanilla.img` to internal storage (after` unxz filename` from  https://github.com/phhusson/treble_experimentations/releases
* Flash as 'system image'
* Reboot to System


***


### Working GSI builds 

* Tested AOSP 10.0 v209 (Jan 2020) 
* Tested sep 2019 AOSP 9.0 v119 https://github.com/phhusson/treble_experimentations/releases   
* Aosp 8 go
* RR oreo go 
* Havoc os pie
* Lineageos 15 go 
* android 10 200c



