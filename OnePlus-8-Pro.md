# [OnePlus 8 Pro] - [instantnoodlep]

This device uses A/B partition.

## Tested images
√AOSP 11.0 v300.f

×AndyYan's LineageOS 18.0 20201008 (Doesn't Boot)

## Flashing instructions (You need to have the latest platform-tools and Android 11 firmware installed)

Reboot to bootloader:
```
adb reboot bootloader
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

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √; Stock camera apk supports main and front camera |
| Audio                     | √? Speaker and microphone is working, USB DAC untested. |
| Bluetooth                 | √? Bluetooth is recognized. Doesn't have a device to test |
| Display                   | √× High-res works with bug. Low-res works fine. 120hz works fine. |
| WiFi / Hotspot            | √? Hotspot not sure |
| GPS                       | √ |
| SIM / Mobile Data / Voice | ? (Device hardware broken, untested) |
| VoLTE                     | ? (Untested) |
| Fingerprint               | × (Recognizes fingerprint scanner exist, doesn't work) |
| NFC                       | ? (Untested) |
| Offline Charging          | × |

Device tested by:
lulujyc @ H2OS R Preview

Template created by @zguithues and @hackintosh5