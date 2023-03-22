# Device
well fingerprint and face unlock do not work
headphone jack needs a little fix with adb
brightness is kinda broken but you can fix it with adb too
auto brightness does not work

## Steps to install

* Step 1:
download any gsi you want as long as it's android 10 or lower (ARM64-A-only)
* Note:
the ones i tried are HavocOS(3.8), LineageOS(17/16), AOSP(8.1/9/10)
* Step 2
unlock bootloader using mtk client and flash twrp to your phone (phone does not have fastboot)
* Step 3
1.boot into TWRP and Install>System Image
2.go to Wipe>System>Resize Partition x2
3.wipe dalvik and cache and data partitions
4.boot into system

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                    |
| Speaker / Mic             | Working                                                    |
| Bluetooth                 | Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| Fingerprint               | Not Working                                                    |
| Offline Charging          | Working                                                    |
| Other feature             | Face Unlock Does not work                                                    |
---

Tested By: khalylexe - CPH1909-Europe, CPH1909EX_11_A.46 - 22/03/2023