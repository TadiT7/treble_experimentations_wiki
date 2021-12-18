Tested LineageOS on Huawei P10 Plus (VKY-L29)

Tested AOSP 10 & AOSP 11 on Huawei P10 (VTR-L29 9.0.1.201)

## Hardware Support

No issues comparing stock Huawei ROM

## Known issues

On Oreo vendor:
- Q roms do not boot. (Tested with 8.0.0.386)
- Oreo rom (8.1) did not boot for Snuupy.
- P roms work great and I think it could be used as daily drivers.

On Pie vendor:
- Q and R roms boot (Android 12 not tested yet)

* Speakers: Audio playback through speaker not working properly. Audio works through the 3.5mm jack. (Tested with both 9.1.0.252 and 9.0.1.185)
> See Fixes Below

* Touchscreen: Left and Right edge of the screen might not respond to touch due to Huawei aptouch service.
> See Fixes Below

* Camera:
> Ugly LineageOS stock camera app, OpenCamera is good but with slow autofocus.

There is a way to run [stock camera app (XDA)](https://forum.xda-developers.com/showpost.php?p=76662319&postcount=225) under LineageOS.

* SIM
> LineageOS asking to reboot when pulling in/out the SIM card. Just reject this requests.

> USSD (like *100#) requests are not working

* WiFi, Mobile Data
> Working perfectly

* Fingerprint Reader
> Working perfectly

* Face unlock
> no feature in LineageOS

* Fast charging
> Working perfectly

## Installation process

Working image: LineageOS by phhusson from [here (XDA)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690)

### Prerequisites:

* Stock Android 8 (Oreo) by Huawei (tested from VKY-L29C10B362 and VKY-AL00C00 8.0.0.358)
* Unlocked bootloader

### Installation steps:

* Backup all your internal-storage stuff
* Perform factory reset using **stock Recovery**
* Install GSI image using fastboot as described on XDA

### Superuser (root) and/or Google Apps, if you wish:

* Install TWRP using fastboot from [here (XDA)](https://forum.xda-developers.com/p10-plus/development/recovery-twrp-3-2-1-0-oreo-t3734993)
* Reboot to TWRP pressing VolumeUp till it's loaded
* Leave system non-modified when TWRP ask for it
* In TWRP: install LineageOS **addonsu** from [LineageOS Extras](https://download.lineageos.org/extras) for arm64 v15.1
* In TWRP: install [from MindTheGapps](http://downloads.codefi.re/jdcteam/javelinanddart/gapps) the file MindTheGapps-8.1.0-arm64-20180320_011441.zip

### TWRP: important note

**DO NOT factory reset user data using TWRP,  ever!** This will break your internal storage! If you need to perform factory reset - flash stock Recovery using fastboot and wipe data in it.

If you will wipe data in TWRP, the LineageOS will not be able to write to userdata (/data) partition, initial device setup will not finish ever.

### Google Apps (GApps)

Why MindTheGapps??? Because [OpenGApps](https://opengapps.org/) is not working. When installing using TWRP it's rising error 20 detecting that we have wrong Android (it minds that we have Android 7.1.2 with wrong SDK level).

#### Note: OpenGapps for Android 9.0 (Pie) is now working for Pie GSIs.

## Fixes

### Fix for Speakers
Audio through speakers can be fixed by running these commands as root for every boot:

    chown root:audio /dev/nxp_smartpa_dev
    chmod 0660 /dev/nxp_smartpa_dev

Or running commands using `adb shell`:

    adb root
    adb shell chown root:audio /dev/nxp_smartpa_dev
    adb shell chmod 0660 /dev/nxp_smartpa_dev

> Note: This issue has been addressed and has a fix for newer builds of Phh AOSP

### Touchscreen Issue
The touchscreen might be irresponsive on the left/right edge of the screen. Simple workaround is to stop aptouch service as root:

    stop aptouch
 
Or using `adb shell`:

    adb root
    adb shell stop aptouch
