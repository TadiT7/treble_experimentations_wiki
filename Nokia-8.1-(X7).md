# [Nokia 8.1 (X7)] - [pnx]

## Hardware Support (AOSP 8.1)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ? (Unable to test due to lack of hardware.)               |
| Notch Display             | Unproperly                                                |

> Battery and overall performance isn't ideal

## Hardware Support (AOSP 9)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ? (Unable to test due to lack of hardware.)               |
| Notch Display             | Unproperly [Actual Photo](https://t.me/phhtreble/194608)  |

## Hardware Support (AOSP 10)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √ (No alarms/ringtones sound, sound cracking in games ([Actual Record](https://t.me/nokia_pnx_gsi/17)); Mic can become broken during cellular voice calls)                                                       |
| Bluetooth                 | √ (AAC/aptX/aptX HD/LDAC audio has issues)                |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ? (Tried to force, but my carrier doesn't allow VoLTE on devices out of its supported list)                                                         |
| Fingerprint               | √                                                         |
| NFC                       | √                                                         |
| Notch Display             | Unproperly (Is going to be fixed with [this pull request](https://github.com/phhusson/vendor_hardware_overlay/pull/204))                         |

***
## Additional Notes

Nokia X7 sold in China (TA-1131) doesn't have NFC hardware.

Nokia X7 / 8.1 are too difficult to flash custom ROM.
When flashing, please ensure the vbmeta from PNX stock firmware need to be flashed with both disabling parameters as well.

***


## Tested By:
AOSP 8.1: * Calyx Hikari (HikariCalyx) @ Nokia X7 00CN_1_24F @ 12/04/2019

AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia X7 00WW_2_47A @ 12/04/2019

AOSP 10: * TechnoStone @ Nokia 8.1 00WW_4_30B @ 10/04/2020

Template created by @zguithues