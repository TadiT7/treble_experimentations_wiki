## HTC U12 Life
![](https://s.yimg.com/zp/MerchandiseImages/FBFAD7ACDB-SP-6410389.jpg)

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

* System UI freezes frequently on some GSI (Try delete `/System/app/NfcNci` through root explorer or TWRP

* System nearly freezes in ringtone selection window (only on R)

## Requirements

* An ARM64 A-Only (vndklite) image
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

# Tested GSIs

## Boots

* [phh AOSP](https://github.com/phhusson/treble_experimentations/releases)
* [CAOS](https://sourceforge.net/projects/treblerom/files/CAOS/)
* [Descendant XI (vndklite)](https://downloads.descendant.me/)
* [LineageOS](https://sourceforge.net/projects/andyyan-gsi/files)
* [HavocOS](https://sourceforge.net/projects/havoc-os/files/arm64-aonly/)
* [BlessRoms](https://sourceforge.net/projects/treblerom/files/BLESS)
* [Diust's GSI](https://sourceforge.net/projects/androidgsi/files/)
* [eremitein's GSI](https://sourceforge.net/projects/treblerom/files/)

## Not booting

* All non phh-based GSI
* Non vndk-lite
* [AlphaROM](https://alpha.droidstars.com/)

## Untested

None

##
Tested By: @asrieldashie ; Feb 7 2021
##
Unofficial TWRP and stock system image can be found [here](https://m.gamer.com.tw/forum/C.php?bsn=60559&snA=50050)(Trad. Chinese)
##
Template created by @zguithues and @hackintosh5
