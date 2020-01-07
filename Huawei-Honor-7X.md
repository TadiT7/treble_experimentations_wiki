# Huawei Honor 7X

* HIGHLY EXPERIMENTAL(USE AT YOUR OWN RISK)
* confirmed on: [BND-L24][BND-L21]
* waiting for confirmation: [BND-AL00/AL10/AL20/L22/L31&TL10]
* have test LineageOS,AOSP and Dotos
* Treble ROMs for Honor 7x:  
  https://forum.xda-developers.com/honor-7x/how-to/best-treble-roms-honor-7x-t3799700

## Hardware Support
### RR and AOSP:
#### Camera
* Works, but does not look as good as stock

#### Speaker / Microphone
* Speaker - works (Works on both ROMs, RR and AOSP)
* Mic - works (AOSP, did not try RR)
* Headphone Jack- works (AOSP, did not try RR)

#### Bluetooth
* I am able to connect to another phone to fileshare but not able to connect bluetooth headphones
* Connected to bluetooth headphones for me on AOSP

#### Wifi
* Works fine

#### SIM / Mobile Data / Voice
* SIM works, not sure if data works because I don't have it, calls work fine
* If you don't get mobile data, you have to enter APN-settings manually.

#### VoLTE
* Unable to provide as this is secondary phone, no sim is attach to device
* Can't check because there is no Volte for my provider

#### Fingerprint Reader
* works

---

### Dotos:
#### SDcard
* Sdcard doesnt seem to be working in the build used (5/15/2018)
#### Camera 
* Works fine
#### Mic
* Works fine
#### Speakers 
* Working fine
#### Bluetooth
* Only tested file transfer and it works fine

---

## Install Instructions

### Prerequisite
* ADB & FASTBOOT 
* UNLOCKED BOOTLOADER
* FRP UNLOCKED(OEM UNLOCKING TURN ON)
* CURRENT EMUI/ANDROID VERSION : EMUI 9.1

### TWRP
FLASH LIKE YOU ARE FLASHING A ROM.(DID NOT TEST AS I DO NOT HAVE TWRP ON 7X)

### USING ADB & FASTBOOT
LINE 1 IS FOR CMD WHILE LINE 2 IS FOR POWERSHELL

#### 1a. Boot into Bootloader via adb
adb reboot bootloader  
.\adb reboot bootloader

#### 1b. Boot into Bootloader via buttons
1. switch off phone
2. connect to pc via usb data-cable
3. press and hold pwr + vol-

#### 2. Flashing the System Img

fastboot flash system system-arm64-aonly.img (LineageOS or RR)  
.\fastboot flash system system-arm64-aonly.img

fastboot flash system system-arm64-aonly-gapps-su.img (AOSP w/ GAPPS and Root)  
.\fastboot flash system system-arm64-aonly-gapps-su.img

fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img (AOSP)  
.\fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img

#### 3. Reboot
fastboot reboot  
.\fastboot reboot

### POST FLASH INSTRUCTIONS

After entering the reboot command, your 7x will reboot and you will see the warning screen where it tell you that your device is unlocked. On that screen "PRESS AND HOLD THE VOLUME UP KEY" to boot into erecovery to perform a Factory Reset. 
If you do not, the phone will boot loop til it forces you too.


## Additional Notes
* When flashing a Gsi , sometimes the system image size gets reduced to the flashed image , to solve this simply resize the system partition via twrp 


## Tested By:
* shadowsiul - BND-L24 - 05/15/2018 - AOSP & LineageOS
* Twigimc - Bnd-L21 - 5/21/2018 - Dotos
* osly888 (crayonicle [on XDA]) - BND-L24 - 6-09-2018 - CosmicOS, Pixel Experience, AEX, AOSiP, XenonHD, AOKP, BootleggersROM
* jabba80 - BND-L21 - 01/07/2020 - AOSP9 v123