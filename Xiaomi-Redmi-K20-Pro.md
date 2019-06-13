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
| Camera                    | √× (Cameras work, but front camera pops up on first boot and won't retract, requiring manual control via terminal command - see [#539](https://github.com/phhusson/treble_experimentations/issues/539) and below note) |
| Audio                     | √× (No Type-C audio - see [#542](https://github.com/phhusson/treble_experimentations/issues/542)) |
| Bluetooth                 | √× (In-call audio doesn't work) |
| Display                   | √× (Auto-brightness doesn't work, manual does; corners look slightly pixelated due to lack of corresponding overlay) |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √ |
| VoLTE                     | ? (Untested) |
| Fingerprint               | √ (Recognition a little slower maybe due to system setting; unlocking from off/AOD state not supported) |
| NFC                       | √? (Support card info reading via NXP.TagInfo, need more tests like card writing / simulation) |
| Offline Charging          | × |

## Additional note

Terminal command for manually controlling the front camera motor (root required):

Popup: `xiaomi-motor popup 1`

Retract: `xiaomi-motor takeback 1`

---

Tested By: AndyYan (AndyCGYan), kumoilain @ Redmi K20 Pro V10.3.6.0.PFKCNXM @ 2019/06

Template created by @zguithues and @hackintosh5