# [Redmi K30 Ultra] - [cezanne]

## Tested images
?AOSP 10.0 v216

?AOSP 10.0 v217

√AOSP 10.0 v220

?AndyYan's LineageOS 17.1 20200511 (Doesn't Boot)

?Google GSI, Havoc, CrDroid, LineageOS (Credits Chaptsand from CoolApk, same w/ Xiaomi Mi 10 umi)
  
---
**[Updated Jan 2022]**

√[AndyYan's LineageOS 19.0 20220114](https://sourceforge.net/projects/andyyan-gsi/files/lineage-19.x/)

√[treble_build_pe v400.h self-build](https://github.com/AngelaCooljx/treble_build_pe/releases)

√[Yillié's ArrowOS v400.g](https://sourceforge.net/projects/gsi-projects/files/)

## Flashing instructions (similar to K30 Pro, no working TWRP currently available for this model)

**(Unlock through Xiaomi MI Unlock tool first, takes days :disappointed:)**

Reboot to bootloader:
```
adb reboot bootloader
```
Flash vbmeta with 
```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
``` 
Reboot to fastbootd
```
fastboot reboot fastboot
```
Flash system with
```
fastboot flash system system.img
```
Wipe data
```
fastboot -w
```
Reboot phone
```
fastboot reboot
```

### Another way to flash GSI on cezanne
Download [GSI-packer-tools](https://github.com/ChasonJiang/GSI-packer-tools/releases) and upzip it
  
Prepare a stock MIUI firmware(Android11 must)
  
Rename GSI to gsi.img, then copy the stock MIUI and it to the "input" directory in GSI-packer-tools
  
Click build.bat and choose '2'

Wait a minute and you will get a gsi_rom.zip in "output" directory
  
Flash it via twrp,and disabled-vbmeta.zip is a must
  
Magisk 23+ if you need, flash it before disabled-vbmeta.zip

# Important note about recovery

I had difficulties reflashing the stock MIUI rom with Mi Flash Tool, and other MTK flash tools as this processor is unsupported.

(For early builds like AOSP 10.0) To reflash stock MIUI use the V12.0.8.0 Recovery/Fastboot ROM [link](https://bigota.d.miui.com/V12.0.8.0.QJNCNXM/miui_CEZANNE_V12.0.8.0.QJNCNXM_1ae9faa171_10.0.zip)
  
**(For newer builds) To reflash stock MIUI use the V12.5.7.0 Recovery/Fastboot ROM [link](https://bigota.d.miui.com/V12.5.7.0.RJNCNXM/miui_CEZANNE_V12.5.7.0.RJNCNXM_207f23b3bf_11.0.zip), unzip and run the flash_all script for your operating system while your device is in fastboot mode.**

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √? Cameras work, front lift-camera needs [GSI-patch-cezanne](https://github.com/AngelaCooljx/GSI-patch-cezanne/releases) module |
| Audio                     | √? Speaker and microphone is working, otherwise untested |
| Bluetooth                 | √? Bluetooth Speaker works fine, In-call is untested. Try settings -- Phh Treble Settings -- Misc features -- Choose Force-disable A2DP offload  -- reboot |
| Display                   | √ Can be set to 120Hz in Phh Treble Settings, brightness slider broken |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √? LTE working, SMS working, 5G working with only NSA |
| VoLTE                     | ?  VOLTE working but conflicts to SMS |
| LED                       | √? it lights up |
| Fingerprint               | x Options exist but record failed |
| NFC                       | √ |
| Offline Charging          | ?x It didn't show a charging indicator, uncertain if it was charging |
| IR                        | √ IR blaster works |


---

Redmi K30 Ultra Tested By:

Tom Golden (tbjgolden) @ Redmi K30 Ultra V12.0.8.0.QJNCNXM 

AngelaCool (AngelaCooljx) @ Redmi K30 Ultra [V12.5.7.0.RJNCNXM](https://bigota.d.miui.com/V12.5.7.0.RJNCNXM/miui_CEZANNE_V12.5.7.0.RJNCNXM_207f23b3bf_11.0.zip) and newer version
