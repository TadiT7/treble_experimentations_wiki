Tested LineageOS on Huawei P10 Plus (VKY-L29)
Tested AOSP 10/11/12 on Huawei P10 (VTR-L29 9.0.1.201)
## Tested **[PE Android 13] (https://sourceforge.net/projects/altairfr-huawei/files/PixelExp/PixelExperience-13.0-20220930-iceows-ane.7z/download)** (VTR-L29 9.0.1.190)

Tested AOSP 12 on Huawei P10 (VTR-AL00 9.0.1.179(C00E65R1P12))

Tested **[Pixel Experience (Based Android 12)](https://github.com/ponces/treble_build_pe/releases)** on Huawei P10 (VTR-AL00 9.0.1.179(C00E65R1P12)),  
If you want use **Pixel Experience (Based Android 12)** ,you only can install slim version.Because system partition too small.  
  
**Recommended Android GSI version:Android Q(Android 10).**  
> For example:Lineage OS 17,Havoc-OS v3.12 or else.  
  
## Kernel Require(Only For EMUI9.If you are in EMUI8,you can use command in terminal or adb.)  
Some GSI need SELinux is permissive mode.So you need flash the custom kernel. Because official Kernel don't have permissive mode.  
**Recommended kernel:[Pangu Kernel](https://github.com/maimaiguanfan/android_kernel_huawei_hi3660).**  

## Android 13 won't boot without permissive kernel and fstab decrypt 

## Hardware Support

No issues comparing stock Huawei ROM

## Known issues  
  
> If you have magisk, you can use this module to easily solve touchscreen and speakers issues.  
> [Android10 and 11 GSI Generic Fix Module For Huawei P10(Support Android 12 too.)](https://github.com/Coconutat/GSI_Generic_Fix_Magisk_Module_For_Huawei_P10)  

On Oreo vendor:
- Q roms do not boot. (Tested with 8.0.0.386)
- Oreo rom (8.1) did not boot for Snuupy.
- P roms work great and I think it could be used as daily drivers.

On Pie vendor:
- Q/R/S roms boot. Could be used as daily drivers.

* Speakers: Audio playback through speaker not working properly. Audio works through the 3.5mm jack. (Tested with both 9.1.0.252 and 9.0.1.185)
> Fixed on AOSP 12.0 v400.e

> See Fixes Below

* Touchscreen: Left and Right edge of the screen might not respond to touch due to Huawei aptouch service.
> See Fixes Below

* Camera:
> Ugly LineageOS stock camera app, OpenCamera is good but with slow autofocus.

There is a way to run [stock camera app (XDA)](https://forum.xda-developers.com/showpost.php?p=76662319&postcount=225) under LineageOS.

* SIM
> LineageOS asking to reboot when pulling in/out the SIM card. Just reject this requests.

> USSD (like *100#) requests are not working

> USSD seems to be working fine on EMUI 9.0 vendor (Tested on P10, test for yourself)

* WiFi, Mobile Data
> Working perfectly

> Mobile Data on Android 12 requires tuning on Phh Treble Settings > IMS features > Request IMS network

* Fingerprint Reader
> Working perfectly (Broken on Android 12 v400.e)

* Face unlock
> are now available on Pixel Experience v402 

* Fast charging
> Working perfectly

## Installation process

### Prerequisites:

* Stock EMUI 8.0/EMUI 9.0 by Huawei (tested from VKY-L29C10B362/VKY-AL00C00 8.0.0.358/VTR-L29C185E3R1P9T8)
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

> Note: This issue has been fixed since AOSP 12.0 v400.e

### Touchscreen Issue
The touchscreen might be irresponsive on the left/right edge of the screen. Simple workaround is to stop aptouch service as root:

    stop aptouch
 
Or using `adb shell`:

    adb root
    adb shell stop aptouch

### decrypt fstab for Huawei kirin 960
In order for you to decrypt you need to use emui 9.0 base stock not 9.1(9.1 is erofs which it's read only filesystem that can't be mounted), find the fstab.hi3660 in vendor/etc, then edit the fstab just remove the "encrypxxxxxxxxxxxxxxxxxxxxxxxx20m" after do a factory reset from stock recovery 

### Magisk Support 
You can install Magsik v25+ for Based EMUI 9 or EMUI 8 Devices,Even you Use GSI.      
You need download Magsik APP in **[Github releases](https://github.com/topjohnwu/Magisk/releases).**  
Then you cna use adb to install.      
Please note that,**EMUI 9 don't have RAMDISK**.    
So,you need extract **RECOVERY_RAMDIS.img in UPDATA.APP**.You need this page to find your firmware.**[HUAWEI FIRM FINDER V2.0](https://professorjtj.github.io/v2/)**   
Then,follow the guide.Full install guide in here:**[Installation](https://topjohnwu.github.io/Magisk/install.html)**



