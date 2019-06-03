# [Redmi K20 Pro] - [raphael]

## Steps to install

Similar to Mi 9, download [vbmeta.img](https://github.com/TadiT7/xiaomi_raphael_dump/blob/raphael-user-9-PKQ1.181121.001-V10.3.6.0.PFKCNXM-release-keys/vbmeta.img), then flash with
```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
```
Proceed with regular system image flashing steps.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √× (Cameras work, but front camera pops up on first boot and won't retract - see [#539](https://github.com/phhusson/treble_experimentations/issues/539))|
| Audio                     | √× (No Type-C audio; Mic-recorded audio stutters)         |
| Bluetooth                 | √× (In-call audio doesn't work)                           |
| Display                   | √× (Auto-brightness doesn't work, manual does)            |
| WiFi / Hotspot            | √                                                         |
| GPS                       | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ? (Untested)                                              |
| Fingerprint               | ? (Enrollment works, recognition untested)                |
| NFC                       | ? (Untested)                                              |
| Offline Charging          | ×                                                         |
---

Tested By: AndyYan (AndyCGYan) @ Redmi K20 Pro V10.3.6.0.PFKCNXM @ 2019/06/03

Template created by @zguithues and @hackintosh5