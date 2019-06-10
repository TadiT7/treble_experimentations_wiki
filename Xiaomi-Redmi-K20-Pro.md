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
| Camera                    | √× (Cameras work, but front camera pops up on first boot and won't retract, and you need manually control the motor by terminal command - see [#539](https://github.com/phhusson/treble_experimentations/issues/539))|
| Audio                     | √× (Audio playback stutters - see [#541](https://github.com/phhusson/treble_experimentations/issues/541); no Type-C audio - see [#542](https://github.com/phhusson/treble_experimentations/issues/541))         |
| Bluetooth                 | √× (In-call audio doesn't work)                           |
| Display                   | √× (Auto-brightness doesn't work, manual does, corner display looks a little strange with unexpected color pixel)            |
| WiFi / Hotspot            | √                                                         |
| GPS                       | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | ? (Untested)                                              |
| Fingerprint               | ? (Enrollment works, recognition a little slowwer maybe duet to system setting. Not support wake up device when screen is AOD/off)                |
| NFC                       | √? (Support card info reading via NXP.TagInfo, need more test like card simulate)                                              |
| Offline Charging          | × (only stop at Redmi LOGO, and system not boot)          |
---

Tested By: AndyYan (AndyCGYan) @ Redmi K20 Pro V10.3.6.0.PFKCNXM @ 2019/06/03

Template created by @zguithues and @hackintosh5