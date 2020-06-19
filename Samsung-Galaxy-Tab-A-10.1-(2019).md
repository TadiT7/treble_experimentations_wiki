# Samsung Galaxy Tab A 10.1 (2019) [SM-T510/T515]

Running pretty well overall, and I have a fix for offline charging.

## Steps to install

* Unlock bootloader
* Hold Power & Vol Up buttons during restart to enter stock recovery
* Wipe data/factory reset
* Reboot to bootloader
* Install [TWRP](https://forum.xda-developers.com/galaxy-tab-a/development/recovery-twrp-3-3-1-2019-galaxy-tab-10-1-t3934805) to AP with Odin
* Hold Power & Vol Up buttons during restart to enter TWRP recovery
* Install [latest Multidisabler](https://forum.xda-developers.com/galaxy-tab-a/development/sm-t510-t515-multidisabler-encryption-t3963020) from TWRP
* Wipe data/factory reset
* Install arm32_binder64-ab image to system partition
* Reboot to system

Some more info:
* Alternatively, you can flash [Nexus Stock custom ROM](https://forum.xda-developers.com/galaxy-tab-a/development/rom-nexus-stock-2019-galaxy-tab-10-1-t3944222), which is based on latest AOSP build and includes the [MTP fix](https://forum.xda-developers.com/showpost.php?p=76453315&postcount=245).

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | SM-T515 only                                              |
| VoLTE                     | Unknown                                                   |
| Fingerprint               | N/A                                                       |
| NFC                       | N/A                                                       |
| Offline Charging          | Hangs on state-of-charge animation                        |
| MTP                       | Kernel fix required                                       |
---

Tested By: Magendanz - SM-T510(XAR), Firmware Version T510XXU1ASEF - 20190909