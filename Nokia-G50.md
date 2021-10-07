# [Nokia G50] - [punisher / PHR]

Bootloader Unlock : TBD (following test is performed on prototype unit with retail OS)

## Hardware Support (Android 11)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC                       | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ×                                                         |
| Fingerprint               | √                                                         |
| 5G                        | √                                                         |


## Additional Notes

You'll need to delete product partition under fastbootd before flashing GSI:
```
fastboot delete-logical-partition product
```

## Tested By:

@HikariCalyx @ Nokia G50 00WW_1_100 @ 07/10/2021


Template created by @zguithues