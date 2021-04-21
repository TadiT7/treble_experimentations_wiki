# [Rakuten Mini C330] - [C330]

## How to unlock bootloader
1. Tap "Software version" in Settings menu a few times
2. Enter *636865625# on the dial pad
3. Open Developer options and enable OEM unlocking
4. Reboot to bootloader and run `fastboot flashing unlock` and `fastboot flashing unlock_critical`

Source (Japanese, by @AndroPlus-org ): https://androplus.org/Entry/14664/

## Hardware Support (AOSP 9)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC                       | √                                                         |
| FeliCa                    | x                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |

## Hardware Support (AOSP 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC                       | √                                                         |
| FeliCa                    | x                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |

## Hardware Support (AOSP 11)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC (Felica)              | ?                                                         |
| FeliCa                    | x                                                         |
| SIM / Mobile Data / Voice | ?                                                         |
| VoLTE                     | ?                                                         |

## Additional Notes

* vbmeta need to be flashed with this command:

```fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img```

* To boot Android 10 GSI or newer, you'll have to replace these files in vendor partition with files extracted from Xiaomi Redmi 8, or the phone will boot loop:
```
/vendor/bin/hw/android.hardware.graphics.composer@2.1-service
/vendor/lib64/libsdmcore.so
/vendor/lib64/hw/android.hardware.graphics.composer@2.1-impl.so
/vendor/lib64/hw/hwcomposer.msm8937.so
```

* This device is eSIM only. If you want to use mobile data, you have to extract and place these files to register a new eSIM profile:
```
/system/app/EuiccOverlay/EuiccOverlay.apk
/system/priv-app/EuiccGoogle/EuiccGoogle.apk
```
## Tested By:

AOSP 9: * AndroPlus_org @ Rakuten Mini C330 C330AE_9.0_RMN_JP_72_SS @ 17/06/2020  
AOSP 10: * AndroPlus_org @ Rakuten Mini C330 C330AE_9.0_RMN_JP_72_SS @ 17/06/2020  
AOSP 11: * Calyx Hikari (HikariCalyx) @ Rakuten Mini C330 C330AE_9.0_RMN_JP_90_SS @ 21/04/2021

Template created by @zguithues