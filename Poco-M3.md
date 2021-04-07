# Poco M3 (Global)

Only found `bluetooth: audio 🎵` don't work.

## Steps to install

* Backup anything
* Unlock your `bootloader`
* Install `TWRP` or `OrangeFox` and boot to the non-original `fastboot` mode
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-<version>-arm64-<variants>.img
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ✅                                                        |
| Speaker / Mic             | ✅                                                        |
| Bluetooth                 | ✅ Pairing; ✅ File Sharing; ❌ Audio                      |
| WiFi                      | ✅                                                        |
| SIM / Mobile Data / Voice | ✅ (Tested /w 4G)                                         |
| VoLTE                     | Unknown                                                   |
| Fingerprint               | ✅                                                        |
| NFC                       | N/A                                                       |
| Offline Charging          | ✅                                                        |
| Other feature(s)          | ✅ 3.5 headset audio and mic and button jack              |
|                           | ✅ Magisk root                                            |
|                           | ✅ GPS                                                    |
|                           | ✅ Portable storage: SD card                              |
---

Tested By: [@edwining01](https://github.com/edwining01) - M2010J19CG(HK) - 20210407 - Template created by @zguithues and @hackintosh5

**!!!IF YOU'RE EDITING THIS TEMPLATE TO ADD YOUR DEVICE, CREATE ITS PAGE AND EDIT THERE, OTHERWISE YOU'LL DELETE THE TEMPLATE ITSELF!!!**