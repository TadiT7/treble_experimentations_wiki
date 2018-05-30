# Huawei P10 and P10 Plus

Tested LineageOS, only on Huawei P10 Plus (VKY-L29)

## Hardware Support

No issues comparing stock Huawei ROM

## Known issues

* Camera:
> Ugly LineageOS stock camera app, OpenCamera is good but with slow autofocus.

There is a way to run [stock camera app (XDA)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/huawei-stock-camera-app-treble-roms-t3735169) under LineageOS.

* WiFi, Mobile Data
> Working perfectly

* SIM
> LineageOS asking to reboot when pulling in/out the SIM card. Solution: turn on/off the Airplane Mode.

* Fingerprint Reader
> Working perfectly

* Face unlock
> no feature in LineageOS

## Installation process

Working image: LineageOS by phhusson from [here (XDA)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690)

### Prerequisites:

* Stock Android 8 (Oreo) by Huawei (tested from VKY-L29C10B362)
* Unlocked bootloader

### Installation steps:

* Backup all your internal-storage stuff
* Perform factory reset using **stock Recovery**
* Install GSI image using fastboot as described on XDA

### Superuser (root) and/or Google Apps:

* Install TWRP using fastboot from [here (XDA)](https://forum.xda-developers.com/p10-plus/development/recovery-twrp-3-2-1-0-oreo-t3734993)
* In TWRP: install LineageOS **addonsu** from [LineageOS Extras](https://download.lineageos.org/extras) for arm64 v15.1
* In TWRP: install [from MindTheGapps](http://downloads.codefi.re/jdcteam/javelinanddart/gapps) the file MindTheGapps-8.1.0-arm64-20180320_011441.zip

### TWRP: important note

**DO NOT factory reset user data using TWRP,  ever!** This will break your internal storage! If you need to perform factory reset - flash stock Recovery using fastboot and wipe data in it.

If you will wipe data in TWRP, the LineageOS will not be able to write to userdata (/data) partition, initial device setup will not finish ever.

### Google Apps (GApps)

Why MindTheGapps??? Because [OpenGApps](https://opengapps.org/) is not working. When installing using TWRP it's rising error 20 detecting that we have wrong Android (it minds that we have Android 7.1.2 with wrong SDK level).

