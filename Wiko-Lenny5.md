# Wiko Lenny5 - W_K400

## Preliminary information and warnings
Your warranty is now void. Wiko declines all responsibility.

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
### Flashing procedure for Lenny5 (W_K400) Pre-Production Sample running Mass Production SW (V01.14)
1.	Enable adb and  oem unlock in developer options
2.	adb reboot bootloader
3.	fastboot flashing unlock
4.	fastboot oem unlock
5.	fastboot flash system  _your_gsi_path_
6.	fastboot reboot


***


## Tested By:
* Max Renusson - Wiko R&D
* Pre-Production sample running Mass Production SW (V01.15)
* Flashed using Phh-Treble v18 - arm

Template created by @zguithues