This device is arm64 A-only, but as explained [here on the wiki](https://github.com/phhusson/treble_experimentations/wiki), the device needs a GSI for A/B device.

## Android 10

-   AOSP 10.0 v221 GSI
-   Lineage OS 17.1 GSI

## Steps to install

You need to unlock your bootloader and flash a signed vbmeta image (the device uses dm-verity).
You can also use a boot image patched with the latest Magisk Canary build.

The bootloader doesn't accept full-sized images, you need to send it in pieces,
with the `fastboot` option `-S XXX`. I've found that the size need to be 250M or below.

-   reboot to fastboot
-   flash this image with the `fastboot` utility:

    ```
    $ fastboot erase system
    $ fastboot -S 250M flash system SYSTEM.img
    $ fastboot reboot
    ```

-   if not upgrading from a previous AOSP GSI, do a factory reset

I've not used TWRP, but it may work with it's `flash image` mode.

## Hardware support

| Component                 | Comment                |
| ------------------------- | ---------------------- |
| Camera                    | Working (front / back) |
| Speaker / Mic             | Working                |
| Bluetooth                 | Working                |
| WiFi                      | Working                |
| GPS                       | Not tested             |
| SIM / Mobile Data / Voice | Not tested             |
| VoLTE                     | Not tested             |
| SD card                   | Not tested             |
| Fingerprint               | No hardware            |
| NFC                       | No hardware            |


## Stock ROM

You can check the [official Teclast website](https://teclast.com), and download the ROMs there.
Most of them are on pan.baidu.com, but asking the support for another link worked for me.

---

Tested By: c0eos - P10_HD_ROW model N8H3, AOSP 10.0 v221 - 18/07/2020