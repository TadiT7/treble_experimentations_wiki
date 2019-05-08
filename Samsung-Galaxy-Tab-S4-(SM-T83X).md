# Device

Everything works, except stereo sound and s-pen optimizations.

## Steps to install

* Step 1
Flash ARK4 firmware. This is the one i tested with, newer versions should also be fine but i cannot guarantee.
* Step 2
Flash modesty kernel [from here](https://forum.xda-developers.com/galaxy-tab-s4/development/kernel-modesty-0-99-4-t3856088)
* Step 3
flash this image with the `fastboot` utility:
    ```
    $ a-command
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Mic working, Speaker: mono, only bottom speaker           |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working                                                   |
| Fingerprint               | N/A - Samsung Face Unlock does not work either (obviously)|
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | S-Pen works, displays as Mouse pointer                    |
---

## Fixes:

### S-Pen Mouse pointer: 

Add the following line to /system/usr/idc/sec_e-pen.idc
`touch.deviceType=touchscreen`

### Lock-Screen Rotation

Add the following line to /system/build.prop
`lockscreen.rot_override=true`
Make sure to set permissions of /system/build.prop to 0600 otherwise you will get stuck at the boot animation.

Tested By: mKenfenheuer - SM-T835 (Germany), Firmware Version ARK4 - 08.05.2019 - Template created by @zguithues and @hackintosh5