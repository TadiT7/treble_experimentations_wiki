# [Nokia 2.2] - [wasp]
** Bootloader unlock for this phone: https://forum.xda-developers.com/t/guide-how-to-unlock-the-bootloader-for-nokia-2-2.4244039/

## Hardware Support (AOSP 9)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ×                                                         |

## Hardware Support (AOSP 10)
not done yet

## Hardware Support (AOSP 11)
not done yet

***
## Additional Notes

When flashing, please ensure the vbmeta from WSP stock firmware need to be flashed with both disabling parameters as well.

To fix the notch issue, choose Hide in developer options - Display cutout, then the rounded corners diameter in Phh Treble Settings - Misc features need to be configured to 11.

Example:
`fastboot --disable-verity --disable-verification flash vbmeta_a /path/to/vbmeta.img`

***

## Tested By:
AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 2.2 (TA-1179) 00WW_1_680 (WSP-1680-0-00WW-B01) @ 8/3/2021

Template created by @zguithues