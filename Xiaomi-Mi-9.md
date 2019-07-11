# Xiaomi Mi 9

Although this device is A-only, you have to choose GSI for A/B devices because this device is "system-as-root". 

Tested with AOSP 9.0 v114 image

## Hardware Support

* Camera:
> Basic usage works. Triple camera access works from modded GCAM
> Extented support works enabling it from Phh settings

* Speaker / Microphone
> Works

* Bluetooth
> A2DP AAC works \
> In-call broken

* Wi-Fi
> Works, tethering works

* GPS
> Works, including double band

* NFC
> Works

* SIM / Mobile Data / Voice
> Works, LTE+ works.
> Some GSI force 3G only, type \*#\*#4636#\*#\* and set LTE
> If that doesn't work use primary slot instead of secondary

* VoLTE
> Not tested

* Dual-Sim
> Working except:
> it's not possible to select main (4G) SIM
> it's not possible to set preference for 3g/4g in settings, use *#*#4636#*#* instead
> second sim cannot use 4g due to the above issue

* Fingerprint Reader
> Works
> Broken on Always on Display (turn screen on first)

* Brightness control
> Works

* Quick Charge
> Works (9V/2A with USB PD charger)

* Wireless Charge
> Works

* Type-c audio output
> Works

* Video recording:
> Limited to 1080p/720p. Need to kang Pixel 3 media_profiles_V1_0.xml, /vendor/etc and overwrite the old one \
[media_profiles_V1_0.xml](https://github.com/TadiT7/google_blueline_dump/blob/e43766b36473595b7e3d0ef28613bc0821aeefd0/vendor/etc/media_profiles_V1_0.xml) \
> Limited to 30fps. Need to copy media_profiles.xml to /vendor/etc \
[media_profiles.xml](https://forum.xda-developers.com/attachment.php?attachmentid=4740601&d=1554967755)

* Misc
> Instagram video recording: Good and smooth (stock lags)

## Tested By:
* @phhusson - 17 March 2019
* @koenkk - 05 April 2019
* @linjie997 - 14 April 2019
* @penn5 - 11 July 3187 (descendant 3.0)

## Flashing instructions

No need for magisk, nor no-verity, no-forceencrypt, etc... \

You simply need to flash vbmeta then system. \

Download vbmeta from https://github.com/TadiT7/xiaomi_cepheus_dump/raw/cepheus-user-9-PKQ1.181121.001-9.3.1-release-keys/firmware-update/vbmeta.img \

Download latest adb and fastboot drivers from [https://developer.android.com](https://developer.android.com/studio/releases/platform-tools) 

Connect the phone to your computer with the USB cable

Reboot to bootloader:
```
adb reboot bootloader
```
Flash vbmeta with 
```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
``` 

Flash system with 
```
fastboot flash system system.img
``` 
Reboot to recovery pressing power up + power

Factory reset, reboot

### Community
Telegram: https://t.me/mi9_group


Template created by @zguithues