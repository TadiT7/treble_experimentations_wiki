# [Nokia 5.1] - [co2]

## Hardware Support (AOSP 9)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √ |
| NFC                       | ?                                                         |

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √|
| NFC                       | ?                                                         |

***
## Additional Notes

The GSI need to be flashed with command, and you must define a slot:

> fastboot -w flash system_a /path/to/system-quack-arm64-ab-gapps.img.xz

***


## Tested By:

AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 5.1 00WW_3_25B_SP01 (CO2-315C-0-00WW-B01) @ 25/10/2019

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 5.1 00WW_3_25B_SP01 (CO2-315C-0-00WW-B01) @ 25/10/2019


Template created by @zguithues

