**Tested on:**
phh's AOSP v212 ARM64 A/B gappsed

## Hardware support:
| Component | Status |
|-|-|
| Camera 64MP | Works only in 16MP mode, even in Google Camera Port. |
| Camera Macro | Use Google Cemera Port. |
| Camera Ultrawide | Use Google Camera Port. |
| Camera Depth Sensor | *Unknown* |
| Speaker / Mic | Working |
| Bluetooth | Working |
| WiFi | Working |
| RIL | Working on AOSP 10, Not working on AOSP 9 ([#1051](https://github.com/phhusson/treble_experimentations/issues/1051)) |
| Double SIM | *Untested* |
| Fingerprint | Working |
| Offline Charging | Working, but has animation bootloop |
| NFC | *Untested* |
| IR blaster | Working |
You can found GCam Port here: telegram.

## Software Support:
| Component | Status |
|-|-|
| Performance | Little bit unstable, random little freezes and lags. |
| Random reboots | Not detected, phone is stable on this. |
| Mirrorcast | Not working. |
| SafetyNet -> Google Pay | Basic Integrity fail, CTS Profile fail. | 
| Media playback / Recording | Working, please apply sound fix on AOSP 10 ([#1028](https://github.com/phhusson/treble_experimentations/issues/1028)) |
| Notch and rounded corners detection | Working |
| Auto-brightness | Working. No "A" button, go to settings to turn it on. |
| Nightlight | Bugged. To fix flickering, disable HW overlay in developer settings after each reboot. |
| VoLTE | *Untested* |
| Bluetooth calls | Working |

Please, edit page and add other major features, if I have missed any.

## Bug reports:
*Please, read issue [#1028](https://github.com/phhusson/treble_experimentations/issues/1028) first.*
| Application | Status |
|-|-|
| None unfixed bug is reported |  |

## Installation:
Your **warranty** will be **void** if not already. **Proceed on your own risk.** I'm (tvardero) not responsible for any damage made to your phones.

Dependencies: unlocked bootloader, TWRP (not official one), stock MIUI (rooted/unrooted).

*Please note: if you wish to use Google Market, flash GSI with preinstalled GApps. Unfortunately, Gapps can't be flashed due error 20, resizing of system partition leads to bootloop.*

**ARM64 A/B**

1. Go to TWRP and make backup of System and Data partitions. **You DON'T need to backup other partitions such as Vendor or Boot, because if you do restore them once, you will GET A SOFTBRICK.**
2. Format -> Format Data -> Type "yes". Do NOT format system and any other partition.
3. Install -> Flash image -> Select your GSI.img and flash it as "System image".
4. Boot into system.
5. If you wish, you can root with Magisk. Go to TWRP Advanced -> Root device. Then you can update your Magisk binary later with Magisk Manager.
6. Apply some fixes, like brightness slider fix and others. DONE.

## Uninstall: 
 - If you wish to **change GSI**: restore System partition from your backup made on step 1, an then continue from step 2.
 - If you wish to **go back to stock**: restore System partition, reboot to system, then restore Data. Please note, that your lockscreen password will be reset, but not your fingerprints.

## Recovery:
| Problem | Solution |
|-|-|
| Got bootloop after restoring vendor / boot / any other partition | Flash **vendor -> firmware -> MIUI ROM** files from https://xiaomifirmwareupdater.com/ (begonia, mind your version (global or not)!) |
| Can't boot into recovery mode, but fastboot mode is ok | Recovery is broken. Flash TWRP recovery.img using ADB. Do not use official version, it doesn't have AVB patcher. |
| Can't boot nothing, even fastboot mode | Dry out your phone battery fully. After seeing critical battery charge logo (~5 days after), plug your charger in. Wait some time until Redmi logo. After that you can boot into fastboot and recover your phone. |
| HardestBrick | Service center |

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
   - GSI: phh's AOSP 10 ARM64 A/B v212; phh's AOSP 9 ARM64 A/B v123

More testers needed.