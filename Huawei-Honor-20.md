# Huawei Honor 20 (YAL-AL00)

Installation instruction and tests

## Steps to install
###  Downgrade to Magic UI 2.1 and unlock the bootloader
(Software test points using DC-Phoneix and HCU clients etc...)  If you managed to get an unlock code, that's worth a try too.
If you downgrade a device from EMUI 11 (errr maybe not this name on an Honor device) or above, you will need a harmony tp cable to reenable USB **2.0** transfer. Regular USB **3.0** cable is OK.

If downgrading from EMUI 11,  Huawei SCP fast charging cannot be activated.

### Flash the image
`adb reboot bootloader`

`fastboot flash system Havoc-OS-v3.12-20201230-Official-arm64-ab.img`

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    |Works|
| Speaker / Mic / Calls     |Works|
| Bluetooth                 |Works|
| WiFi                      |Works|
| SIM / Mobile Data / Voice |Works with China Mobile sim card, others may need to set the access point correctly|
| VoLTE                     |Not tested|
| Fingerprint               |Works|
| NFC                       |Not tested|
| USB transfer              |Same as when running Magic UI 2.1|
| ADB                       |Works, but needs to manually set the authorization file|
---

## Tested by
* @Cyanide-zh - Magic UI 2.1 version 9.1.143 base [[Havoc-OS-v3.12-20201230-Official-arm64-ab.img.xz](https://sourceforge.net/projects/havoc-os/files/arm64-ab/Havoc-OS-v3.12-20201230-Official-arm64-ab.img.xz/download)] - Tested 2022.07.30 

_Template created by @zguithues and @hackintosh5_