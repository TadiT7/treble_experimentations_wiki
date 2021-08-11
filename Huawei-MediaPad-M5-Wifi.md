# Huawei MediaPad M5  (SHT-W09)

UPDATE 11/08/2021: roar-311-arm64-ab-gapps.img boots fine, most things work, but video doesn't play from within Chrome, due to what looks like problems with hardware video decoding.  This is a long standing issue, and likely to affect all previous builds also.  It's a showstopper for me sadly.

UPDATE 26/04/2021: Roar-306-vanilla-AB-arm64-vndklite boots, it has no offline charging and i cannot set lower brightness. Install DavX from F-droid if you need to sync contacts/cal. events from google and the aurorastore to access to the google store.

UPDATE 09/12/20: flashed Roar AB, arm64, gapps version v300.j and it boots

The [AOSP 10 image by phh](https://github.com/phhusson/treble_experimentations/releases/tag/v222) works (i tested the gapps version v222)

I don't test Magisk for now, when i do i'll update this page.

## Steps to install

* Setup your system.
* Download an arm64 / ab variant of phh's AOSP 10 GSI.
* Download [the vbmeta.img file](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img).
* Flash the AOSP 10 GSI using [the method introduced here as "flashing a GSI without TWRP"](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/) with the command: 

`fastboot flash system your_extracted_flavour.img`.

* Launch: `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`.
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
| Offline Charging          | not working                                               |
| Fast Charging             | working                                                   |
| Hardware Video Decoding   | not working                                               |

## Power save Google play service without magisk
I think to have enabled battery saver for GMS. I simply edited the file google.xml stored in /System/product/etc/sysconfig. I commented these 2 string adding `<!--    -->`, so:

`<!-- <allow-in-data-usage-save package="com.google.android.gms"/> -->`

`<!-- <allow-in-power-save  package="com.google.android.gms"/> -->`

Now it is possible to power save GMS.

---
Tested By: @attigliuzzo - Model-Number "SHT-W09 9.1.0.335(C432E3R1P2)" - Date tested: 03.11.2020
