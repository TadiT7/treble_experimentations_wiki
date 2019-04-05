# Xiaomi Mi 9

Although this device is A-only, you have to choose GSI for A/B devices because this device is "system-as-root".

## Hardware Support

* Camera:
> Basic usage works. Extented support (= access all cameras) still need work

* Speaker / Microphone
> Works

* Bluetooth
> A2DP AAC works

* Wi-Fi
> Works, tethering works

* GPS
> Works, including double band

* NFC
> Works

* SIM / Mobile Data / Voice
> Works, LTE+ works. Need to switch technology in `*#*#4636#*#*` to LTE/UMTS (global forces 3G... why?)

* VoLTE
> Not tested

* Dual-Sim
> Working except it's not possible to select main (4G) SIM

* Fingerprint Reader
> Works but need high screen brightness

* Brightness control
> Works

* Quick Charge
> Works (9V/2A with USB PD charger)

* Wireless Charge
> Works

* Type-c audio output
> Works

* Video Playback
> Lag on
> VP9 1080p 60fps
> VP9 4k 60fps has the issue
> AVC 4k 60fps 
> https://github.com/phhusson/treble_experimentations/issues/458

## Tested By:
* @phhusson - 17 March 2019
* @linjie997 - 03 April 2019
* @koenkk - 05 April 2019

## Flashing instructions

No need for magisk, nor no-verity, no-forceencrypt... \
You simply need to flash vbmeta then system. \
Download vbmeta from https://github.com/TadiT7/xiaomi_cepheus_dump/raw/cepheus-user-9-PKQ1.181121.001-9.3.1-release-keys/firmware-update/vbmeta.img \
Flash it with `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img` \
Flash system with `fastboot flash system system.img` \
Reboot to recovery and factory reset.


Template created by @zguithues