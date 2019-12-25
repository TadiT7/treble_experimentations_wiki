# Device

BV9600Pro International version<br>
Stock Firmware : BV9600Pro_S700_V1.1_20190104V45<br>
Tested phh's *AOSP 8.1 v29* and *AOSP 9 v109*<br>
<br>
OR<br>
<br>
BV9600Pro International version with Helio P60 hw rev2 (MT6771V/CT)<br>
Stock Firmware : BV9600Pro_EEA_S700_V1.0_20190530V8 (Android 9)<br>
Tested phh's *AOSP 10 v208* (gapps&vanilla flavours)<br>


#### Actual status (15/05/2019):
 - Booting is long (30+ min) but go trough  
 - Some rare freezes and ui crashes
 - No main speaker   
 - More tests needed
#### Actual status (25/12/2019):
 - Booting takes few seconds.
 - GAPPS version has ui glitches on animations
 - No main speaker, no main camera
 - More tests needed

#### Usefull links:          
* [BV9600 4PDA thread (ru)](https://4pda.ru/forum/index.php?showtopic=917008) with lot of infos / files (stock ROM, TWRP)
* [SP Flash Tool Thread (ru)](https://4pda.ru/forum/index.php?showtopic=469340&st=26020)
* [Magisk Thread](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445)
* [My BV9600Pro's Overlay repo](https://github.com/Mel-kior/vendor_hardware_overlay/tree/master/Blackview/BV9600Pro/) (Help welcomed!)
* [Treble Info](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck)
 
## Steps to install

* Backup your personal data and IMEI
* Check your partition table layout A or A/B (depending on Stock used 8.1 or 9) with [Treble Info](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck) app and choose correct system image

> To go into fastboot or recovery keep `Vol+` and `power` down when starting your phone

* Install TWRP (after flashing don't reboot into the main system)
  * **Fastboot** :  
    * Install Mediatek USB driver and adb/fastboot utilities  
    * Open a console in the fastboot utility's folder  
    * Reboot your phone into fastboot and plug it
    * Unlock bootloader (or flashing non-critical partitions), flash TWRP image, lock back (optional?), reboot into the recovery:  
`fastboot oem unlock`<br>
`fastboot flash recovery recovery.img`<br>
`fastboot oem lock`<br>
`fastboot reboot recovery`<br>
or<br>
`fastboot flashing unlock`<br>
`fastboot flash recovery recovery.img`<br>
`fastboot reboot recovery`<br>

  * **SP Flash Tool** :
    * Download and install MediaTek VCOM driver and SPFlashTool
    * Download Stock Image
    * In SPFlashTool go to the download tab and load the scatter file of the stock rom `MT6771_Android_scatter.txt`
    * Uncheck everything except recovery and change the recovery.img to the TWRP one.
    * Click `Download` and connect your powered off phone and let the flash go until green check-mark.
* Reboot directly into recovery and flash [Magisk](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445) if you want to go into the stock rom.   
  Without Root, stock rom remove TWRP and install back stock recovery!
* Boot into recovery:
  * Factory Wipe (data/cache/dalvik) + System
  * Flash correct phh-treble System image
  * [Optional] Copy [**treble-overlay-Blackview-BV9600Pro.apk**](https://github.com/Mel-kior/BV9600Pro_Overlay/raw/master/treble-overlay-Blackview-BV9600Pro.apk) in /system/overlay   
   > Overlay is raw copypasta from stock image and may need some tweak (for the notch especially)

You can probably flash the system with fastboot or SP Flash Tool directly but I didn't test.<br>
//25.12.2019 Tested. Flashing system directly with SP_Flash_Tool_v5.1916_Linux works. [@AreYouLoco?](https://github.com/AreYouLoco)

## Hardware support

| Component                 | Comment (tested by [@Mel-kior](https://github.com/Mel-kior)) |
Comment (tested by [@AreYouLoco?](https://github.com/AreYouLoco)) | [Github Issues] |
|---------------------------|:---------------------------------------------------------:|:---------------------------------------------------------:|:------:|
| Camera                    | Back: At least 1 Ok / Front: Ok                         | Back: Not working / Front: Ok                         |        |
| Speaker / Microphone             | Main Speaker: Not working / "Call" Speaker: Ok / Mic: Ok     | Main Speaker: Not working / "Call" Speaker: Not tested / Mic: Ok     | [Link] |
| Bluetooth                 | Not tested                                                | Ok? (Turns on, detects devices, but disconnects randomly. Audio stream works tho!)                                                |        |
| WiFi                      | Ok                                                        | 5GHz: Ok / 2.4Ghz: Ok                                                      |        |
| SIM / Mobile Data / Voice | Not tested                                                | Not tested                                                |        |
| VoLTE                     | Not tested                                                | Not tested                                                |        |
| GPS                       | Ok                                                        | Not tested                                                |        |
| Fingerprint               | Ok                                                        | Ok                                                |        |
| NFC                       | Not working                                               | Ok? (Other phone could detect tag) / Payment: Not tested                                               |        |
| Proximity sensor / Giro / Magnetic / Pressure   | Ok / Ok                                        | Not working / Ok / Ok / Not working                                      |        |
| Offline Charging          | Not working (or no animation)                             | Not tested         |
| Additional Side button    | Not Working (or not app to use it?)                       | Ok (works with [Keyboard/Button Mapper](https://f-droid.org/app/io.github.sds100.keymapper))    |
| Screen Notch              | No overlay config yet                                     | No overlay config yet                                     |        |
| Flashlight              | n/a                                  | Not working (Back camera related?)                                   |        |

---

Tested By:

* [@Mel-kior](https://github.com/Mel-kior) - BV9600Pro International (used in France) - AOSP 8.1v29 & 9v109 - 15/05/2019
* [@AreYouLoco?](https://github.com/AreYouLoco) - BV9600Pro International (with stock based on Android 9, used in Poland) - AOSP 10v208 (gaaps&vanilla) - 25/12/2019

Template created by @zguithues and @hackintosh5



[Github Issues]: https://github.com/phhusson/treble_experimentations/issues/

[Link]: https://github.com/phhusson/treble_experimentations/issues/417
