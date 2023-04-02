# [Nokia 2.3] - [ironman / IRM]

Bootloader Unlock : 

Please use [MTKClient](https://github.com/bkerler/mtkclient) to perform bootloader unlock.

## Hardware Support (Android 13)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ?                                                         |
| Speaker / Mic             | ?                                                         |
| Bluetooth                 | ?                                                         |
| WiFi                      | ?                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |


## Additional Notes

Tested GSI: https://forum.xda-developers.com/t/gsi-13-lineageos-20-trebledroid-based.4517345/ , arm-binder64 (a64) bgN variant.

After flashing it along with vbmeta, you must format userdata partition as f2fs filesystem, or the phone will bootloop:

```fastboot format:f2fs userdata```

## Tested By:

@HikariCalyx @ Nokia 2.3 TA-1206 00WW_3_310_SP09 (IRM-331J-0-00WW-B01) @ 02/04/2023


Template created by @zguithues