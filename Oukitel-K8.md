**Oukitel K8 device details:**
* SoC: MT6750T
* Base Android OS: Android 8.0 Oreo 

**Tested:**
* Pie GSI 

**Bugs:**
* Hotspot (seems to be common with most GSIs tested) 

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

USSD may not work as expected such as when checking balance. This can simply be fixed editing the build.prop and adding 
**persist.sys.radio.ussd.fix=true**

If SMS sending isn't working, do the following (but applies to the data SIM):
 
1. Download "ForceLTE" from Play Store, 
* Click to change 4G/3G/E
* Scroll down to SMSC and enter your network's Message Centre number. 

2. Or dial `*#*#4636#*#*` and follow same step as in No. 1.