 # Asus Zenfone Live L1 (ZA550KL)

Front and back camera both working. Stock GSI ROM camera is working fine with few bugs, flash on stock camera if set to on or auto the camera will launch force close. Also the camera are pitch black/dark on some GSI ROM. If we using the front camera, we will see our face rendered very weird (AICP-mordiford by AndroPlus is one of many example of GSI ROM with pre-installed bugs free/normal camera). Install 3rd party camera apps will solve the problem like Open Camera app.

## Steps to install

* Extract the image file (if it compressed, like zip or xz).
* Boot into TWRP (if you already have TWRP installed).
* Flash the image file into the System Image partition.
* Flash this image with the `fastboot` utility if you not have TWRP installed. Reboot your device to fastboot mode before:
    ```
    fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    **DON'T EVER WIPE VENDOR PARTITION! IT'S A GSI, NOT AN OFFICIAL CUSTOM ROM!**

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working with bugs                                                    |
| Speaker / Mic             | Working                                                    |
| Bluetooth                 | Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| VoLTE                     | Not working, need a patch.                                                    |
| Hotspot                   | Working                                                    |
| Flashlight                | Working                                                    |
| Offline Charging          | Working                                                    |
| Other feature             | Not tested at all                                                    |
---

Tested By: AcAciA, Maulana Kurniawan, Satu Prasetyo Gilang Mahameru - ASUS_X00RD, WW-15.01.xxxx.xxx - September 14, 2018 - Template created by @maulaaana, @zguithues and @hackintosh5

Join our Asus Zenfone Live L1 Indonesia Official Telegram Group here https://t.me/ZenfoneLiveL1