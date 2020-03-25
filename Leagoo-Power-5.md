# Device

Leagoo Power 5
Sim operator Tele2 Lithuania, Firmware Version - AOSPEX 6.5 -
ARM64 A Only

Requirements::

* Unlocked Bootloader;
* Your Recovery has to be stock, so if you have TWRP, I recommend to reflash the stock one;
* Choose an ARM64 A GSI Rom from [here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list);


Quick Guide:

Turn off your phone and then start it with Power and VOL-, until you see the Android Fastboot now;
On Windows download ADB tools and Linux or Mac they can be added using terminal (You can find it easily by doing a simple search);
To make sure the phone is correctly connected, type in the CMD Line or Terminal: fastboot devices ;
You should see a series of numbers, so now you can flash by typing: fastboot flash system WHATEVERGSIIMAGEYOUCHOOSE.IMG ;
Wait about 2-3 minutes and then when the flash is finished, type: fastboot reboot ;
That's it! Your phone should now boot to your preferred GSI ROM with more or less everyhing working 
## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera 1 and 2            | OK |                                               
| Speaker / Mic             | OK |                                            
| Bluetooth                 | OK |                                                 
| WiFi                      | OK |                                                  
| SIM / Mobile Data / Voice | OK |                                                  
| VoLTE                     | Not verified|                                                 
| Fingerprint               | OK |                                                                                         
| Fast and Wireless Charging| OK |                                                  
| GPS                       | OK |    
| Notification Led          | OK |
| Brightness                | OK |