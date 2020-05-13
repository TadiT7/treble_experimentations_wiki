**Tested on:**
- phh's AOSP v212, both vanilla and gappsed
- AndyYan's LOS v17.1-20200227 

## Hardware support:
| Component | Status |
|-|-|
| Camera 64MP | Works only in 16MP mode, even on Google Camera Port. |
| Camera Macro | Use listed below camera apps. |
| Camera Ultrawide | Use listed below camera apps. |
| Camera Depth Sensor | Works as simple 2MP camera. |
| Speaker / Mic | Working |
| Bluetooth | Working |
| WiFi | Working |
| RIL | Working on AOSP 10, Not working on AOSP 9 ([#1051](https://github.com/phhusson/treble_experimentations/issues/1051)) |
| Double SIM | AOSP 10 - Working |
| Fingerprint | Working |
| Offline Charging | Working, but boots into recovery after plug-in. |
| NFC | Working |
| IR blaster | Working |

You can found GCam Port here, but it's very buggy on GSIs: [telegram chat (speak english only!)](https://t.me/rn8pro_gcam).
Also apps that works with multi cameras: Open Camera (from Google Play), HedgeCam2 (from Google Play). Don't forget to swith on Camera2API, in other case you can't set manually camera exposure.

## Software Support:
| Component | Status |
|-|-|
| Performance and random reboots | Little bit unstable, random little freezes and lags. No random reboots. |
| Bluetooth calls | Working |
| Auto-brightness | Working |
| SafetyNet and Google Pay | See fix below. | 
| Media playback / Recording | See fix below. |
| Nightlight | See fix below. |
| Mirrorcast | Not working. |
| VoLTE | *Untested* |
| Notch and rounded corners detection | Working |

Please, edit page and add other major features, if I have missed any.

## Bugs:
*Please, read issue [#1028](https://github.com/phhusson/treble_experimentations/issues/1028) first before adding new bugs here or creating new issues on repo.*
| Bug | Status |
|-|-|
| Camera is glitchy in some apps like Viber | Please, be updated with [#1154](https://github.com/phhusson/treble_experimentations/issues/1154) issue. |

## Fixes:
#### Nightlight fix
**Problem:** Nightlight is flickering with strong orange color on screen updates.
**Solution:** Go to developer settings (unlock them first), turn on "Disable HW overlay" ("Отключить аппаратное наложение"). Apply this after each reboot. **Note that this will lower your phone performance.**

#### Media fix
**Problem:** No sound, no video, no notifications and alarms, no ringtones. Apps crash when trying record or play sound, or stuck on 0:00.
**Solution:** Add those lines to the end of file /etc/prop.default (root needed, mount partition r/w):
```
debug.stagefright.omx_default_rank.sw-audio=1
debug.stagefright.omx_default_rank=0
```

#### Google Pay and SafetyNet:
**Problem:** basicIntegrity fail, ctsProfile fail.
**Solution:** Root explorer needed.
- To fix basicIntegrity remove folder /data/su. To prevent creation of this folder each reboot remove file (mount partition r/w): /etc/init/su.rc
- To fix ctsProfile, flash this module with Magisk Manager: [module.zip](https://drive.google.com/open?id=1mlAWmNJdJnN77rZN0AvGddURxh65RXxU) and reboot.
- Also you want to uninstall vanilla SU apk: me.phh.superuser to stop getting notification about update of binary file.

**Solution #2:**
See installation option #2

## Installation:
Your **warranty** will be **void** if not already. **Proceed on your own risk.** I'm (tvardero) not responsible for any damage made to your phones.

Dependencies: unlocked bootloader, TWRP (not official one), stock MIUI (rooted/unrooted).

Use only **ARM64 A/B** GSIs. Use of sGSI is not recommended, they weren't tested yet.

1. Go to TWRP and make backup of System and Data partitions. **You DON'T need to backup other partitions such as Vendor or Boot, because if you do restore them once, you will GET A SOFTBRICK.**
2. Format -> Format Data -> Type "yes". Do NOT format system and any other partition.
3. Install -> Flash image -> Select your GSI.img and flash it as "System image".
4. If you are sure that your GSI comes without GApps, then flash [latest GApps](https://opengapps.org/) made for ARM64, nano or micro (if available) are recommended. If you encounter error 20, then mount system. If you encounter error 70, then go to "wipe" -> "advanced" -> select system partition -> "resize or repair" -> resize partition first -> then repair partition, now you can flash GApps.
5. If you wish, you can root with Magisk. Go to TWRP Advanced -> Root device. Then you can update your Magisk binary later with Magisk Manager.
6. Boot into system.
7. Apply some fixes, like brightness slider fix and others. DONE.

**Option #2:**
- Fastboot flash stock rom
- Fastboot flash Phh gsi
- `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`
- Boot gsi, do not setup, go to Phh Settings -> securize, wait for reboot, see bootloop
- Go to stock recovery and factory reset (wipe)
- Setup, device should be encrypted, non-rooted, passing Safetynet

## Uninstall: 
Before anything, wipe system partition and "format data -> yes".
 - If you wish to **change GSI**: restore System partition from your backup made on step 1, boot once, go back to TWRP and continue from step 2.
 - If you wish to **go back to stock**: format Data -> yes, restore System partition, reboot to system, then restore Data. Please note, that your lockscreen password will be reset, but not your fingers.

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
   - GSI: phh's AOSP 10 ARM64 A/B v212
   - GSI: AndyYan's LOS v17.1-20200227 

3. Username: timbortnik
   - Model: Redmi Note 8 Pro (begonia) Global ver.
   - Region: Ukraine
   - MIUI Vendor: MIUI Global Stable 11 (Pie vendor)
   - GSI: phh's AOSP 10 ARM64 A/B v216

More testers needed.