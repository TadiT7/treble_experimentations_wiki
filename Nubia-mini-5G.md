# [Nubia mini 5G] - [TP1803]

## Hardware Support (Android 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |
| 5G                        | ×                                                         |



***
## Additional Notes

* Flash an alternative vbmeta (e.g. [Google's](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img))
* Format /data and flash GSI from TWRP
* Change `persist.radio.multisim.config` from `dsds` to `ssss` in `/vendor/build.prop`
* Remove `IBootControl` subsection from `/vendor/etc/vintf/manifest.xml` (seems to remedy random bootloop)
* If stuck in bootanimation on first boot, force reboot via key combo

***


## Tested By:

LineageOS 17.1: AndyYan (AndyCGYan) @ Nubia mini 5G TP1803_Z77_CN_WPL0P_V116 @ 2020/06/17


Template created by @zguithues