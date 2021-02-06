# [Blackview BV9500 Plus] - [s62v71c2k_jk_eea/MT6771V/CT]
## Calls, Camera (only primary and front facing), bluetooth, gps, Wireless charging all work.

## Steps to install
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

| Component                 | LineageOS 18.1 20210111   | AOSP 11.0 v300.m (FOSS)         |
|---------------------------|---------------------------|--------------------------------|
| Wireless Charging/Charging| Working                   | Working                        |
| GPS                       | Working                   | Working                    |
| Camera                    | Working, not second camera| Working, Front Cam Decent      |
| Speaker / Mic             | Working                   | Working                        |
| Bluetooth                 | Working                   | Working                        |
| WiFi                      | Working                   | Working                        |
| SIM / Mobile Data / Voice | Working, tested SIM1 only | Working                        |
| Fingerprint               | Working                   | Working                        |
| Micro SD Card             | Working, tested with 128GB A2| Working, tested with 128GB A2  |
| GApps                     | Not working                  | Not tested                     |
| microG                    | Not working                | Included, working              |
| Magisk                    | Not working                   | phh-su, no magisk              |
---

## Additional Information
  * This device is A/B with VNDK version 28.0, choose arm64-ab when downloading an image.
  * Magisk not working. phh-su working.
  * Flashed image via fastboot. Could not get TWRP working
### Magisk Installation (via patched boot.img) (Android 10.1/LineageOS 17.1 only)
  * Enable Android Debugging (ADB) and get into device via Terminal/Console.
     `$ adb shell`
  * Run the below command to extract the boot image:
     `$ dd if=/dev/block/by-name/boot  of=/sdcard/boot.img`
  * Using Magisk manager patch the boot.img.
  * Via fastboot flash the patched boot.img. Replace "patched_boot" with the name of your patched boot image.
     `$ fastboot flash boot patched_boot.img`
### GApps
  * Installed GApps onto Unofficial Lineage OS GSI 20200111 by copying play services and play store apk's to `system/priv-app/`
### microG (Android 10.1/LineageOS 17.1 only)
  * To get microG working properly (Must have Magisk  completely installed and android debugging (ADB) enabled with rooted debugging enabled.
  * Installed microG onto Unofficial Lineage OS GSI 20200920. Follow official microG installation instructions from their page plus minor changes listed below.
  * Connect phone to PC and open a console/terminal and run:
     `$ adb shell`
  * Then Get su permissions:
     `$ su`
  * Grant SU permission to the shell and run this to give permission to the FakeStore/BlackStore:
     `# pm grant com.android.vending android.permission.FAKE_PACKAGE_SIGNATURE`
  * Reboot.
## Test Results
  *  LineageOS 18.1 20210111, Boots - Results above.
  *  AOSP 11.0 v300.m (FOSS), Boots - Results above.
  *  Lineage 17.1 20200111, Boots - Results above.
## Notes
  *  Signature spoofing not working on LineageOS 18.1/ Cannot manually patch either.

Tested By: nobody666 - BV9500 Plus, 2021.02.05