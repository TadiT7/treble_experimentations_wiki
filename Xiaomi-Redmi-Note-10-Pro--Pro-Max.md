# Xiaomi Redmi Note 10 Pro / Pro Max

## Status as of 2021-05-03, with Android 11 GSI

Everything worked for me, except DT2W (Double Tap to Wake)

## Steps to install
- Educate yourself, read the [main page](https://github.com/phhusson/treble_experimentations), [Wiki](https://github.com/phhusson/treble_experimentations/wiki), [FAQ](https://github.com/phhusson/treble_experimentations/wiki/Frequently-Asked-Questions-%28FAQ%29), check the [issues](https://github.com/phhusson/treble_experimentations/issues)
- Backup all your data from the phone. They will be lost permanently when the phone is unlocked.
- Phone has to be unlocked, it is not an easy process: https://en.miui.com/unlock/
- Be on a factory ROM, to have a factory boot image. I've used: [V12.0.10.0 Indian ROM](https://bigota.d.miui.com/V12.0.10.0.RKFINXM/miui_SWEETININGlobal_V12.0.10.0.RKFINXM_13e6d3033e_11.0.zip)
- Download the GSI, and uncompress it.
- Get vbmeta.img from https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img
- From running Android, do adb reboot bootloader
- fastboot flash vbmeta vbmeta.img
- fastboot reboot fastboot
- fastboot flash system system-xxxx.img
- fastboot reboot recovery
- Once back in recovery, select "factory reset / wipe data"
- Reboot and enjoy

## Hardware support

| Component | Comment |
|-----------|---------|
| Front Camera | Works |
| Back Camera | Main, telephoto and wide Cameras works, did not test Marco lens |
| Speaker / Mic | Works |
| Bluetooth | Works |
| Wi-Fi | Works |
| SIM / Mobile Data / Voice | Works, dual SIM not tested |
| VoLTE | Works |
| Fingerprint | Works |
| Offline Charging | Works |

## Device specific Phh Treble Settings
- In Phh Treble settings, disable audio effects. This will fix the distorted audio 
- In Misc features, you can enable 120hz, Under force FPS

Tested By: aryan. - Redmi Note 10 Pro Max, V12.0.10.0.RKFINXM - 2021-05-03
 
Template created by @zguithues and @hackintosh5
