# Timovi Insignia Delta 3 (MT8321)

Tested AOSP 10 v207 and AOSP 11 v30x
* What's working on AOSP v207:
WiFi, Bluetooth (for some reason if you try to send an APK file to the target device it will give an error "Unsupported content"), Calls (both sending calls and receiving are working), SMS (both sending and receiving are working too), brightness, camera, etc.
* What's not working:
Hotspot, screen rotation is messed up (only in AOSP 11) and camera is flipped 90° (also only on AOSP 11), etc.

**Warning: for some reason in AOSP 11 v309+, SystemUI will no longer work on this device.**

## Steps to install

* Step 1: `fastboot OEM unlock` / `fastboot flashing unlock`
* Step 2: disable force encryption (data encryption are not tested yet! Ignore this step under your own risk!) in `/vendor/fstab.mt6580`
* Step 3: factory reset with stock Recovery
* flash this image with the `fastboot` utility:
    ```
    $ a-command
    $ fastboot flash system system-arm-aonly-gogapps.img
    ```
    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working fine (only in AOSP 10), it is flipped 90° in AOSP 11.                                                    |
| Speaker / Mic             | Speaker working fine, Microphone have been not tested yet.                                                   |
| Bluetooth                 | Working fine.                                                  |
| WiFi                      | Working fine.                                                    |
| Hotspot                   | Not working.                                                     |
| SIM / Mobile Data / Voice | For some reason you can't view contacts saved in SIM card or create new ones, Mobile data is working fine.                                                                                                      |                                                   |                                                                                                     |
| Other feature             | Dual Sim capabilities are not tested yet and screen rotation is broken (only in AOSP 11 v30x) as shown in [this issue](https://github.com/phhusson/treble_experimentations/issues/1770).                                                    |
---

Tested By: @acastillorobles77

Btw sorry for my horrible English, I'm still learning.
