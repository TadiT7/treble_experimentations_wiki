# [Blackview BV9500 Plus] - [s62v71c2k_jk_eea/MT6771V/CT]
## Calls, Camera (only primary and front facing), bluetooth, gps, Wireless charging all work.

## Steps to install
### Warning!! 
  * There is no way to restore the phone back to its original state. I couldn't find the official firmware anywhere, and there is only one slot for each partition (not A/B).
**NOTE: If you want to install Magisk follow the steps below before proceeding with the installation of these GSI's
* With Android Debugging (ADB) enabled reboot to recovery via PC.
     `$ adb reboot bootloader`
* Check if device is connected via PC:
    `$ fastboot devices`
* If device is connected:
    `$ fastboot erase userdata`
    `$ fastboot erase system`
* flash this image with the `fastboot` utility:
    `$ fastboot flash system system.img`

## Hardware support

| Component                 | LineageOS 18.1 20210111      | AOSP 11.0 v308 (FLOSS)       | LineageOS R Mod v308         |
|---------------------------|------------------------------|------------------------------|------------------------------|
| Wireless Charging/Charging| Working                      | Working                      | Working                      |
| GPS                       | Working                      | Working                      | Working                      |
| Camera                    | Working, not secondary one   | Working, not secondary one   | Working, not secondary one   |
| Speaker / Mic             | Working                      | Working                      | Working                      |
| Bluetooth                 | Working                      | Working                      | Working                      |
| WiFi                      | Working                      | Working                      | Working                      |
| SIM / Mobile Data / Voice | Working, tested SIM1 only    | Working                      | Working                      |
| Fingerprint               | Working                      | Working                      | Working                      |
| Micro SD Card             | Working, tested with 128GB A2| Working, tested with 128GB A2| Working, tested with 128GB A2|
| GApps                     | Not working                  | Not tested                   | Not tested, Varient available|
| microG                    | Not working                  | Included, working            | Working                      |
| Magisk/Root               | Not working                  | phh-su, no magisk            | Magisk Included              |
---

## Additional Information
  * This device is A/B with VNDK version 28.0, choose arm64-ab when downloading an image.
  * Magisk not working. phh-su working.
  * Flashed image via fastboot. Could not get TWRP working
### Magisk Installation (via patched boot.img)
#### Android 10.1/LineageOS 17.1
  * Enable Android Debugging (ADB) and get into device via Terminal/Console.
     `$ adb shell`
  * Run the below command to extract the boot image:
     `$ dd if=/dev/block/by-name/boot  of=/sdcard/boot.img`
  * Using Magisk manager patch the boot.img.
  * Via fastboot flash the patched boot.img. Replace "patched_boot" with the name of your patched boot image.
     `$ fastboot flash boot patched_boot.img`
### GApps
#### LineageOS 17.1
  * Installed GApps onto Unofficial LineageOS 17.1 GSI 20200111 by copying play services and play store apk's to `system/priv-app/`
### microG
#### LineageOS R Mod v308
  * In order to get microG working proper we need to enable signature spoofing.
  * Follow this guide to enable signature spoofing - [LINK](https://forum.xda-developers.com/t/signature-spoofing-on-unsuported-android-11-r-roms.4214143/)
  * After you get signature spoofing enabled follow the same instructions for Android 10.1/LineageOS 17.1.
#### Android 10.1/LineageOS 17.1
  * To get microG working properly (Must have Magisk/Root completely installed and android debugging (ADB) enabled with rooted debugging enabled.
  * Installed microG onto Unofficial Lineage OS GSI 20200920. Follow official microG installation instructions from their page plus minor changes listed below.
  * Connect phone to PC and open a console/terminal and run:
     `$ adb shell`
  * Then Get su permissions:
     `$ su`
  * Grant SU permission to the shell and run this to give permission to the FakeStore/BlackStore:
     `# pm grant com.android.vending android.permission.FAKE_PACKAGE_SIGNATURE`
  * Reboot.
#### LineageOS 18.1
  * It is mentioned that signature spoofing is enabled in Andy Yan's builds of LineageOS 18.1 however I have not tested this.
  * If it is the case that signature spoofing is enabled then follow the same instructions for Android 10.1/LineageOS 17.1
## Test Results
  *  AOSP 11.0 v304 (FLOSS), Boots - Daily driver material.
  *  AOSP 11.0 v308 (FLOSS), Boots - Results above.
  *  LineageOS 17.1 20200111, Boots - Relatively Daily driver material sans Gapps.
  *  LineageOS 18.1 20210111, Boots - Results above.

## Notes
### LineageOS 18.1
  *  Signature spoofing only working for apps inside /system. Have not tested on methods to get microg working this way.
### AOSP 11.0 v300.i+
  *  Now comes with a FLOSS variant from v300i and later.

|Tested By: nobody666 - BV9500 Plus | 2021.06.05|