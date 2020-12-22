# Blackview BV9900

Overall it is usable.
Have some issues with the display that is flickering, even with option 

## Steps to install


* fastboot -u flash system lineage-17.1-20201215-UNOFFICIAL-treble_arm64_bvS.img

then following with the stock rom images found on the support page from [support page from blackview](https://bbs.blackview.hk/) 

* fastboot -u flash --disable-verity --disable-verification vbmeta BV9900_EEA_S900AA_V1.0_20191225V08_user_20200103_2/vbmeta.img

* fastboot -u flash userdata BV9900_EEA_S900AA_V1.0_20191225V08_user_20200103_2/userdata.img



## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ok                                                        |
| Speaker / Mic             | ok                                                        |
| Bluetooth                 | ok                                                        |
| WiFi                      | ok                                                        |
| SIM / Mobile Data / Voice | ok                                                        |
| VoLTE                     | Doesn't seems to work                                     |
| Fingerprint               | ok                                                        |
| NFC                       | not tested yet                                            |
| Offline Charging          | screen remains on                                         |
| Display / Backlight       | flickering issues                                         |
---

Tested By: openstove - BV9900(EEA), lineage-17.1-20201215-UNOFFICIAL-treble_arm64_bvS.img - 22.12.2020