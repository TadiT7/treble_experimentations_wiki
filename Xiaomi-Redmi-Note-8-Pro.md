## Hardware support:

| Component | Comment |
|-|-|
| Camera 64MP | Status: Works in 16MP mode |
| Camera Macro | Status: No support |
| Camera Ultrawide | Status: No support |
| Camera Depth Sensor | Status: *Untested* |
| Speaker / Mic | Status: Working |
| Bluetooth | Status: Working |
| WiFi | Status: Working |
| RIL | Status: Working on AOSP 10, Not working on AOSP 9 ([#1051](https://github.com/phhusson/treble_experimentations/issues/1051)) |
| Fingerprint | Status: Working |
| Offline Charging | Status: Working |

## Software Support:

| Component | Comment |
|-|-|
| Media playback / Recording | Status: Working on AOSP 9, Not working on AOSP 10 ([#1028](https://github.com/phhusson/treble_experimentations/issues/1028)) |
| Brightness | Status: Not working, but overlay was made ([Pull req. #174](https://github.com/phhusson/vendor_hardware_overlay/pull/174)) |
| VoLTE | Status: *Untested* |

Please add other features, if I have missed anything.

## Bug reports:

| Application |      Status                                              |
|---------------------------|-----------------------------------------------------------|
| YouTube / Twitter | Crashes with NDK Mediacodec, Errors when playing video, First Frame Loads then crashes on AOSP 10 |
| Android Setup Master / Android Settings | Broken embedded 2D animations on AOSP 10 |
| Audio Recorder | Crash on start of recording on AOSP 10 |
---

### Tested By:
1. Username: hopefullyidontgetbanned
   - Model: Redmi Note 8 Pro (Begonia)
   - Region: United States
   - MIUI Vendor: MIUI Global Stable 10
   - GSI: AOSP 10.0 v208 A/B ARM64

2. Username: tvardero
   - Model: Redmi Note 8 Pro (begonia) Global ver.
   - Region: Ukraine
   - MIUI Vendor: MIUI Global Stable 11
   - GSI: phh's AOSP 10 ARM64 A/B v208; phh's AOSP 9 ARM64 A/B v123