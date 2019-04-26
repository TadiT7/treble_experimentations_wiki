# **Asus Zenfone Live (L1) ZA550KL**
##  **Hardware support**
* **Camera**
> Front and back both working. Stock gsi ROM camera is working fine with few bugs, flash on stock camera if set to on or auto will make camera force close, also the camera are pitch black on some gsi ROM, if we using the front camera, we will see our face rendered very weird (AICP-mordiford by AndroPlus is one of many example of gsi ROM with pre-installed normal camera). Install 3rd party camera apps will solve the problem. Or you can enable the Camera2 API for minimizing the bugs. Add this line `persist.vendor.camera.HAL3.enabled=1` to _/system/buid.prop_
* **Speaker / Microphone**
> Loud-speak (bottom) works, earpiece (top-front) works, microphone works
* **Bluetooth**
> Bluetooth with Mi Band 2 worked
* **WiFi**
> Works
* **SIM / Mobile Data / Voice**
> Works
* **Hotspot**
> Works. Some of gsi ROM can't enable hotspot like Pixel Experience by EnesSastim.
## **Additional Notes**
_This model pre-installed by Asus with Android 8.0 (ZenUI customized) and support project Treble._
## **Tested By** :
* **AcAciA** - Asus Zenfone Live (L1) ZA550KL 2GB RAM on AOSP 8.1 v23 by phhusson, and Pixel Experience 2018-09-11 by jhenrique09. On 2018-9-13.
* **Maulana Kurniawan & Satu Prasetyo Gilang Mahameru** - Asus Zenfone Live L1 ZA550KL 2GB RAM on AOSP 8.1 v30 & AOSP 9.1 v112 by phhusson, AOSP Extended v6.0, v6.1 & v6.3 by EnesSastim, AICP-mordiford v13.1 by AndroPlus, LineageOS v15.1 gsi by phhusson, dotOS v2.3.1 by dotOS Team, POSP by NFound etc. On 2019-04-15