# [OnePlus 7 Pro](https://www.gsmarena.com/oneplus_7_pro-9689.php) - guacamole

## Preliminary information and warnings
OnePlus is cool with warranty, even on unlocked bootloader. You will lose Widevine L1 after unlocking the bootloader, though it's pretty easy to re-flash [stock firmware](https://forum.xda-developers.com/showthread.php?t=3930585) & re-lock the bootloader to regain the functionality.

## Hardware Support

* Camera: Works out of the box (both back and front), although the front camera gets popped up after opening the Camera app (stock or Google Camera ports) and is stuck at the position until reboot. 

* Speaker / Microphone : Works out of the box

* Bluetooth : Works out of the box

* Wi-Fi : Works out of the box

* SIM / Mobile Data / Voice / SMS : Works out of the box

* VoLTE : Device supports VoLTE, but can't test at this moment 

* Fingerprint Reader : Detects the presence of the sensor, but unable to detect any finger after placing them on top of the screen.  

***
## Additional Notes
### Flashing procedure for OnePlus 7 Pro (guacamole) Indian retail unit (GM1911) running OxygenOS 9.5.6.GM21AA
1. Enable USB debugging and OEM unlock in Developer options
2. `adb reboot bootloader`
3. `fastboot oem unlock`
4. `fastboot flash system_a  _your_gsi_path_`
5. `fastboot flash system_b  _your_gsi_path_`
6. `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img` (stock vbmeta.img extracted from official update package)
7. `fastboot -w`
8. `fastboot reboot`


***


## Tested By:
* [Titokhan](https://github.com/Titokhan)
* Tested with [Phh-Treble AOSP v113](https://github.com/phhusson/treble_experimentations/releases/tag/v113) (system-arm64-ab-gapps-su) and [LineageOS 16.0](https://sourceforge.net/projects/andyyan-gsi/files/) by @AndyCGYan (20190515)

Template created by @zguithues