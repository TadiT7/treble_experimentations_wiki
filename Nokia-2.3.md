# [Nokia 2.3] - [ironman / IRM]

Bootloader Unlock : 

Please use [MTKClient](https://github.com/bkerler/mtkclient) to perform bootloader unlock.

To remove your device is corrupt warning, simply flash vbmeta image and disable verity/verification.

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

```
fastboot flash system /path/to/gsi/image.img
fastboot --disable-verity --disable-verification flash vbmeta /path/to/vbmeta.img
```

After flashing it along with vbmeta, you must format userdata partition as f2fs filesystem, or the phone will bootloop:

```fastboot format:f2fs userdata```

## Tested By:

@HikariCalyx @ Nokia 2.3 TA-1206 00WW_3_310_SP09 (IRM-331J-0-00WW-B01) @ 02/04/2023

@pcurz @ Nokia 2.3 TA-1214 00WW_3_310 @ 15/04/2023
Latest build goes into bootloop (I formatted userdata to f2fs, fastboot always says something about that Partition is ext4 but continue with the process anyway, If there is something I forgot, ping me thanks)

Template created by @zguithues