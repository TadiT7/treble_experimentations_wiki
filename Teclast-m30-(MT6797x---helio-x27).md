No special flash settings for the GSI are required (not known for me). Process is as generically stated on XDA pages. The display scaling is much smaller than OEM ROM on 2K screen, but you can set custom DPI in settings. 

As an alternative you can flash via TWRP as "System Image" and format data.
Stock maybe flashed via fasboot and SP Flash Tool: [thread about SPFT on russian 4pda](https://4pda.ru/forum/index.php?showtopic=469340)

Device version M4P7 [official stock v3 link](https://mega.nz/#!1FY1BA4Q!aLM899AghOQHnnDdR5f_6L0IqADZxUieKJqqYwhi2rI)

Device version M6P4 [official rom v1 link](https://yadi.sk/d/-2QpFnbGK95v8A)

At future possible ( [asuvoro](https://github.com/asuvoro) ) will change rom-links to torrents.
If you have stock firmware, tell me.

## Tested
This device is arm64 A-only with VNDK version 26.0, choose arm64-aonly when downloading an images.
Only some Android Pie 9 (below) boots and works.

### Android 9
* Havoc-OS v2.9 [XDA](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/-t3930030/)
* Lineage OS 16.0 GSI
* AOSP 9.0 v123 [phhusson/treble_experimentations/releases](https://github.com/phhusson/treble_experimentations/tree/v123)
* Descendant 4.0.1 for Treble Enabled Devices [XDA](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/descendant-android-pie-custom-rom-ver-t3840578)

### WIP Android 10 (no booting yet)
* AOSP v10.0 v211 [phhusson/treble_experimentations/releases](https://github.com/phhusson/treble_experimentations/tree/v211)

### POST FLASH INSTRUCTIONS
fill it in if you know

## Hardware support (not tested fully)

| Component                 |      Comment                                 |
|---------------------------|----------------------------------------------|
| Camera                    | Work                                         |
| Speaker / Mic             | Work                                         |
| Bluetooth                 | Not working                                  |
| WiFi                      | Work                                         |
| SIM / Mobile Data / Voice | Glitches / Secondary SIM seems not working   |
| SDcard                    | Not tested                                   |
| VoLTE                     | Not tested                                   |
| Sensors                   | Not tested                                   |
| GPS                       | Seems not working                            |
| Fingerprint               | No hardware                                  |
| NFC                       | No hardware                                  |
| Offline Charging          | Not tested                                   |
| Other feature             | Needs to be added                            |
---

[SGI's list](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)

---
