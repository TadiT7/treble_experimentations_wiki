## Hardware support:
| Component | Status |
|-|-|
| Camera 64MP | Works only in 16MP mode |
| Camera Macro | No support |
| Camera Ultrawide | No support |
| Camera Depth Sensor | *Untested* |
| Speaker / Mic | Working |
| Bluetooth | Working |
| WiFi | Working |
| RIL | Working on AOSP 10, Not working on AOSP 9 ([#1051](https://github.com/phhusson/treble_experimentations/issues/1051)) |
| Fingerprint | Working |
| Offline Charging | Working, but has animation bootloop |
| NFC | *Untested* |

## Software Support:
| Component | Status |
|-|-|
| Media playback / Recording | Working on AOSP 9, Not working on AOSP 10 ([#1028](https://github.com/phhusson/treble_experimentations/issues/1028)) |
| Auto-brightness | Not working, but overlay was made ([Pull req. #174](https://github.com/phhusson/vendor_hardware_overlay/pull/174)) |
| VoLTE | *Untested* |
| Bluetooth calls | Working |

Please add other features, if I have missed anything.

## Bug reports:
| Application |      Status                                              |
|---------------------------|-----------------------------------------------------------|
| YouTube / Twitter | Crashes with NDK Mediacodec, Errors when playing video, First Frame Loads then crashes on AOSP 10 |
| Android Setup Master / Android Settings | Broken embedded 2D animations on AOSP 10 |
| Audio Recorder | Crash on start of recording on AOSP 10 |

## Installation:
Your warranty will be **nullified** if not already. **Proceed on your own risk.** I'm (tvardero) not responsible for any damage made to your phones.

Dependencies: unlocked bootloader, TWRP (not official one), stock MIUI (rooted/unrooted).

_Please note: if you wish to use Google Market, flash GSI with preinstalled GApps. Unfortunately, Gapps can't be flashed due error 20, resizing of system partition leads to bootloop._

1. Go to TWRP and make backup of System and Data partitions. **You DON'T need to backup other partitions such as Vendor or Boot, because if you do restore them once, you will GET A SOFTBRICK.**
2. Format -> Format Data -> Type "yes". Do NOT format system and any other partition.
3. Install -> Flash image -> Select your GSI.img and flash it as "System image".
4. Boot into system.
5. If you wish, you can root with Magisk. Go to TWRP Advanced -> Root device. Then you can update your Magisk binary later with Magisk Manager.
6. Apply some fixes, like brightness slider fix and others. DONE.

## Uninstall: 
 - If you wish to **change GSI**: restore System partition from your backup made on step 1, an then continue from step 2.
 - If you wish to **go back to stock**: restore System partition, reboot to system, then restore Data.

## Recovery:
|-|-|
| Got bootloop after restoring vendor / boot / any other partition | Flash **vendor -> firmware -> MIUI ROM** files from https://xiaomifirmwareupdater.com/ (begonia, mind your version (global or not)!) |
| Can't boot into recovery mode, but fastboot mode is ok | Same here |
| Can't boot nothing | Dry out your phone battery fully. After that plug your charger in, you will see charging animation. After that ASAP boot into fastboot and recover your phone |

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

More testers needed.