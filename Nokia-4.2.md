# [Nokia 4.2] - [panther]

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

***
## Additional Notes

This particular one is a prototype unit with many parts missing including camera, so most of functions can't be tested.

No navigation bar during boot, you must use following command under root permission to add it:

`setprop persist.sys.phh.mainkeys 0`

When flashing, please ensure the vbmeta from PAN stock firmware need to be flashed with only "`--disable-verity`" parameter, otherwise the phone will get stuck at HS-USB Diagnostics 900E mode.

e.g.
`fastboot --disable-verity flash vbmeta_a /path/to/vbmeta.img`

To fix the notch issue, choose Hide in developer options - Display cutout, then the rounded corners diameter in Phh Treble Settings - Misc features need to be configured to 10.

***


## Tested By:
AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_1_36C @ 28/08/2019

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_1_36C @ 09/11/2019 

Template created by @zguithues