# [Nokia 3.1 and 5.1] - [es2 and co2]

Nokia 3.1 and 5.1 shares the same source code and can be cross flashed between each other, therefore the report shown here can be applied on both Nokia 3.1 and Nokia 5.1.

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

> fastboot -w flash system_a /path/to/system-quack-arm64-ab-gapps.img

NFC can't be tested due to lack of hardware.

***


## Tested By:

AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 5.1 00WW_3_25B_SP01 (CO2-325C-0-00WW-B01) @ 25/10/2019

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 5.1 00WW_3_25B_SP01 (CO2-325C-0-00WW-B01) @ 25/10/2019


Template created by @zguithues

