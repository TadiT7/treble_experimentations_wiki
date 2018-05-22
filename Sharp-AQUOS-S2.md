# [Sharp AQUOS S2] - [ss2/sat]

## Hardware Support

* Camera:
> Working

* Speaker / Microphone
> Working

* Bluetooth
> Working

* Wi-Fi
> Working

* SIM / Mobile Data / Voice
> Working

* VoLTE
> Unable to test

* Fingerprint Reader
> Working

***
## Additional Notes

* In fact the boot kernel of [[Nokia 6 (2018)]], [[Nokia 7]], [[Nokia 7 plus]] and [[Sharp AQUOS S2]] are identical.  
You can use Nokia 7 or 7 plus kernel on AQUOS S2, but camera, Wi-Fi and some other functions won't work properly.

* The OS doesn't display status bar properly due to notch (cutout) and Sharp / FIH Mobile aren't providing proper vendor image.  
To fix this problem, you have to add overlay by yourself or flash [modded vendor image for 00CN_2_070](https://drive.google.com/open?id=1h_lby181FerHcs3pg45SAoiY9-nGtomO) and [boot image](https://drive.google.com/open?id=1_uginpiJ_JfRuE0Z8oeR1D-qnsHUZWN-).

* For some reason, bootloader sometimes forget what slot he is using now and reboot to bootloader continuously.  
You can check current slot by `fastboot getvar current-slot` and re-set by `fastboot --set-active=_a reboot` or `fastboot --set-active=_b reboot`.

***


## Tested By:
* AndroPlus ([@AndroPlus_org](https://twitter.com/AndroPlus_org)) @ SHARP AQUOS S2 (SS2) 00CN_2_070 @ 22/05/2018
* Calyx Hikari (@HikariCalyx) @ SHARP AQUOS S2 (SS2) 00CN_2_070 @ 17/04/2018
