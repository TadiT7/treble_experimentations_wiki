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

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | need magisk modules for it to work                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ×                                                         |

## Hardware Support (AOSP 12)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                                                          |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | untested                                                  |

***
## Additional Notes

When flashing, please ensure the vbmeta from WSP stock firmware need to be flashed with both disabling parameters as well.

To fix the notch issue, choose Hide in developer options - Display cutout, then the rounded corners diameter in Phh Treble Settings - Misc features need to be configured to 11.

Before installing AOSP 11 update to stock android 11 after your bootloader unlock and then wipe system and finally flash the gsi and vbmeta to fix the notch choose hide in dev options then the rounded corner diameter in phh treble settings or just do the rounded corner diameter itself

Example:
`fastboot --disable-verity --disable-verification flash vbmeta_a /path/to/vbmeta.img`

***

## Tested By:

AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 2.2 (TA-1179) 00WW_1_680 (WSP-1680-0-00WW-B01) @ 8/3/2021

AOSP 11: * Areallydumbperson on xda @ Nokia 2.2 (TA-1188) 00WW_3_270) (WSP-3270-0-00WW-B01) @ 6/10/2021

AOSP 12: * VR25 @ xda-developers, find updated installation instructions [here](https://forum.xda-developers.com/t/guide-how-to-unlock-the-bootloader-for-nokia-2-2.4244039/post-86251579).

Template created by @zguithues