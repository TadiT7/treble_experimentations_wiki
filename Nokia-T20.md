# [Nokia T20] - [riddler / RDD]

Bootloader Unlock : TBD (following test is performed on prototype unit with retail OS)

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

You'll need to delete product partition under fastbootd before flashing GSI:
```
fastboot delete-logical-partition product
```

## Tested By:

@HikariCalyx @ Nokia T20 00WW_2_340 @ 15/05/2023


Template created by @zguithues