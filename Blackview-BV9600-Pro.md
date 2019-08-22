# Device

BV9600Pro Internationnal version     
Stock Firmware : BV9600Pro_S700_V1.1_20190104V45     
Tested phh's *AOSP 8.1 v29* and *AOSP 9 v109*

#### Actual status (15/05/2019):
 - Booting is long (30+ min) but go trought  
 - Some rare freeze and ui crash.   
 - No main speaker   
 - More tests needed


#### Usefull links:          
* [BV9600 4PDA thread (ru)](https://4pda.ru/forum/index.php?showtopic=917008) with lot of infos / files (stock ROM, TWRP)
* [SP Flash Tool Thread (ru)](https://4pda.ru/forum/index.php?showtopic=469340&st=26020)
* [Magisk Thread](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445)
* [My BV9600Pro's Overlay repo](https://github.com/Mel-kior/vendor_hardware_overlay/tree/master/Blackview/BV9600Pro/) (Help welcomed!)

## Steps to install

* Backup your personnal data and IMEI

> To go into fastboot or recovery keep `Vol+` and `power` down when starting your phone

* Install TWRP (after flashing dont reboot into the main system)
  * **Fastboot** :  
    * Install Mediatek USB driver and adb/fastboot utilities  
    * Open a console in the fastboot utility's folder  
    * Reboot your phone into fastboot and plug it
    * Unlock bootloader, flash TWRP image, lock back, reboot into the recovery :  
    ```bash
    fastboot oem unlock
    fastboot flash recovery recovery.img
    fastboot oem lock
    fastboot reboot recovery
    ```
  * **SP Flash Tool** :
    * Download and install MediaTek VCOM driver and SPFlashTool
    * Download Stock Image
    * In SPFlashTool go to the download tab and load the scatter file of the stock rom `MT6771_Android_scatter.txt`
    * Uncheck everything except recovery and change the recovery.img to the TWRP one.
    * Click `Download` and connect your powered off phone and let the flash go until green checkmark.
* Reboot directly into recovery and flash [Magisk](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445) if you want to go into the stock rom.   
  Without Root, stock rom remove TWRP and install back stock recovery!
* Boot into recovery:
  * Factory Wipe (data/cache/davlink) + System
  * Flash phh-tremble System image
  * [Optionnal] Copy [**treble-overlay-Blackview-BV9600Pro.apk**](https://github.com/Mel-kior/BV9600Pro_Overlay/raw/master/treble-overlay-Blackview-BV9600Pro.apk) in /system/overlay   
   > Overlay is raw copypasta from stock image and may need some tweak (for the notch especialy)

You can probably flash the system with fastboot or SP Flash Tool directly but I didn't test

## Hardware support

| Component                 |      Comment                                              | [Github Issues] |
|---------------------------|:---------------------------------------------------------:|:------:|
| Camera                    | Back : At least 1 Ok / Front : Ok                         |        |
| Speaker / Mic             | Main Speaker not working / "Call" speaker Ok / Mic Ok     | [Link] |
| Bluetooth                 | Not tested                                                |        |
| WiFi                      | Ok                                                        |        |
| SIM / Mobile Data / Voice | Not tested                                                |        |
| VoLTE                     | Not tested                                                |        |
| GPS                       | Ok                                                        |        |
| Fingerprint               | Ok                                                        |        |
| NFC                       | Not working                                               |        |
| Proximity sensor / Giro / Magnetic   | Ok / Ok                                        |        |
| Offline Charging          | Not working (or no animation)                             |        |
| Additional Side button    | Not Working (or not app to use it?)                       |        |
| Screen Notch              | No overlay config yet                                     |        |

---

Tested By:

* [@Mel-kior](https://github.com/Mel-kior) - BV9600Pro International (use in France) - AOSP 8.1v29 & 9v109 - 15/05/2019

Template created by @zguithues and @hackintosh5



[Github Issues]: https://github.com/phhusson/treble_experimentations/issues/

[Link]: https://github.com/phhusson/treble_experimentations/issues/417
