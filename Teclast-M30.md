No special flash settings for the GSI are required (not known for me). Process is as generically stated on XDA pages. The display scaling is much smaller than OEM ROM on 2K screen, but you can set custom DPI in settings. 

As an alternative you can flash via TWRP as "System Image" and format data.
Stock maybe flashed via fasboot and SP Flash Tool: [thread about SPFT on russian 4pda](https://4pda.ru/forum/index.php?showtopic=469340)

Device version **M4P7** [official stock v3 link](https://mega.nz/#!1FY1BA4Q!aLM899AghOQHnnDdR5f_6L0IqADZxUieKJqqYwhi2rI)

Device version **M5P3** [official stock v1.02 link (no google play services)](https://mega.nz/file/3wAQDIrA#44HoXZxLt19mPo1XbzRbMPSCuZ9kZKIRWTWPvUJJhdY)

Device version **M6P4** [official rom v1 link](https://yadi.sk/d/-2QpFnbGK95v8A)



At future possible ( [asuvoro](https://github.com/asuvoro) ) will change rom-links to torrents.
If you have stock firmware, tell me.

## Tested
This device is arm64 A-only with VNDK version 26.0, choose arm64-aonly when downloading an images.
Only some Android Pie 9 (below) boots and works.

### Android 9
* Havoc-OS v2.9 [XDA](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/-t3930030/)
* Lineage OS 16.0 GSI
* AOSP 9.0 v123 [phhusson/treble_experimentations/releases](https://github.com/phhusson/treble_experimentations/releases/tag/v123)
* Descendant 4.0.1 for Treble Enabled Devices [XDA](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/descendant-android-pie-custom-rom-ver-t3840578)

### WIP Android 10
* AOSP v10.0 v213 [phhusson/treble_experimentations/releases](https://github.com/phhusson/treble_experimentations/releases/tag/v213)
In release applied fix for lib's : dlopen failed: library "libstdc++.so" not found
Maybe you still have to copy it in /vendor/lib/libstdc++.so [(details issue #1134)](https://github.com/phhusson/treble_experimentations/issues/1134) (+ magisk_pphusson + magisk_4_gsi_fix if needed)


### POST FLASH INSTRUCTIONS
fill it in if you know

## Hardware support (not tested fully)

| Component                 |      Comment                                 |
|---------------------------|----------------------------------------------|
| Camera                    | Work                                         |
| Speaker / Mic             | Work                                         |
| Bluetooth                 | Work (turn on workaround in phh-settings)    |
| WiFi                      | Work                                         |
| SIM / Mobile Data / Voice | Work                                         |
| SDcard                    | Not tested                                   |
| VoLTE                     | Not tested                                   |
| Sensors / Rotation        | Ok                                           |
| Sensors                   | Others?                                      |
| GPS                       | Seems not working                            |
| Fingerprint               | No hardware                                  |
| NFC                       | No hardware                                  |
| Offline Charging          | Not tested                                   |
| Other feature             | Needs to be added                            |
---

[SGI's list](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)

---
