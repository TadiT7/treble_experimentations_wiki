# [Nokia 1 Plus] - [ant]

## Hardware Support (AOSP 9)

Unable to flash due to small system partition (1,488 MB).

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |

***
## Additional Notes

### AOSP 10
For AOSP10, Only "arm32_binder64-ab-vanilla" flavor is known working.

You must wipe data / factory reset under stock recovery + stock ROM before flashing this treble GSI, don't use fastboot to erase userdata (either format userdata, -w or flash userdata are not acceptable). Otherwise you'll only get less than 1GB free storage space to use.

### AOSP 11 and AOSP 12

To install, follow these steps:
1. On stock ROM, use [Magisk (24.3 or newer)](https://github.com/topjohnwu/Magisk/releases/) to patch boot.img extracted from [last version of Android 11 OTA](https://android.googleapis.com/packages/ota-api/package/0abc215a4a29b1800c35cbc27fe36767a03b1977.zip). During installation, you should deselect "Forceencrypt" and select "patch vbmeta in boot image".
2. Pull the patched boot image out of your device.
3. Reboot to recovery mode and select wipe data/factory reset manually.
4. Reboot to bootloader mode and install OS.
```
fastboot flash boot magisk_patched-25200_XXXXX.img
fastboot flash system system-squeak-arm32_binder64-ab-vndklite-vanilla.img
fastboot reboot
```

***


## Tested By:

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 1 Plus TA-1111 00WW_0_980 @ 08/11/2019


Template created by @zguithues