# [Redmi K30 Pro] - [lmi]

## Hardware support (Referred from Redmi K20 Pro)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √× (Cameras work, but front camera pops up on first boot and won't retract, requiring manual control via terminal command - see [#539](https://github.com/phhusson/treble_experimentations/issues/539) and below note 1); Stock camera apk only support main camera as 12MP |
| Audio                     | √× (No Type-C audio - see [#542](https://github.com/phhusson/treble_experimentations/issues/542); Background noise with armature earphone at low sound level - see below note 2) |
| Bluetooth                 | √× (In-call audio doesn't work) |
| Display                   | √× (Auto-brightness doesn't work yet - waiting on [the overlay](https://github.com/phhusson/vendor_hardware_overlay/pull/110) to be merged; Corners look slightly pixelated due to lack of corresponding overlay item) |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √ |
| VoLTE                     | ? (Untested) |
| Fingerprint               | √× (Recognition a little slower maybe due to system setting; Unlocking from off/AOD state not supported, need press power button first) |
| NFC                       | √? (Support card info reading via NXP.TagInfo, need more tests like card writing / simulation) |
| Offline Charging          | × |

## Additional Note

Terminal command for manually controlling the front camera motor (may require `su` depending on the GSI):

Popup: `xiaomi-motor popup 1`

Retract: `xiaomi-motor takeback 1`

---

This wiki page is referred from Xiaomi Redmi K20 Pro (raphael) page as this device have almost everything in common with it.
Redmi K30 Pro Tested By: Akito Mizukito (RealAkito) @ Redmi K30 Pro V11.0.6.0.QJKEUXM / V11.0.16.0.QJKCNXM / 20.5.14 Beta 
Redmi K20 Pro Tested By: AndyYan (AndyCGYan), kumoilain @ Redmi K20 Pro V10.3.6.0.PFKCNXM @ 2019/06

Template created by @zguithues and @hackintosh5