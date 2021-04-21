# [Rakuten Mini C330] - [9]

Bootloader Unlock for this device (Japanese, by @AndroPlus_org ): https://androplus.org/Entry/14664/

## Hardware Support (AOSP 9)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC (Felica)              | ?                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC (Felica)              | ?                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |

## Hardware Support (AOSP 11)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC (Felica)              | ?                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |

## Additional Notes

* vbmeta need to be flashed with this command:

```fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img```

* To boot Android 10 GSI or newer, you'll have to replace these files in vendor partition, or the phone will boot loop:
```/vendor/bin/hw/android.hardware.graphics.composer@2.1-service
/vendor/lib64/libsdmcore.so
/vendor/lib64/hw/android.hardware.graphics.composer@2.1-impl.so
/vendor/lib64/hw/hwcomposer.msm8937.so
```
## Tested By:

AOSP 11: * Calyx Hikari (HikariCalyx) @ Rakuten Mini C330 C330AE_9.0_RMN_JP_90_SS @ 21/4/2021

Template created by @zguithues