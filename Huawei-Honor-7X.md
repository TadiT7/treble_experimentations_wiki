# Huawei Honor 7X - [BND-L24] [BND-AL00/AL10/AL20/L21/L22/L31&TL10(Hopefully)]

## Hardware Support

* Camera:
> Works, but does not look as good as sotck

* Speaker / Microphone
> Speaker - yes
> Mic - ?
> Headphone Jack- ?

* Bluetooth
> I am able to connect to another phone to file share but not able to connect bluetooth headphones

* Wifi
> Works fine

* SIM / Mobile Data / Voice
> Unable to provide as this is my game phone, no sim is attach to device

* VoLTE
> Unable to provide as this is my game phone, no sim is attach to device

* Fingerprint Reader
> worked on AOSP.did not test on lineageOS

***
## Install Help
**Command Prompt**

**Boot into Bootloader**

adb reboot bootloader

**Flashing the System Img**

fastboot flash system system-arm64-aonly.img (LineageOS or RR)

fastboot flash system system-arm64-aonly-gapps-su.img (AOSP w/ GAPPS and Root)

fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img (AOSP)

**Reboot**

fastboot reboot

**Powershell**

**Boot into Bootloader**

.\adb reboot bootloader

**Flashing the System Img**

.\fastboot flash system system-arm64-aonly.img 	(LineageOS or RR)

.\fastboot flash system system-arm64-aonly-gapps-su.img	(AOSP w/ GAPPS and Root)

.\fastboot flash systemsystem-arm64-aonly-vanilla-nosu.img  (AOSP)

**Reboot**

.\fastboot reboot

# POST FLASH INSTRUCTIONS

After entering the reboot command, your 7x will reboot and you will see the warning screen where it tell you that your device is unlocked. On that screen "PRESS AND HOLD THE VOLUME UP KEY" to boot into erecovery to perform a Factory Reset. 
If you do not, the phone will boot loop til it forces you too.
***
***
## Additional Notes


***


## Tested By:
* shadowsiul - BND-L24 - 05/15/2018 - AOSP & LineageOS
