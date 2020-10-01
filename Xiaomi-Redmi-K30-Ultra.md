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
| Camera                    | √× Cameras work, but front camera does not popup at all [1] |
| Audio                     | √? Speaker and microphone is working, USB Type C DAC is working, 3.5mm audio jack is not working. |
| Bluetooth                 | √? Bluetooth Speaker works fine, In-call is untested. |
| Display                   | √ |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √× Internet Data works, call works, expect messages to be NOT working. |
| VoLTE                     | ? (Untested) |
| LED                       | √? Working, unsure about the second LED [Need more testing]. |
| Fingerprint               | √× (Recognition a little slower maybe due to system setting; Unlocking from off/AOD state not supported, need press power button first, not working since 216+) |
| NFC                       | √? (Support card info reading via NXP.TagInfo, need more tests like card writing / simulation) |
| Offline Charging          | × |

## Additional Note

1. Terminal command for manually controlling the front camera motor (may require `su` depending on the GSI):

Popup: `xiaomi-motor popup 1`

Retract: `xiaomi-motor takeback 1`

---

Redmi K30 Ultra Tested By:

Tom Golden (tbjgolden) @ Redmi K30 Ultra V12.0.8.0.QJNCNXM 
