# Device

Tested with `crDroid-8.6-arm64_bgN-Unofficial.img.xz` gsi and `SiLonT-4.19-whyred-NEWCAM-deirma.zip`/`Panda-v12.3-eas.zip` kernels.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                     |
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Can't test                                                |
| Fingerprint               | Works                                                     |
| NFC                       | N/A                                                       |
| Offline Charging          | Works                                            |
| Other feature             | Gcam freezes/crashes when switching to front camera with 4.19 kernels (silont for example), charging indication in notification led is not working, exfat is not working on sdcard with some kernels (silont for example) https://github.com/phhusson/treble_experimentations/issues/1197 https://github.com/phhusson/treble_experimentations/issues/761, can be fixed by this module https://github.com/phhusson/treble_experimentations/files/8948418/ntfs-exfat-support.zip                                                    |
---