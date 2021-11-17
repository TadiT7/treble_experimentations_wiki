# [Nokia 3.4 and 5.4] - [doctorstrange and doctordoom]

Nokia 3.4 and 5.4 shares the same motherboard design and Snapdragon 460 and 662 are basically same thing, therefore the report applies on both Nokia 3.4 and 5.4.

## Hardware Support (AOSP 11)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ×                                                         |
| Fingerprint               | √ |
| NFC                       | ×                                                         |

## Hardware Support (AOSP 12)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ×                                                         |
| Fingerprint               | √ |
| NFC                       | ×                                                         |

***
## Additional Notes

You must flash GSI under Fastbootd and the vbmeta need to be processed as well.

```fastboot delete-logical-partition product_a
fastboot delete-logical-partition product_b
fastboot flash system /path/to/system-[codename]-arm64-ab-[flavor].img
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
fastboot reboot-bootloader
fastboot -w reboot
```
***


## Tested By:

AOSP 11: * Calyx Hikari (HikariCalyx) @ Nokia 5.4 00WW_1_300 @ 17/11/2021

AOSP 12: * Calyx Hikari (HikariCalyx) @ Nokia 5.4 00WW_1_300 @ 17/11/2021


Template created by @zguithues

