# Hardware Support
* Camera: Stock camera works.
* Speaker: Works.
* Microphone: Works.
* Bluetooth: Deleting /vendor/etc/a2dp_audio_policy_configuration.xml fixes bluetooth inCall Audio, Bluetooth audio is still broken with pie vendor.
* WiFi: Works.
* Telephony: VoLTE Fix Install the ims.apk(adb push it to /system/app) attached and add this lines to /system/build.prop and reboot
persist.dbg.volte_avail_ovr=1
persist.dbg.vt_avail_ovr=1
* Fingerprint sensor: Works.

## Additional Notes:
(to be updated)

## Tested By:
* Rafyvitto (RR 7.0[03/30/2019])
* Preet M Paatel (Phh Treble[09/11/2018], Descendant[18/11/2018], PixelDust Pie[14/11/2018]{Doesn't boot})
* Kailash Sudhakar (Phh Treble[09/11/2018])
* Prashant (Phh Treble[09/11/2018], PixelDust Pie[14/11/2018]{Doesn't boot})
* Yash (Phh Treble[09/11/2018]
* Shubham (Phh Treble[09/11/2018]