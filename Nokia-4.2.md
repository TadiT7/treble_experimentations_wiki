# [Nokia 4.2] - [panther]

Bootloader Unlock :
Please refer https://github.com/phhusson/treble_experimentations/wiki/Nokia-1.3

## Hardware Support (AOSP 9)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ?                                                         |
| Speaker / Mic             | ?                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ?                                                         |
| Notch Display             | Unproperly in default configuration                       |

## Hardware Support (AOSP 10)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ?                                                         |
| Speaker / Mic             | ?                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ?                                                         |
| Notch Display             | Unproperly in default configuration                       |

## Hardware Support (Android 13)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| NFC                       | √                                                         |
| Notch Display             | √                                                         |

***
## Additional Notes

### AOSP 9 and AOSP 10
This particular one is a prototype unit with many parts missing including camera, so most of functions can't be tested.

No navigation bar during boot, you must use following command under root permission to add it:

`setprop persist.sys.phh.mainkeys 0`

When flashing, please ensure the vbmeta from PAN stock firmware need to be flashed with only "`--disable-verity`" parameter, otherwise the phone will get stuck at HS-USB Diagnostics 900E mode.

e.g.
`fastboot --disable-verity flash vbmeta_a /path/to/vbmeta.img`

To fix the notch issue, choose Hide in developer options - Display cutout, then the rounded corners diameter in Phh Treble Settings - Misc features need to be configured to 10.

***

### AOSP 13

Tested GSI: https://forum.xda-developers.com/t/gsi-13-lineageos-20-trebledroid-based.4517345/ , arm64 bgN variant.

Due to updated bootloader, vbmeta can be flashed with both `--disable-verity` and `--disable-verification` parameters and it won't get stuck at HS-USB Diagnostics 900E mode.

e.g.
`fastboot --disable-verity --disable-verification flash vbmeta /path/to/vbmeta.img`

## Tested By:
AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_1_36C @ 28/08/2019

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_1_36C @ 09/11/2019 

Android 13: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_3_240 @ 02/04/2023

Template created by @zguithues