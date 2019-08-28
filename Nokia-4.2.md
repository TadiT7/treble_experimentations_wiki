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
| Notch Display             | Unproperly                                                |

***
## Additional Notes

This particular one is a prototype unit with many parts missing including camera, so most of functions can't be tested.

No navigation bar during testing, hope this could be fixed soon.

When flashing, please ensure the vbmeta from PAN stock firmware need to be flashed with only "--disable-verity" parameter, otherwise the phone will get stuck at HS-USB Diagnostics 900E mode.

***


## Tested By:
AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 4.2 00WW_1_36C @ 28/08/2019

Template created by @zguithues