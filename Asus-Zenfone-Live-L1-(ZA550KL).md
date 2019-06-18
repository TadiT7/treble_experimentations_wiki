 # Asus Zenfone Live L1 (ZA550KL)

Front and back camera both working but with few bugs. Flash on stock camera if set to on or auto the camera will launch to force close. Also the camera have a dark problem on some GSI. If we using the front camera, we will see our face rendered very weird. Activating Camera2 API & installing 3rd party camera apps will solve the weird face & dark camera problem like Open Camera or GCam Mod. Also video calling cannot use front camera.

## Steps to install

* Extract the image file (if it compressed, like .zip or .xz format).
* Boot into TWRP.
* Flash the image file into the System Image partition.

**DON'T EVER WIPE VENDOR PARTITION! IT'S A GSI, NOT AN OFFICIAL CUSTOM ROM!**

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (with bugs)                                                    |
| Speaker / Mic             | Working                                                    |
| Bluetooth                 | Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| VoLTE                     | Working (with a patch)                                                    |
| Hotspot                   | Working                                                    |
| Flashlight                | Working                                                    |
| Offline Charging          | Working                                                    |
| Other feature             | Not tested at all                                                    |
---

Tested By: AcAciA, [Maulana Kurniawan](https://t.me/maulaaana), [Satu Prasetyo Gilang Mahameru](https://t.me/m4h4m3ru) - ASUS_X00RD, WW-15.01.xxxx.xxx - September 14, 2018 - Template created by [@maulaaana](https://github.com/maulaaana), @zguithues and @hackintosh5

Join our [Asus Zenfone Live L1 Official Telegram Group](https://t.me/ZenfoneLiveL1) or our [Asus Zenfone Live L1 Official Facebook Group](https://www.facebook.com/groups/1179335585483994/)

Helpful tools link below!
* [Unofficial TWRP](https://drive.google.com/file/d/1xoSJfIA_E8q4_ALA3klovVGrjUZCm_UU/view?usp=drivesdk). Extract before flashing this image file with Minimal ADB & Fastboot.
* [Decrypt Patch](https://drive.google.com/file/d/1sYyVHio1WZeyL68dawvQ9lqTqyqrXVMg/view?usp=drivesdk). Format data first in TWRP before installing this zip.
* [VoLTE Activator Patch](https://drive.google.com/file/d/19Kxs2SYVkkTVfMaTECFDsUmHa6a9RtB_/view?usp=drivesdk). Install this zip in TWRP.
* [Camera2 API Activator](https://drive.google.com/file/d/1-0yDk65Zt5DNf61mWzwEzQOuplWh2fwo/view?usp=drivesdk). Install this zip in TWRP.
* [GSI Storage Fix](https://drive.google.com/file/d/1-FqD98pl9DVXeve7uvlSdFagwTYnrItc/view?usp=drivesdk). For GSI who have problem with can't boot into homescreen & fixing storage can't be readed problem. List of GSI that need this patch :
 -AEX v6.3 GSI and above (official).
 -Resurrection Remix v7.0.x GSI (official).
 -AOSiP GSI.
 -LineageOS 16.0 GSI.