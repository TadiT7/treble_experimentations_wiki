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
