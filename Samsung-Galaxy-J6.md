# Samsung Galaxy J6
 ## Hardware Support
 * Camera 
> Works after flashing a zip

 * Speaker / Microphone
> Speaker works, Microphone works
 * Bluetooth
> Works
 * Wifi
> Works
 * SIM
> Mobile Data / ingoing voice calls / outgoing voice calls works
 * VoLTE
>Untested
 * Fingerprint Reader
> Works
 * 3.5mm audio jack
>Works
* Hotspot
>Wifi Hotspot works but it automatically turns off when Mobile data is on
***
## Additional Notes
UI (hwcomposer) crashes very often.
Kernel doesn't allow modifications outside of /system, and doesn't allow permissive SELinux domains.

RR arm_binder64 GSI won't boot on this device (Unknown reason)

 ***
## ROMs Tested:
HavocOS 3.0 (with modified 64bit vendor)

AOSP 9.0 - Phh-Treble (2019-03-10)

RR 7.0 (Pie) - Resurrection Remix Team (2019-04-07)
 ## Tested By:
* [Chakib_Chemso](https://github.com/ChemsoDev)
* [phh](https://github.com/phhusson) - 2018-12-05
* [takarushi](https://github.com/takarushi) - 2019-03-10 & 2019-04-07