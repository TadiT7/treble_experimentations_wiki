# Xiaomi Redmi K20 / Mi 9T - davinci

## Status as of 2021-04-18, with Android 11 GSI

Most things work, except device specific hardware:

- Under-screen fingerprint reader
- Pop-up Camera up-down function (see below for workaround)
- Multiple back cameras
- Auto backlight
- Battery usage data isn't available (percent is OK, just app usage, system usage data isn't there)

## Steps to install
- Educate yourself, read the [main page](https://github.com/phhusson/treble_experimentations), [Wiki](https://github.com/phhusson/treble_experimentations/wiki), [FAQ](https://github.com/phhusson/treble_experimentations/wiki/Frequently-Asked-Questions-%28FAQ%29), check the [issues](https://github.com/phhusson/treble_experimentations/issues)
- Backup all your data from the phone. They will be lost permanently when phone is unlocked.
- Phone has to be unlocked, it is not an easy process: https://en.miui.com/unlock/
- Be on a factory ROM, to have a factory boot image. Don't use xiaomi.eu ROMs. I've used: [V12.0.7.0 Global ROM](https://bigota.d.miui.com/V12.0.7.0.QFJMIXM/miui_DAVINCIGlobal_V12.0.7.0.QFJMIXM_9866f56704_10.0.zip) from [this page](https://c.mi.com/oc/miuidownload/detail?device=1700361)
- flash this image with the fastboot utility:
    $ fastboot flash system  system-roar-arm64-ab-vndklite-gapps.img
- Backup, if you have data on the phone, then do a factory reset before/after installation, to have a clean /data partition.

## Hardware support

| Component | Comment |
|-----------|---------|
| Front Camera | Works, see below |
| Back Camera | Main Camera works, cannot switch to other cameras |
| Speaker / Mic | Works see settings below|
| Bluetooth | Works |
| WiFi | Works |
| SIM / Mobile Data / Voice | Works, dual SIM not tested |
| VoLTE | Not tested |
| Fingerprint | Not supported on Android 11 GSI |
| NFC | Works |
| Offline Charging | Works |

## Pop-up camera 

It can be controlled from command line or ADB with root rights:

| Function | Command |
|----------|---------|
| pop-up | # xiaomi-motor popup 1 |
|takeback (down) | # xiaomi-motor takeback 1 |

## Device specific Phh Treble Settings

| Menu | Item |
|------|------|
| Qualcomm features | Use alternate audio policy |
| Xiaomi features | Enable D2TW (Double tap to wake) |
| Misc features | Force alternative backlight scheme |

## Other

ROM defaults to 3G, it can be set at Settings, Network and Internet, Mobile Network, Preferred network type. I've selected LTE/TDSCDMA/GSM/WCDMA to have LTE, GSM, and WCDMA (3G)

Tested By: Laszlo-Fiat - Mi 9T(Global), V12.0.7.0.QFJMIXM - 2021-04-18 - Template created by @zguithues and @hackintosh5