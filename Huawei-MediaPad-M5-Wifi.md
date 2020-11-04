# Huawei MediaPad M5  (SHT-W09)

The [AOSP 10 image by phh](https://github.com/phhusson/treble_experimentations/releases/tag/v222) works ( i tested the gapps version v222)

I don't test Magisk for now, when i do i'll update this page.

## Steps to install

* Setup your system.
* Download an arm64 / ab variant of phh's AOSP 10 GSI.
* Download [the vbmeta.img file](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img).
* Flash the AOSP 10 GSI using [the method introduced here as "flashing a GSI without TWRP"](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/) with the command: 
`./fastboot flash system your_extracted_flavour.img`.
* Launch: `./fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`.
* wipe devik/cache/data with the standard Huawei recovery.



## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | working                                                   |
| Speaker / Mic             | working                                                   |
| Bluetooth                 | not tested yet                                            |
| WiFi                      | working                                                   |
| SIM / Mobile Data / Voice | not available                                             |
| VoLTE                     | not available                                             |
| Fingerprint               | working                                                   |
| Offline Charging          | not tested yet                                            |
---

Tested By: @attigliuzzo - Model-Number "SHT-W09 9.1.0.335(C432E3R1P2)" - Date tested: 03.11.2020
