# [Blackview BV9500 Plus] - [s62v71c2k_jk_eea/MT6771V/CT]
## Calls, Camera (only primary and front facing), bluetooth, gps, Wireless charging all work.

## Steps to install

* Reboot to bootloader and connect via usb to PC (android debugging should be enabled):
    $ adb reboot bootloader
* Check if device is connected:
    $ fastboot devices
* flash this image with the `fastboot` utility:
    $ fastboot flash system system.img

## Hardware support

| Component                 | LineageOS 17.1 20200111   | AOSP 10.0 v209                 |
|---------------------------|---------------------------|--------------------------------|
| GPS                       | Working                   | Not tested                     |
| Camera                    | Working, Some rare issues in launching | Working, Front Cam Decent      |
| Speaker / Mic             | Working                   | Working                        |
| Bluetooth                 | Working                   | Working                        |
| WiFi                      | Working                   | Working                        |
| SIM / Mobile Data / Voice | Working, Tested SIM1 Only | Not Tested                     |
| Fingerprint               | Working                   | Not Working                    |
| Micro SD Card             | Working, Tested with 128GB A2| Not working                 |
---

## Additional Information
This device is A/B with VNDK version 28.0, choose arm64-ab when downloading an image.
Install Latest version of magisk by patching boot image.
Boot image for lineage 17.1 is in 
Flashed image via fastboot. Could not get TWRP working

## Test Results
  *  Lineage 17.1 20200111, Boots
  *  AOSP10v209  Boots (Goes into bootloop if Factory resent is done via AOSP)
 ***

Tested By: nobody666 - BV9500 Plus, 2020.02.20 - Template created by @zguithues and @hackintosh5