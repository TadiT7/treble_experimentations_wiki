# [Redmi K30 5G] - [picasso]

Although this device is A-only, you have to choose GSI for A/B devices because this device is "system-as-root". 

## Tested images
√AOSP 10.0 v219 

## Flashing instructions (Credits phhusson and Akito)

- make sure to have the [latest platform-tools](https://developer.android.com/studio/run/win-usb) installed.

- Retrive vbmeta.img and recovery.img from official packages.

- Reboot to bootloader:
```
adb reboot bootloader
```
- Flash vbmeta with 
```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
``` 
- Flash stock recovery if using wzsx150's unofficial TWRP
```
fastboot flash recovery recovery.img
```
- Reboot to fastbootd
```
fastboot reboot fastboot
```
- Check device status with `fastboot devices`. Linux may run into problem with udev, and I wrote 
```
$ cat /etc/udev/rules.d/20-k30.rules
SUBSYSTEM=="usb", ATTR{idVendor}=="0000", MODE="0666", GROUP="plugdev"
```
and reboot to fix the permission issue. Windows users may need to install driver manually.

- Flash you downloaded gsi system.img with
```
fastboot flash system gsi-system.img
```
- Wipe data
```
fastboot -w
```
- Reboot phone
```
fastboot reboot
```
- Enjoy!
## Hardware support (Referred from Redmi K20 Pro)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √? (Front and rear cameras work, need to test more lenses) |
| Audio                     | √x (Need to disable audiofx, speaker and microphone is working,  3.5mm audio jack needs flag of using alternative audio policy, bt audio is not working) |
| Bluetooth                 | √x (Bluetooth keyboard works fine, Audio not working.) |
| Display                   | √ (120fps needs unlock) |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √× Dual Sims works, 5G data works, call and messages might be an issue. |
| VoLTE                     | x (No option present) |
| LED                       | x (Not Working) |
| Fingerprint               | √× (Works, Glitched with vanilla kernel, register fp as input event, can be fixed with flashing kernel) |
| NFC                       | ? (Not tested) |
| Offline Charging          | ? (Not tested)|

## Additional Note

Should downgrade if you're on MIUI12, since MIUI12 changes the partition table, system partition becomes super, and flashing AOSP10 directly to super bricks the device by bootloop.

---

This wiki page is referred from Xiaomi Redmi K30 Pro (lmi) page by @lulujyc as this device have a lot of things in common with in.

Redmi K30 5G Tested By: 

R-L-T-Y @ picasso_images_V11.1.25.0.QGICNXM_20200511.0000.00_10.0_cn

Template created by @zguithues and @hackintosh5

MIUI12 note by @peter17ji