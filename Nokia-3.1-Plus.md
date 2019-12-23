# [Nokia 3.1 Plus] - [roo]
**MUST FLASH CHINA FIRMWARE FIRST AS GLOBAL FIRMWARE DOESN'T ALLOW FLASHING VBMETA HENCE IT WILL NOT BOOT**
## Hardware Support (AOSP 8.1)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ✓                                                         |
| Speaker / Mic             | ✓                                                         |
| Bluetooth                 | ✓                                                         |
| WiFi                      | ✓                                                         |
| SIM / Mobile Data / Voice | ✓                                                         |
| VoLTE                     | ✓                                                         |
| Fingerprint               | ✓                                                         |
| NFC                       | ✓                                                         |

Vendor error will appear every time when booting.

## Hardware Support (AOSP 9)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ✓                                                         |
| Speaker / Mic             | ✓                                                         |
| Bluetooth                 | ✓                                                         |
| WiFi                      | ✓                                                         |
| SIM / Mobile Data / Voice | ✓                                                         |
| VoLTE                     | ✓                                                         |
| Fingerprint               | ✓                                                         |
| NFC                       | ✓                                                         |

***
## Additional Notes

Nokia 3.1 Plus sold in China (TA-1117) doesn't have NFC hardware.

When flashing, please ensure the vbmeta from ROO stock firmware need to be flashed with both disabling parameters as well.

Example:
`fastboot --disable-verity --disable-verification flash vbmeta_a /path/to/ROO-0-130C-00CN-vbmeta.img`

If you wipe/format userdata partition under fastboot mode, it can't recognize the whole storage space properly. You have to wipe data under stock recovery.
Effect:
[Photo 1, before resize correction](https://t.me/phhtreble/214538)
[Photo 2, after resize correction](https://t.me/phhtreble/214542)

***


## Tested By:
AOSP 8.1: * Calyx Hikari (HikariCalyx) @ Nokia 3.1 Plus 00CN_1_30C @ 26/06/2019

AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 3.1 Plus 00WW_2_230 @ 26/06/2019

AOSP 9: * Zapacitu18  @ Nokia 3.1 Plus 00CN_1_30C @ 12/23/2019

Template created by @zguithues