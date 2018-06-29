# [Lava Z50](https://www.gsmarena.com/lava_z50-9137.php) - z50

## Preliminary information and warnings
Your warranty is now void, though it's pretty much easy to re-flash stock firmware & re-lock the bootloader.

## Hardware Support

* Camera: Works out of the box

* Speaker / Microphone : Needs further testing but looks OK

* Bluetooth : Works out of the box

* Wifi : Works out of the box

* SIM / Mobile Data / Voice : Works out of the box

* VoLTE : No VoLTE supported on device

* Fingerprint Reader : No fingerprint reader

***
## Additional Notes
### Flashing procedure for Lava Z50 (z50) retail unit running build LAVA_Z50_1_8_V2.0_S129_20180301_ENG_IN
1. Enable USB debugging and oem unlock in developer options
2. adb reboot bootloader
3. fastboot oem unlock
4. fastboot flash system  _your_gsi_path_
5. fastboot format userdata
6. fastboot reboot


***


## Tested By:
* [Titokhan](https://github.com/Titokhan)
* Flashed using Phh-Treble v21 - arm

Template created by @zguithues