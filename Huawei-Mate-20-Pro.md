# Huawei Mate 20 Pro (UD) (LYA-AL10)

Installation instructions and tests

## Steps to install
###  Downgrade to EMUI 9.x and unlock the bootloader
(Software test points using DC-Phoneix and HCU clients etc...)  If you managed to get an unlock code back in 2019, that's worth a try too.
If you downgrade a device from EMUI 11 or above, you will need a harmony tp cable to reenable USB **2.0** transfer. Regular USB **3.0** cable might be OK (not tested).

If downgrading from EMUI 11,  Huawei SCP fast charging cannot be activated.

### Flash the image
`adb reboot bootloader`

`fastboot flash system Havoc-OS-v3.12-20201230-Official-arm64-ab.img`

Don't forget to do a factory reset in the stock recovery.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    |Works|
| Speaker / Mic / Calls     |Works|
| Bluetooth                 |Works|
| WiFi                      |Works|
| SIM / Mobile Data / Voice |Works with China Mobile sim card, others may need to set the access point correctly|
| VoLTE                     |Not tested|
| Fingerprint               |No, doesn't recognize the ud fingerprint sensor, see [Issue #468](https://github.com/phhusson/treble_experimentations/issues/468)|
| NFC                       |Not tested|
| USB transfer              |Same as when running EMUI 9 (*)|
| ADB                       |Works, but needs to manually set the authorization file (**)|

---
*If you downgrade to EMUI 9 and can use usb transfer before flashing the system image, you can still use it after flashing. If you can't before, you can't later。

**Copy the /data/misc/adb/ folder from another Android device that is authorized for debugging to this Android device that needs to be debugged, and then reboot.(recommended)  or  `setprop ro.adb.secure 0` (not recommended as it allows debugging from any computer and is not safe).

## Tested by
 @Cyanide-zh - EMUI 9.1.139 base [[Havoc-OS-v3.12-20201230-Official-arm64-ab.img.xz](https://sourceforge.net/projects/havoc-os/files/arm64-ab/Havoc-OS-v3.12-20201230-Official-arm64-ab.img.xz/download)] - Tested 2022.01.20 

_Template created by @zguithues and @hackintosh5_