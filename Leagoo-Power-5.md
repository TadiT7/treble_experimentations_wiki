# Device

Leagoo Power 5
Sim operator Tele2 Lithuania, Firmware Version - AOSPEX 6.5 -
ARM64 A Only

Requirements::

* Unlocked Bootloader (Not explained here, so you need to use HCU Unlock and purchase a credit for that);
* Your Recovery has to be stock, so if you have TWRP, I recommend to reflash the stock one;
* Choose an ARM64 AB GSI Rom from [here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list);

BUGS:

1. The device might show as not certified, so you won't be able to use any Google services until you register your device. Guide from [Androidsage](https://www.androidsage.com/2018/03/29/fix-device-is-not-certified-by-google-error-on-play-store/)to help doing that;
2. Brightness seems to be at 50% when set at a maximum. This issue might be due to the Vendor Overlays (not a 100% sure though), I am investigating this, but I am using the device as it is and it is fine for me, until we find a solution for it.

Quick Guide:

1. Turn off your phone and then start it with Power and VOL+, until you see the message of the unlocked phone;
2. Wait until you see the Stock recovery not eRecovery;
3. Wipe and reset, Type "YES" and wait for wiping;
4. Plug the USB Cable to PC, reboot the phone while pressing VOL - ;
5. You should see the Android Fastboot now;
6. On Windows download ADB tools and Linux or Mac they can be added using terminal (You can find it easily by doing a simple search);
7. To make sure the phone is correctly connected, type in the CMD Line or Terminal: fastboot devices ;
8. You should see a series of numbers, so now you can flash by typing: fastboot flash system WHATEVERGSIIMAGEYOUCHOOSE.IMG ;
9. Wait about 2-3 minutes and then when the flash is finished, type: fastboot reboot ;
10. That's it! Your phone should now boot to your preferred GSI ROM with more or less everyhing working 
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
| Fast Charging             | OK |                                                  
| GPS                       | OK |    
| Notification Led          | OK |
| Brightness                | 50% only |