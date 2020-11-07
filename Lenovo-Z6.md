Hardware Support

LED:

Not tested

FM:

Not tested

Camera:

Work: front works fine; the vision of the back one seems to be narrow

To fix bright spot in back camera, appending following lines in /system/build.prop

```
#Expose aux camera for below packages
vendor.camera.aux.packagelist=org.codeaurora.snapcam,com.qualcomm.saltproject2,com.zui.camera,com.android.camera,com.zui.camera
#LENOVO_CUSTOM start
sys.camera.packagename.zui=1
```

Speaker / Microphone:

Work

Bluetooth:

Calling with Bluetooth earphone is Ok;
Media sound through Bluetooth earphone do not work.

Wifi:

Work (Both 5.0Ghz and 2.4GHz)

SIM / Mobile Data / Voice:

Work,tested:

China Mobile/Telecom/Unicom LTE

China Mobile/Telecom/Unicom

VoLTE:

Not working;
To receive SMS on LTE, you must send message to CM/CT/CU to cancel VoLTE service:
For example, sending QXVOLTE to 10086 if you are using Beijing CM.

Fingerprint Reader:

Work;
But must specific the location of the fingerprint with hard-coding...
It seems not to read the location from prop.

Headphone:

3.5 mm headphone Work

adb:

Work

Additional Notes:

**DO NOT wipe system** at any time!!!!! Or you cannot enter system and recovery any more and have to flash the stock image with Qualcom 9008.
You might have to format /data/ after flashing system.img if boot loops or booting to recovery.

The firmware/vendor version I am using is 262.