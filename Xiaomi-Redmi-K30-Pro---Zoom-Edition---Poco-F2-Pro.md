# [Redmi K30 Pro] - [lmi]

## Hardware support (Referred from Redmi K20 Pro)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √× (Cameras work, but front camera does not popup at all, please read note 1); Stock camera apk only support main camera |
| Audio                     | √? Speaker and Headphone Jack is working, USB Type C DAC is untested. |
| Bluetooth                 | √? Bluetooth Speaker works fine, In-call is untested. |
| Display                   | √ |
| WiFi / Hotspot            | √ |
| GPS                       | √ |
| SIM / Mobile Data / Voice | √? Internet Data works, call is untested. |
| VoLTE                     | ? (Untested) |
| LED                       | √× There're 2 LEDs in the system, only one is working. |
| Fingerprint               | √× (Recognition a little slower maybe due to system setting; Unlocking from off/AOD state not supported, need press power button first) |
| NFC                       | √? (Support card info reading via NXP.TagInfo, need more tests like card writing / simulation) |
| Offline Charging          | × |

## Additional Note

Terminal command for manually controlling the front camera motor (may require `su` depending on the GSI):

Popup: `xiaomi-motor popup 1`

Retract: `xiaomi-motor takeback 1`

---

This wiki page is referred from Xiaomi Redmi K20 Pro (raphael) page as this device have a lot of things in common with in.

Redmi K30 Pro Tested By: Akito Mizukito (RealAkito) @ Redmi K30 Pro V11.0.6.0.QJKEUXM / V11.0.16.0.QJKCNXM / 20.5.14 Beta 

Origin Redmi K20 Pro Wiki is made by AndyYan (AndyCGYan)

Template created by @zguithues and @hackintosh5