# Huaiwei MediaPad M5 lite

**WARNING**: The information below seems to only be correct for the old AOSP 10 - based builds. The AOSP 11 - based builds do not boot on my device.

The [AOSP 10 image by phh](https://github.com/phhusson/treble_experimentations/releases/tag/v208) works mostly, AOSP 9 is stuck at boot.

Notable problems include: The fingerprint sensor seems not to work, device encryption seems unavailable.

## Steps to install

* Download a arm64 / a-only variant of phh's AOSP 10 GSI.
* Unlock the device using [this guide.](https://forum.xda-developers.com/mediapad-m5-lite/how-to/complete-guide-to-unlock-relock-lock-t3989111) **NOTE**: If your device has the string "C431" in its hardware revision, you need to use the method by user *drumiec* in the linked thread.
* Flash the AOSP 10 GSI using [the method introduced here as "flasing a GSI without TWRP".](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)
* ???
* Profit

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | working                                                    |
| Speaker / Mic             | working                                                    |
| Bluetooth                 | working, but audio is jittery                                                    |
| WiFi                      | working                                                    |
| SIM / Mobile Data / Voice | n/a                                                    |
| VoLTE                     | n/a                                                    |
| Fingerprint               | **not working**                                                    |
| NFC                       | *untested*                                                    |
| Encryption             | **not working**                                                    |
---

Tested By: @tinloaf - Model-Number "BAH2-W19 8.0.0.0.230(W431)" - Date tested: 30.12.2019
