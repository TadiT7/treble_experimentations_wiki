# [Nokia 7.2] - [daredevil / ddv]

## Hardware Support (AOSP 9)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ×                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ?                                                         |

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ?                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| NFC                       | ?                                                         |

***
## Additional Notes

The particular device is a TA-1196 without NFC hardware, so NFC functionality cannot be tested.

On AOSP 9, Camera crashes every time, and third party camera app won't help at all.


When flashing, please ensure the vbmeta from Nokia 7.2 stock firmware need to be flashed with both disabling parameters as well.

``
fastboot --disable-verity --disable-verification flash vbmeta /path/to/vbmeta.img
``

***


## Tested By:


AOSP 9: * Calyx Hikari (HikariCalyx) @ Nokia 7.2 (TA-1196) 00WW_1_270 (DDV-1270-0-00WW-B01) @ 01/04/2020

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 7.2 (TA-1196) 00WW_2_250 (DDV-2250-0-00WW-B01) @ 01/04/2020


Template created by @zguithues