# Huaiwei MediaPad M5 Pro

The [AOSP 10 image by phh](https://github.com/phhusson/treble_experimentations/releases/tag/v222) works without big troubles (gapps and vanilla)

Notable problems include: Magisk installation (found solution), some images are to big and can´t be flashed (didn´t find a solution yet), other things won´t be noticed till now, will be updated if there´s something new.

## Steps to install

* Download a arm64 / ab variant of phh's AOSP 10 GSI.
* Flash the AOSP 10 GSI using [the method introduced here as "flasing a GSI without TWRP".](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)
* Profit

TWRP support on this device isn´t given, so you´ve to patch recovery_ramdis.img by yourself, if you like to use Magisk, which isn´t a go on, because there´s no Custom Channel for phh Magisk files, or I was to blind at all. I opened an Issue [Magisk Custom Channel Issue #1480](https://github.com/phhusson/treble_experimentations/issues/1480)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | working                                                   |
| Speaker / Mic             | working                                                   |
| Bluetooth                 | not tested yet                                            |
| WiFi                      | working                                                   |
| SIM / Mobile Data / Voice | not tested yet                                            |
| VoLTE                     | not tested yet                                            |
| Fingerprint               | working                                                   |
| Offline Charging          | not tested yet                                            |
| Encryption                | working on Havoc-OS and RR                                |
---

Tested By: @PsyEng - Model-Number "CMR-AL19 9.0.1.347(C432)" - Date tested: 11-15.09.2020
