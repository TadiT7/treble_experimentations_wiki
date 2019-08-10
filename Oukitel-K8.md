**Oukitel K8 device details:**
* SoC: MT6750T
* Base Android OS (Vendor): Android 8.0 Oreo 

**Tested:**
* Pie GSI 
* Oreo GSI

**Bugs:**
* Hotspot (only in Pie) 
* None in Oreo

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

SMS works, but if you've messed with your setup or for any reason SMS isn't delivering, do the following (but only applies to the SIM set as data SIM):
 
1. Download "ForceLTE" from Play Store, 
* Click to change 4G/3G/2G
* Scroll down to SMSC and enter your network's Message Centre number. 

2. Or dial `*#*#4636#*#*` and follow same step as in No. 1.
