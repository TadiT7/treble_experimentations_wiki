**Oukitel K8 device details:**
* SoC: MT6750T
* Base Android OS: Android 8.0 Oreo 
* VNDK = 26

**Tested:**
* Pie GSI 
* Oreo GSI

**Bugs:**
* Hotspot (only in Pie) 
* Brightness may be stuck in highest level in Oreo

All other features are confirmed working: 
* WiFi
* Bluetooth 
* Fingerprint
* Dual SIMs
* Sound
* Camera/Video
* Data
* Notification LED
* Call
* SMS

[PIE] USSD may not work as expected such as when checking balance (only in v111 and below) . This can simply be fixed editing the build.prop and adding the line
`persist.sys.radio.ussd.fix=true`

**NOTE:** USSD issues have been fixed in Pie v112+ and Oreo v30+
