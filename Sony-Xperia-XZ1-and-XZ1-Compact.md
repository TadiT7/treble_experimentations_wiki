# Sony Xperia XZ1 Compact, "lilac", G8441 (single-sim variant)

**Factory image:**  47.1.A.12.75

**phh-image:** `release/180417/system-arm64-aonly-gapps-su.img`\
this is an 8.1 image built on 2018-04-17 using the phh script `build.sh`\
android tag is `android-8.1.0_r19`

## Hardware Support

* Camera:
> Google camera does not work; it opens but does not seem to connect to the camera hardware (no preview images are generated).  The Open Camera app (by M Harman) is able to connect to the camera hardware and show previews, but all photos are solid green; this is the infamous Sony green-screen issue, which appears on unlocked Sony devices.  Video works correctly in the Open Camera app.

* Speaker / Microphone
> working (tested YouTube, built-in mp3 player, in-call audio).

* Bluetooth
> working (tested device pairing and file transfer).

* Wifi
> working

* SIM / Mobile Data / Voice
> Voice calls are working.  Mobile-data has not been tested.

* VoLTE
> not tested.

* Fingerprint Reader
> working.

***
## Additional Notes

logcat output shows a number of link failures due to two missing libraries:

```
$ grep -i cannot phh-logcat-1.txt | head -n 6
03-20 07:18:07.561 F/libc    ( 1036): CANNOT LINK EXECUTABLE "/vendor/bin/idd-logreader": library "android.hidl.base@1.0.so" not found
03-20 07:18:07.599 F/DEBUG   ( 1045): Abort message: 'CANNOT LINK EXECUTABLE "/vendor/bin/idd-logreader": library "android.hidl.base@1.0.so" not found'
03-20 07:18:08.192 F/libc    ( 1228): CANNOT LINK EXECUTABLE "/system/vendor/bin/ipacm": library "android.hardware.tetheroffload.control@1.0.so" not found
03-20 07:18:08.308 F/DEBUG   ( 1346): Abort message: 'CANNOT LINK EXECUTABLE "/system/vendor/bin/ipacm": library "android.hardware.tetheroffload.control@1.0.so" not found'
03-20 07:18:08.420 F/libc    ( 1304): CANNOT LINK EXECUTABLE "/system/vendor/bin/netmgrd": cannot locate symbol "_ZN7android4hidl4base4V1_08BnHwBaseD0Ev" referenced by "/system/lib64/android.system.net.netd@1.0.so"...
03-20 07:18:08.434 F/DEBUG   ( 1444): Abort message: 'CANNOT LINK EXECUTABLE "/system/vendor/bin/netmgrd": cannot locate symbol "_ZN7android4hidl4base4V1_08BnHwBaseD0Ev" referenced by "/system/lib64/android.system.net.netd@1.0.so"...'
```

***

## Tested By:

* https://github.com/jamuir, 2018-04-18
