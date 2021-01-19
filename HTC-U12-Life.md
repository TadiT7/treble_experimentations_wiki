# HTC U12 Life

## Hardware support

* Camera
> Working, but sometimes pictures taken on 3rd-party cam apps are darkened a lot.

* Fingerprint
> Working

* Wi-Fi
>Working

* SIM/Calling
> Working
 
* Mobile data
> Working

* Speaker/Microphone
> Working

* Flashlight
> Working

## Bugs

* System frozes when setting up a PIN in setup wizard (only in gapps variant)

* Some UI flickers a lot

* Little chance stucks at lockscreen when trying to unlock

* System UI frozes frequently on some GSI (Try delete `NFC Service` through root explorer or TWRP)

## Requirements

* An ARM64 A-Only image
* TWRP ([Unofficial port](https://onedrive.live.com/redir?resid=F9B931D7BD8BE27F!21020&authkey=!AOpIrolXJBtxyw0))
* [Google's platform tools](https://developer.android.com/studio/releases/platform-tools) extracted on your pc
##
* Connect the phone to your pc, stay connected all the time.
* Open Command Prompt, navigate to the place where you extracted tools


## Unlocking Bootloader

* Enable `OEM Unlocking` in Developer Settings
* Reboot to Bootloader, you can do that by using `adb reboot bootloader` or press `Vol- & Power Button`
* Type `fastboot flashing unlock` 
* You should now see a screen asking you to unlock or not
* Navigate to `Yes` using volume buttons, and hit it with power button

## Installation

* Install TWRP by typing `fastboot flash recovery [TWRP Image]`
* Boot into TWRP, ignore if it shows data encrypted warning
* Choose `Wipe -> Advanced Wipe` and wipe every partition except `Internal Storage`
* Now choose `Reboot -> Bootloader`, It's fine if it gives a "No OS installed" error
* Type `fastboot flash system [Image File]`
* Boot into TWRP again, you can flash additional files now if you want:

* [Magisk Patched for GSI](https://github.com/ExpressLuke/phh-magisk-builder/releases/)
* [Disable Encryption (you can flash this only once)](https://forum.xda-developers.com/t/universal-dm-verity-forceencrypt-disk-quota-disabler-11-2-2020.3817389/)

* Clear data and cache before reboot into system
* Done !

##
Tested By: @asrieldashie ; January 20 2021
Unofficial TWRP and stock system image can be found [here](https://m.gamer.com.tw/forum/C.php?bsn=60559&snA=50050)(Trad. Chinese)
##
Template created by @zguithues and @hackintosh5
