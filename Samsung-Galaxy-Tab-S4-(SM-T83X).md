# Device

Everything works, except stereo sound and s-pen optimizations.

## Steps to install
1. Flash ARK4 firmware. This is the one i tested with, newer versions should also be fine but i cannot guarantee.<br />
You can get the German T835XXU2ARK4 firmware (Oreo) here:<br /> 
https://www.sammobile.com/samsung/galaxy-tab-s4/firmware/SM-T835/DBT/<br />
That website also includes instructions about flashing the device using Odin, which is a windows application. Unfortunately, heimdall (https://glassechidna.com.au/heimdall/) does not support this device.

2. install TWRP:  https://twrp.me/samsung/samsunggalaxytabs4qcom.html<br />
You can use Odin to install TWRP.  Remember to boot immediately into recovery after flashing TWRP and wipe userdata, otherwise the stock recovery image may be re-flashed when you boot the stock system image.

3. Flash modesty kernel [from here](https://forum.xda-developers.com/galaxy-tab-s4/development/kernel-modesty-0-99-4-t3856088)<br />
The modesty kernel has updated fstab entries in its device-tree that disable verity checks.  The GSI won't boot unless the system-image verity check is disabled.

4. reboot into TWRP and flash an oreo arm64 a-only gsi:
  ```
  # use the TWRP ui to mount /data.  You may need to do Wipe \ Format Data first.
  $ adb shell mkdir -p /data/local/tmp
  $ adb push system-arm64-aonly-gapps-su.img /data/local/tmp
  # now use the TWRP ui to flash this image (it is under the "Install" menu)
  # reboot
  ```

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
`lockscreen.rot_override=true`  (this no longer seems to be necessary)
Make sure to set permissions of /system/build.prop to 0600 otherwise you will get stuck at the boot animation.  (this no longer seems to be necessary)

Tested By: @mKenfenheuer - SM-T835 (Germany), Firmware Version ARK4 - 08.05.2019

Updated by @jamuir

Template created by @zguithues and @hackintosh5