# Device

Xiaomi Redmi K50 Ultra / Xiaomi 12T Pro (diting)

## Steps to install

* I just tested it on DSU by [DSU-Sideloader](https://github.com/VegaBobo/DSU-Sideloader)

## Tested Image

[android_13.0.0_r24 ci-20230131](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230131) Based on V13.0.4.0.SLFCNXM  
[android_13.0.0_r35 ci-20230315](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230315) Based on V13.0.4.0.SLFCNXM  
[android_13.0.0_r35 ci-20230324](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230324) Based on V13.0.4.0.SLFCNXM  
[android_13.0.0_r35 ci-20230330](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230330) Based on V13.0.4.0.SLFCNXM  
[android_13.0.0_r41 ci-20230417](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230417) Based on V13.0.4.0.SLFCNXM  

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work, but only 1 back camera.                             |
| Speaker / Mic             | Work.                                                     |
| Bluetooth                 | Work.                                                     |
| WiFi                      | Work.                                                     |
| SIM / Mobile Data / Voice | Can't receive SMS. SIM2 can use VoLTE to receive SMS*.    |
| VoLTE                     | Work, but only SIM2*.                                     |
| 2G                        | Can Voice, send SMS, can't receive SMS.                   |
| 3G                        | No device to test                                         |
| 4G/5G                     | Work.                                                     |
| Fingerprint on display    | Not Work.                                                 |
| NFC                       | Work.                                                     |
| Offline Charging          | Not test on DSU.                                          |
| 120Hz screen              | Not work.                                                 |
| PhhSettings-Xiaomi-DT2W   | Work.                                                     |
| IR                        | Work.                                                     |
| Sensor                    | All work.                                                 |
---
\* Notice:  
Only SIM2 can use VoLTE and receive SMS use VoLTE. (Tested on China Mobile SIM)  
Phh Treble Settings->IMS features-> install IMS APK, and all options need to be pressed, and you can use IMS and VoLTE.  
The IMS & VoLTE work on [android_13.0.0_r24 ci-20230131](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230131),[android_13.0.0_r35 ci-20230315](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230315).   
The IMS & VoLTE don't work on [android_13.0.0_r35 ci-20230324](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230324), [android_13.0.0_r35 ci-20230330](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230330) [android_13.0.0_r41 ci-20230417](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230417).  
For this device, it look like some issues on [android_13.0.0_r35 ci-20230324](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230324) and newer, may be "Add support for in-call audio on AIDL (Android 12 vendor) qcom devices" this change is bad for this device.  

\** Tips:  
Phh Treble Settings->Qualcomm features-> Dsable soundvolume effect. may fix audio distorsion.  

Tested By:   
kindle4jerry - K50Ultra(CN), [android_13.0.0_r24 ci-20230131](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230131) Based on V13.0.4.0.SLFCNXM - 2023/04/09  
kindle4jerry - K50Ultra(CN), [android_13.0.0_r35 ci-20230315](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230315) Based on V13.0.4.0.SLFCNXM - 2023/04/09  
kindle4jerry - K50Ultra(CN), [android_13.0.0_r35 ci-20230324](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230324) Based on V13.0.4.0.SLFCNXM - 2023/04/09  
kindle4jerry - K50Ultra(CN), [android_13.0.0_r35 ci-20230330](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230330) Based on V13.0.4.0.SLFCNXM - 2023/04/09  
kindle4jerry - K50Ultra(CN), [android_13.0.0_r41 ci-20230417](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230417) Based on V13.0.4.0.SLFCNXM - 2023/04/09  

Template created by @zguithues and @hackintosh5