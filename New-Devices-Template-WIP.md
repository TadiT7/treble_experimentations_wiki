# Device: Teclast M20_4G  (M3K1) 

Summary of what works: wifi,BT,camera,data(3g,4g,lte),adb-mtp,SD,charging,videos

## Steps to install

* Step 1 Turn ON oem unlock on the developer options - usb debugging On
  Step 2 unlock bootloader
* Step 3 fastboot erase system 
flash this image with the `fastboot` utility:
    ```
    $ a-command: fastboot -u flash system system-arm64-aonly-gapps-su.img
    $ fastboot reboot 
    ```
    Some more info: everything on my device works fine in aosp treble phh 8.1 - build V28 

    As an alternative you can flash via TWRP as "System Image" and format data.
      Yes,you can flash it via twrp 3.2.2-0 for chuwi hi9 air!! (same hardware-confirmed works)
## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Status      works                                              |
| Speaker / Mic             | Status      works                                             |
| Bluetooth                 | Status      works                                             |
| WiFi                      | Status      works                                             |
| SIM / Mobile Data / Voice | Status      works                                              |
| VoLTE                     | Status      ?(not support by my provider)                                            |
| Fingerprint               | Status       __(device not support)                                          |
| NFC                       | Status       __(device not support)                                            |
| Offline Charging          | Status       works                                             |
| Other feature             | Status       works                                            |
---

Tested By: hercules21 - Model-Number(region):M20_4G(M3K1), Firmware Version:M20_4G M3K1- V1.04_20180814 Date tested:2 Feb 2019 - Template created by @zguithues and @hackintosh5