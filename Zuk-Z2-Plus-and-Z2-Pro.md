## Lenovo Zuk Z2 Plus and Z2 Pro <br> <img src="https://www.91-img.com/pictures/98062-v1-lenovo-zuk-z2-mobile-phone-large-1.jpg" alt="Z2 Plus" width="200"/><img src="https://gloimg.gbtcdn.com/soa/gb/pdm-product-pic/Electronic/2016/09/22/goods_img_big-v1/20160922154413_95471.jpg" alt="Z2 Pro" width="200"/>

Full Treble enabled by [Zuk-devs](https://github.com/Zuk-devs) (**Cosmedd, Davidevinavil and DD3Boh**)

**REMEMBER** : Zuk Z2 Plus and Z2 Pro are arm64 and System A-ONLY

## Hardware Support

* Camera & Camcorder
> Working
**Note:** Gcam HDR+ will not work as API2 isnt supported here.

* Speaker / Microphone
> Working

* Bluetooth
> Working

* Wifi & Hotspot
> Working.

* SIM / Mobile Data / Voice
> Calling works, Mobile Data works. 

* GPS
> Working

* VoLTE
> Not Working

* Fingerprint Reader
> Working

* Offline charging
> Working

***
## Additional Notes

We don't have Treble out of the box, it has been enabled by Zuk-devs (Cosmedd, Davidevinavil and DD3Boh)
We are using /factory partition which is around 382mb in our Zuk Z2 as our /vendor partition.

**F.A.Q**

Q: How to get Treble support in Z2 Plus / Z2 Pro?

A: To get **Treble support**, you'll need to flash a latest **ROM which has vendor image** compiled with the latest changes done in sources by ZUK-devs, once you flash such a ROM, you'll get the **vendor stuff stored in the vendor partition**, and after that you can **flash any GSI** on your phone!


Q: Your device doesn't have **/factory** partition?

A: Flash **ZUI 3.5 Oreo** and after that **unlock bootloader** and **flash a TWRP flashable Treble ROM**


***

## Important Links

### Here is a Guide on how to flash Treble builds and how to revert back to Non Treble

**You can find the latest Treble TWRP and a GUIDE on how get TREBLE on your phone here:**

**Z2 Plus:** [Click Here](https://forum.xda-developers.com/lenovo-zuk-z2/how-to/z2plus-treble-roms-flashing-reverting-t3778287)

**Z2 Pro:** [Click Here](https://forum.xda-developers.com/zuk-z2-pro/how-to/z2pro-treble-roms-flashing-reverting-t3778697)

**Note:** From [this](https://github.com/zuk-devs/android_device_zuk_msm8996-common/commit/49409f2132a055590f5d986071e1e1ce174cebc7) commit we have now renamed /factory to /vendor which means now factory is converted into vendor with this you no more need to use modded Magisk, normal Magisk shall work


**XDA Forum**

[Z2_plus](https://forum.xda-developers.com/lenovo-zuk-z2)

[Z2_row](https://forum.xda-developers.com/zuk-z2-pro)

## Tested By:
* **Davidevinavil** - Z2_plus/Z2_row - 20/03/2018
* **Cosmedd** - Z2_row - 20/03/2018
* **Kuber Sharma** - Z2_plus - 25/03/2018
* **Faiz Authar** - Z2_plus - 25/03/2018
* **Subhajeet** - Z2_plus - 23/03/2018
* **Devabhi** - Z2_plus - 22/07/2018

