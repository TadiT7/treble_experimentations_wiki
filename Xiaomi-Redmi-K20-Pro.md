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
| Camera                    | √× (Cameras work, but front camera pops up on first boot and won't retract, requiring manual control via terminal command - see [#539](https://github.com/phhusson/treble_experimentations/issues/539) and below note 1); Stock carema apk only support main camera as 12MP |
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

## Additional note 1

Terminal command for manually controlling the front camera motor:

Popup: `xiaomi-motor popup 1`

Retract: `xiaomi-motor takeback 1`

## Additional note 2

Maybe it's just a problem caused by vendor, or lack some configure in gsi system.

If you have a high-sensitive armature earphone and suffer from terrible background noise, try to use CLS_H_ULP rather than LOHIFI as headphone default mode in `/vendor/etc/mixer_paths_tavil.xml` file.

The original string is "CLS_H_LOHIFI".

```
<!-- Headphone Default mode - uLP -->

<ctl value="CLS_H_ULP" name="RX HPH Mode"/>


<path name="hph-lowpower-mode">

<ctl value="CLS_H_ULP" name="RX HPH Mode"/>

</path>
```

---

Tested By: AndyYan (AndyCGYan), kumoilain @ Redmi K20 Pro V10.3.6.0.PFKCNXM @ 2019/06

Template created by @zguithues and @hackintosh5