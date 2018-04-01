# [Razer Phone] - [cheryl]

## Hardware Support

* Camera:
> Works properly for 1 lens - Porting original Razer Camera unsuccesful

* Speaker / Microphone
> 

* Bluetooth
> 

* Wifi
> 

* SIM / Mobile Data / Voice
> Only detected as 3G, not capable of 4G/LTE (hotplugging Sim-card may fix issue)
> No incoming audio in voicecalls (to be fixed). See #12

* VoLTE
> Not tested

* Fingerprint Reader
> 

***
## Additional Notes

Your device may lose the active partition status from time to time after several reboots or just by turning it off and on, several times. Te device will appear in "Download mode" and won't get out of it. To fix it, type in a fastboot terminal: 
`fastboot set_active a` and `fastboot reboot`  
That will fix it. 

***


## Tested By:
* Sergio (linuxct) @ Razer Oreo DP1 @ 29/03/2018

Template created by @zguithues