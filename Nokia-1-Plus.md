# [Nokia 1 Plus] - [ant]

## Hardware Support (AOSP 9)

Unable to flash due to small system partition (1,488 MB).

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |

***
## Additional Notes

Only "arm32_binder64-ab-vanilla" flavor is known working.

You must wipe data / factory reset under stock recovery + stock ROM before flashing this treble GSI, don't use fastboot to erase userdata (either format userdata, -w or flash userdata are not acceptable). Otherwise you'll only get less than 1GB free storage space to use.

***


## Tested By:

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 1 Plus TA-1111 00WW_0_980 @ 08/11/2019


Template created by @zguithues