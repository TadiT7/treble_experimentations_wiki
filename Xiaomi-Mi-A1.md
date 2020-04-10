# Xiaomi Mi A1 - tissot

## Hardware Support

* Camera:
> Working

* Speaker / Microphone
> Working

* Bluetooth
> Working

* Wifi
> Working

* SIM / Mobile Data / Voice
> Working

* VoLTE
> Working

* Fingerprint Reader
> Working

* Offline Charging
> Not working (tested on 2020-04-09 by fenik, see section below) 

* FM Radio
> Not working; Missing userspace application and possibly support by community vendor images

***
## Additional Notes

Treble on the A1 is unofficial and was ported by CosmicDan. A tutorial is available [here on XDA](https://forum.xda-developers.com/mi-a1/how-to/treble-stock-to-treble-everything-to-t3793734). The tool repartitions devices for 2 vendor partions, slot A and slot B.


***


## Tested By:
* fenik on 2020-04-09: sooti's boot.img (2020-01-20) and vendor.img (2020-01-28) (
  - Android 11 Google GSI (gsi_gms_arm64-exp-RPP2.200227.014-6343719.zip): Stuck at boot animation
  - Android 10 Google GSI (gsi_gms_arm64-exp-QJR1.191112.001-6004257.zip): Boots, setup can't be completed due to missing screen lock options
  - LineageOS 17.0 AndyYan (lineage-17.1-20200309-UNOFFICIAL-treble_arm64_bvN.img): Seems to be working fully, aside from offline charging, possibly due to fault in sooti's vendor/boot 
* Nofan Tasi - 2020-03-05
  - Phh AOSP Android 10/Q (March 2020) fully working
   - sooti 07-11-19 vendor.img
   - prorooter007 Lightning Kernel V5.1
   - giovix92 TWRP 3.3 withTM 2.1
* GabrielHoward - 2018-12-03
  - [Android P PQ2A](https://t.me/psemigsi) working
* kdrag0n - Resized userdata - 2018-05-27
  - Phh-AOSP, Phh-RR, dotOS working
  - Phh-Lineage and AOSIP stuck on boot animation

* dgadelha - Resized userdata - 2018-06-02
  - Phh-Pixel Experience working

* Prochy - Resized userdata - 2018-06-04
  - AEX 5.4 working

* Cj-Malone - Resized userdata - 2018-07-02
  - [Lineage OS (2018-06-27, vanilla)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690) booting
  - [AOSP (2018-06-27, vanilla)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) booting
  - [CosmicOS (2018-06-14)](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/cosmic-ospulsar8-1-0201805243-2-t3794806) booting

* Codie - Resized userdata - 2018-07-17
   - [Android P DP3/Beta 2 (2018-07-17)](https://forum.xda-developers.com/mi-a1/how-to/guide-install-android-p-dp3-mi-a1-t3817937) booting
  - [Android P DP4/Beta 3 (2018-07-19)](https://forum.xda-developers.com/mi-a1/how-to/guide-install-android-p-dp3-mi-a1-t3817937) booting
  - [Android P DP5/Beta 4 (2018-07-25)](https://forum.xda-developers.com/mi-a1/how-to/guide-install-android-p-dp3-mi-a1-t3817937) booting