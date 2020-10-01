# [Redmi K30 Ultra] - [cezanne]

## Tested images
?AOSP 10.0 v216

?AOSP 10.0 v217

√AOSP 10.0 v220

?AndyYan's LineageOS 17.1 20200511 (Doesn't Boot)

?Google GSI, Havoc, CrDroid, LineageOS (Credits Chaptsand from CoolApk, same w/ Xiaomi Mi 10 umi)

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

# Important note about recovery

I had difficulties reflashing the stock MIUI rom with Mi Flash Tool, and other MTK flash tools as this processor is unsupported.

To reflash stock MIUI use the V12.0.8.0 Recovery/Fastboot ROM [link](https://bigota.d.miui.com/V12.0.8.0.QJNCNXM/miui_CEZANNE_V12.0.8.0.QJNCNXM_1ae9faa171_10.0.zip), unzip and run the flash_all script for your operating system while your device is in fastboot mode.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √× Cameras work, but front camera does not popup at all, even using xiaomi-motor commands |
| Audio                     | √? Speaker and microphone is working, otherwise untested |
| Bluetooth                 | ? Bluetooth Speaker works fine, In-call is untested. |
| Display                   | √ Can be set to 120Hz in Phh Treble Settings, brightness slider broken |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √x LTE working, SMS working, 5G not working [1] |
| VoLTE                     | ? untested |
| LED                       | √? it lights up |
| Fingerprint               | x Not working |
| NFC                       | ? |
| Offline Charging          | ?x It didn't show a charging indicator, uncertain if it was charging |
| IR                        | √ IR blaster works |

## Notes

[1] Had to set preferred network type to LTE. While 5G is listed as an option, it doesn't work (`Invalid network mode 26. Ignore.`)

---

Redmi K30 Ultra Tested By:

Tom Golden (tbjgolden) @ Redmi K30 Ultra V12.0.8.0.QJNCNXM 