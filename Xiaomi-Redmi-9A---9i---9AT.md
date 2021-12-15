# Xiaomi Redmi 9A/9i/9AT
![](https://i.imgur.com/5YVQScz.png)

Currently this device only have 2 working custom recovery, TWRP LR and PitchBlack Recovery.

# Requirements
* Stock recovery
* vbmeta.img
* PC/Laptop that have ADB and Fastboot drivers installed

You can find those recovery and vbmeta on stock firmware file. Download [here](https://xiaomifirmwareupdater.com/miui/dandelion/) and extract.

## How to flash GSI?
Firstly, choose a GSI image you want to install according to the Android version and the architecture of our device. Redmi 9A uses A64 A/B variant (arm32 Binder 64 A/B), so make sure you are using A64/Binder64 GSI not arm64 GSI else it doesn't booted! After that, you should extract it to your desired location, then move it to the ADB location and rename the image file as 'system.img'.

Now reboot your device into recovery mode!
* Using key combination ( shut down the device first )
```
Power key + volume up
```
* Using ADB command
```
adb devices
adb reboot recovery
```
After you are in MIUI Recovery, do wipe data and reboot again to fastboot mode.

Now reboot your device into fastboot mode!
* Using key combination ( shut down the device first )
```
Power key + volume up
```
* Using ADB command
```
adb devices
adb reboot bootloader
```

Then plug it into your PC and then execute these codes in the command prompt. Use vbmeta that you already extract from stock firmware.
```
fastboot devices
fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img
fastboot reboot fastboot
```
Now, your Redmi 9A/9i are in yellow fastboot mode (fastbootd). After that, do these steps onward.
```
fastboot flash system system.img
fastboot reboot
```
Voila! You have successfully managed to flash a GSI ROM to your Redmi 9A device!

### Working GSI
* Tested [CrDroid v313 by eremitein](https://sourceforge.net/projects/treblerom/files/crDRom11/2021.09.21/)
* Tested [Bless v306 by eremitein](https://sourceforge.net/projects/treblerom/files/BLESS11/2021.05.02/)
* Tested [phh GSI](https://github.com/phhusson/treble_experimentations/releases)
* Every [eremitein](https://sourceforge.net/projects/treblerom/files/) builds

## Hardware support

| Component                 |   |   Comment                                              |
|---------------------------|---|-------------------------------------------------------|
| Camera                    | √ |
| Audio                     | √/×| (headphone jack doesn't work, but can be fixed with a simple code on termux) |
| Bluetooth                 | √ |
| Display                   | √ |(brightness slider doesn't work / can also be fixed via termux) |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | × |(RIL dead in GSI Phh of A11 and A12, only in GSI of Eremitein works) |
| VoLTE                     | ? |(Untested) |
| Fingerprint               | √ |
| Offline Charging          | × |

### Fixes

To fix the earphone issue, execute these lines on any Terminal Emulator (preferably Termux) then reboot.
```
su
setprop persist.sys.overlay.devinputjack true
```

For brightness, please also execute these lines on any Terminal Emulator. 

```
setprop persist.sys.qcom-brightness $(cat /sys/class/leds/lcd-backlight/max_brightness)
```
If you still don't understand, you can join this telegram group! [Redmi 9A GSI](https://t.me/Redmi9Achat)

## Credits
* [Brahm Daniel Verano](https://github.com/liafourte) for this template
 