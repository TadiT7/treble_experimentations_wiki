

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

Assuming that you've already installed [Platform tools](https://developer.android.com/studio/releases/platform-tools) and is aware how to start the adb-fastboot shell , open platform tools in terminal/CMD (depending on os) and follow these steps ( Make sure that you've moved the appropriate vbmeta file you downloaded earlier in this guide to platform tools folder. Also move the phh/phh based gsi you've downloaded into platform tools folder and rename it to system.img )

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

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | works (for aux cams, enable aux cam expose toggle in phh settings)                                                    |
| Speaker / Mic             | working                                                   |
| Bluetooth                 | working                                                 |
| WiFi                      | working                                                    |
| SIM / Mobile Data / Voice | working (disable a2dp overload from phh settings else no call voice)                                                 |
| VoLTE                     | working (enable all three toggles in phh settings/ims)                                                    |
| Fingerprint               | silead works on Android 10 A23 vendor (et512 doesn't)                                                   |
| NFC                       | not available                                                   |
| Offline Charging          | works, but no animation                                                   |
|                                                   |
---

Tested By: [@realkarthiknair](https://realkarthiknair.github.io) - RMX2191/2193(India), A23 vendor - Date tested - 2021

