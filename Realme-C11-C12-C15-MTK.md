# Realme C11/C12/C15 MTK

These three devices share very similar specs and share exactly same firmware. All three devices have Mediatek Helio G35.  
ARM64 A/B is the version of GSI which is compatible.

If we want VoLTE, then we have to downloaded AOSP v300j+ GSI(or based on this). For working of VoLTE in it, we have to do some steps after installing GSI. See GSI flashing guide for the steps.

## Steps to install

* Unlock Bootloader using [this](https://forum.xda-developers.com/t/guide-bootloader-unlock-realme-c12.4244957/)
* Flash GSI using [this](https://forum.xda-developers.com/t/gsi-phh-q-r-gsi-flashing-for-realme-c12.4244979/)

As of now flashing in [TWRP](https://forum.xda-developers.com/t/recovery-twrp-rmx2185-twrp-3-5-0-for-realme-c11.4236095/) is buggy, because of dynamic partitions. So only flash GSI with fastboot.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | N/A                                                    |
| Speaker / Mic             | Working                                                    |
| Bluetooth                 | Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| VoLTE                     | See notes                                                    |
| Fingerprint               | Not working                                                    |
| DoubleTapToWake               | Not working                                                    |
| Offline Charging          | N/A                                                    |

---

Not working components are tested in AOSP Roar v302 and AOSP Quack v222.

Tested By: HemanthJabalpuri  
Model(region) - RMX2189(India)  
Firmware Version - Android 10 A.83  
Date tested - 2nd March 2021
