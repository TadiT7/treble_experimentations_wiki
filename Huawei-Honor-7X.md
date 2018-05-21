# Huawei Honor 7X - [BND-L24] [BND-AL00/AL10/AL20/L21/L22/L31&TL10(Hopefully)]

# **HIGHLY EXPERIMENTAL(USE AT YOUR OWN RISK)**

#Only have test LineageOS and AOSP

## Hardware Support

* Camera:
> Works, but does not look as good as stock

* Speaker / Microphone
> Speaker - yes
> Mic - ?
> Headphone Jack- ?

* Bluetooth
> I am able to connect to another phone to fileshare but not able to connect bluetooth headphones

* Wifi
> Works fine

* SIM / Mobile Data / Voice
> Unable to provide as this is secondary phone, no sim is attach to device

* VoLTE
> Unable to provide as this is secondary phone, no sim is attach to device

* Fingerprint Reader
> works
***

# Prerequisite

* ADB & FASTBOOT 
* UNLOCKED BOOTLOADER
* FRP UNLOCKED(OEM UNLOCKING TURN ON)
* CURRENT EMUI/ANDROID VERSION : EMUI 8/8.0
***
## Install Instructions

**TWRP**

FLASH LIKE YOU ARE FLASHING A ROM.(DID NOT TEST AS I DO NOT HAVE TWRP ON 7X)

**USING ADB & FASTBOOT**

LINE 1 IS FOR CMD WHILE LINE 2 IS FOR POWERSHELL

**Boot into Bootloader**

adb reboot bootloader

.\adb reboot bootloader

**Flashing the System Img**

fastboot flash system system-arm64-aonly.img (LineageOS or RR)

.\fastboot flash system system-arm64-aonly.img

fastboot flash system system-arm64-aonly-gapps-su.img (AOSP w/ GAPPS and Root)

.\fastboot flash system system-arm64-aonly-gapps-su.img

fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img (AOSP)

.\fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img

**Reboot**

fastboot reboot

.\fastboot reboot

# POST FLASH INSTRUCTIONS

After entering the reboot command, your 7x will reboot and you will see the warning screen where it tell you that your device is unlocked. On that screen "PRESS AND HOLD THE VOLUME UP KEY" to boot into erecovery to perform a Factory Reset. 
If you do not, the phone will boot loop til it forces you too.
***

## Additional Notes
When flashing a Gsi , sometimes the system image size gets reduced to the flashed image , to solve this simply resize the system partition via twrp 

***


## Tested By:
* shadowsiul - BND-L24 - 05/15/2018 - AOSP & LineageOS
* Twigimc - Bnd-L21 - 5/21/2018 - Dotos
