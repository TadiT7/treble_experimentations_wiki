# Huawei Honor 9 Lite

Most stuff works fine except every 5 seconds there are some green lines on the camera and SafetyNet does not pass (not even on the nosu variant and also not by installing magisk 16.4, because it says the boot image is already patched and magisk manager force closes).

## Steps to install

* [unlock your bootloader](https://forum.xda-developers.com/honor-7x/how-to/how-to-unlock-huawei-bootloader-removal-t3780903) ;
* enable developer settings and disable OEM/FRP lock ;
* reboot to fastboot (it should confirm you that the bootloader and FRP are both unlocked) ;
* [build your Generic Standard Image (GSI)](https://github.com/phhusson/treble_experimentations/wiki/How-to-build-a-GSI);
* flash this image with the `fastboot` utility:
    ```
    $ fastboot -w
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    The device will bootloop 3 times. This is FINE! After the third boot the recovery tells you that the data partition has to be low level formatted. Click on okay and after that the device will boot just fine! :)

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Issue: every ~5 seconds there are minor green lines.      |
| Camera                    | OK                                                        |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| Wifi                       | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | Unknown                                                   |
| Fingerprint               | OK                                                        |

---

Tested By: kaiomatico - LLD-L31(C432, so a German Device), Firmware 8.0.0.128 - 05/03/2018 - Template created by @zguithues