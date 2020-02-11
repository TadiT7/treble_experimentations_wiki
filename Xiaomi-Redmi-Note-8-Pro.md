## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera 64MP                    | Status: Working in 16MP mode |
| Camera Macro | Status: No support |
| Camera Ultrawide | Status: No support |
| Camera Depth Sensor | Status: *Untested* |
| Speaker / Mic             | Status: Working                                        |
| Media playback / Recording | Status: Working on AOSP 9, Not working on AOSP 10 ([#1028](https://github.com/phhusson/treble_experimentations/issues/1028)) |
| Bluetooth                 | Status: Working                                           |
| WiFi                      | Status: Working                                           |
| RIL | Status: Working on AOSP 10, Not working on AOSP 9 ([#1051](https://github.com/phhusson/treble_experimentations/issues/1051)) |
| VoLTE                     | Status: *Untested*                                       |
| Fingerprint               | Status: Working                                           |
| Offline Charging          | Status: Working                                     |
| Adaptive Brightness       | Status: Not working                                 |

Please add other features, if I have missed anything.

---
## Software Support
| Application |      Status                                              |
|---------------------------|-----------------------------------------------------------|
| Youtube |Crashes with NDK Mediacodec Errors when playing video, First Frame Loads then crashes|
| AOSP Setup   | Functional with broken 2D Animations (ex. Animated Google Logo)|
| Twitter  | Crashes with NDK Mediacodec Errors when playing video,  First Frame Loads then crashes |
---
Tested By:
1. Username: hopefullyidontgetbanned
   - Model: Redmi Note 8 Pro (Begonia)
   - Region: United States
   - MIUI Vendor: MIUI Global Stable 10
   - GSI: AOSP 10.0 v208 A/B ARM64

2. Username: tvardero
   - Model: Redmi Note 8 Pro Global (begonia)
   - Region: Ukraine
   - MIUI Vendor: MIUI Global Stable 11
   - GSI: phh's AOSP 10 ARM64 A/B v208; phh's AOSP 9 ARM64 A/B v123