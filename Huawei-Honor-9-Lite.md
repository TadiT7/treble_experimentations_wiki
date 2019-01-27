# Huawei Honor 9 Lite

Most stuff works fine except every 5 seconds there are some green lines on the camera and offline charging is broken until https://github.com/phhusson/device_phh_treble/pull/77 gets merged.

## Steps to install

* [unlock your bootloader](https://forum.xda-developers.com/9-lite/how-to/unlock-bootloader-code-t3859685) ;
* reboot to fastboot (it should confirm you that the bootloader and FRP are both unlocked) ;
* flash this image (aonly arm64) with the `fastboot` utility:
    ```
    $ fastboot -w
    $ fastboot flash system system-arm64-aonly-type-type.img
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
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | Broken, of course                                         |
| Fingerprint               | OK                                                        |
| NFC                       | OK                                                        |
| Offline Charging          | Pending merge                                             |
---

Tested By: kaiomatico - LLD-L31(C432, so a German Device), Firmware 8.0.0.128 - 05/03/2018 and hackintosh5 - LLD-L31C432, firmware 8.0.0.132 - 27/01/2019 - Template created by @zguithues