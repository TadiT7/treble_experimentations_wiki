Enable OEM unlocking in developer settings.

```
adb reboot bootloader
fastboot flashing unlock
# this may be unnecessary
fastboot flashing unlock-critical
fastboot reboot fastboot
# from https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img, may be unnecessary
fastboot --disable-verification flash vbmeta vbmeta.img
fastboot flash system system-roar-arm64-ab-vanilla.img
fastboot reboot
```

If you get `Writing 'system' FAILED (remote: 'This partition doesn't exist')` then you are probably in the wrong fastboot mode (there is more than one), where you get 1 small line of text on a black screen. `fastboot reboot fastboot` reboots into the right one where you get a bootmenu that says "fastbootd" at the top. You can flash while at the menu, no need to choose an option.

With the 12.1 floss image my system partition was too small, but after deleting the product partition I could flash:
```
$ fastboot flash system system-squeak-arm64-ab-floss-12.1-v416.img
Resizing 'system'                                  FAILED (remote: 'Not enough space to resize partition')
fastboot: error: Command failed
$ fastboot delete-logical-partition product
Deleting 'product'                                 OKAY [  0.010s]
Finished. Total time: 0.010s
```


## Hardware Support

* Camera:
> Working

* Speaker / Microphone
> Working

* Bluetooth
> Working

* Wifi
> Working

* SIM / Mobile Data / Voice
> Not tested

* VoLTE
> Not tested

* Fingerprint Reader
> Not tested

* Wifi-Router
> Not tested
