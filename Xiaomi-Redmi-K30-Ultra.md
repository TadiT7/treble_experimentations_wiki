# [Redmi K30 Ultra] - [cezanne]

## Tested images
?AOSP 10.0 v216

?AOSP 10.0 v217

√AOSP 10.0 v220

?AndyYan's LineageOS 17.1 20200511 (Doesn't Boot)

?Google GSI, Havoc, CrDroid, LineageOS (Credits Chaptsand from CoolApk, same w/ Xiaomi Mi 10 umi)

## Flashing instructions (similar to K30 Pro, no working TWRP currently available for this model)

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
| Display                   | √ |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √? at least partly working, will test further |
| VoLTE                     | ? |
| LED                       | ? |
| Fingerprint               | x Not working |
| NFC                       | ? |
| Offline Charging          | ? |
| IR                        | √ IR blaster works |

---

Redmi K30 Ultra Tested By:

Tom Golden (tbjgolden) @ Redmi K30 Ultra V12.0.8.0.QJNCNXM 
