

## Instructions to install GSI on Narzo 20:

### 1. Unlock Bootloader

>Bootloader unlock tools    
For Realme UI 1 : [Get here](https://www.mediafire.com/file/4cy9u8r2yu9ve9t/DeepTest_realme_Narzo20.apk/file)  
For Realme UI 2 : [Get here](https://www.mediafire.com/file/8l33d9kxlxkdc80/DeepTesting_realme-release_20210426_newID_signed.apk/file)

>Vbmeta
For Realme UI 1 : [Get here](https://www.mediafire.com/file/0svn1vj1pn7buy7/vbmeta.img/file)  
For Realme UI 2 : [Get here](https://www.mediafire.com/view/instcb5n119uelv)

Guide to unlock bootloader : [Get here](https://telegra.ph/How-to-unlock-bootloader-03-02)

### 2. After unlocking bootloader and rebooting device, shut it down again and enter fastboot mode by pressing vol minus and power button together

Assuming that you've already installed [Platform tools](https://developer.android.com/studio/releases/platform-tools) and is aware how to start the adb-fastboot shell , open platform tools in terminal/CMD (depending on os) and follow these steps ( Make sure that you've moved the appropriate vbmeta file you downloaded earlier in this guide to platform tools folder. Also extract the phh/phh based gsi file you've downloaded and move the extracted img file into platform tools folder and rename it to system.img )

`adb reboot bootloader `  
`fastboot reboot fastboot`  
`# Your device will boot to recovery , dont touch anything in recovery, just focus on the commands below`  
`fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`  
`fastboot reboot fastboot`  
`fastboot erase system`  
`fastboot reboot fastboot`  
`fastboot flash system system.img`  
`fastboot -w`  
`fastboot reboot bootloader`  
`fastboot erase userdata`  
`fastboot reboot`  

Now in 99% of cases, if you didn't mess up anything, gsi will boot normally, Incase it doesn't,  you can either flash stock ROM using [this guide](https://www.mediafire.com/view/d7ygdwkqs46zw4b) or message me (who published this guide here) at [Instagram](http://instagr.am/harry_kris) or [telegram](https://t.me/realkarthiknair) . I'll try to help out if you've the basic common sense(s)

For extended support, join the narzo 20 community at telegram [here](https://t.me/realme_narzo_20_group)

## Hardware support

| Component                 | Over Realme UI 1 vendor (Android 10| Over Realme UI 2 vendor (Android 11)|Footnotes|
|---------------------------|-----------------------------------------------------------|-------------------------------------------------------------|---|
| Camera                    | working |working | 1. For aux cam support in third party apps like freedcam or gcam ports, enable aux cam expose toggle in phh settings <br> 2. You won't get fancy effects, 48 MP mode or even aux cam support in stock camera, for aux cam support and some advanced features, uses [this gcam ](https://www.mediafire.com/file/30meevjip83rm0d/narzo20Gcam7.apk/file) and [these ](https://www.mediafire.com/file/bqt78jr6p6kdudv/narzo20configsbyknair.xml/file)configs|
| Speaker / Mic             | working|working| sound quality isn't as impressive in GSIs out of the box like in  stock ROM, though it can be improved with tweaks and all|
| Bluetooth                 | working|broken in some cases including wireless headphones| I'll update this column if the issue(s) are fixed |
|headphone jack |working|working|incase doesn't work, turn on 'alternate headset detection' from settings/phh settings |
| WiFi                      | working|working- slightly buggy |I'll update this column if the issue(s) are fixed |
|Hotspot|working|Turns on, but no device can connect to |I'll update this column if the issue(s) are fixed |
| SIM / Mobile Data / Voice | working |working | If no sound in calls, disable a2dp overload from phh settings |
| VoLTE                     | working |working |**doesnt work** out-of-box, enable all three toggles in phh settings/ims for VoLTE to work |
| Fingerprint               | works if silead (only Android 10 A23 vendor) (et512 doesn't)|works if silead on all Android 11 vendors| use [this ](https://www.mediafire.com/file/szpnddw5ltm5gda/A11+EGIS_ET512+fix+for+realme+RMX2193.zip/file) magisk module to fix fp if et512 on android 10 A23 vendor|
| NFC                       | not NFC Hardware in Narzo 20 |not NFC Hardware in Narzo 20 | -|
| Offline Charging          | works | works| offline charging works, but no animation showing percentage |                                                   |
|                                                   |
---

Tested By: [@realkarthiknair](https://realkarthiknair.github.io) - RMX2191/2193(India), A23 vendor - Date tested - march 2021, C11 vendor - Date teseted - august 2021

