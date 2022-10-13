# Pre-flash info

- Device name: Xiaomi Redmi Note 10S (secret; rosemary)
- Earlier rom: MIUI 12.5.14 (Global)
- Rooted: No

# Tested images

- Corvus OS
- phh's Android 12
- DotOS
- Pixel Experience
- LineageOS
- ProtonAOSP
- CAOS 11

# Steps to install

<https://forum.xda-developers.com/t/flashing-gsi-roms-on-redmi-note-10s-and-then-fixing-some-issues-all-without-any-custom-recovery.4337099/>

# Hardware Support post flashing

| Component | Comment|
| --- | --- |
| Camera | Works |
| Speaker/Mic | Works (headphone jack requires [tweak](#notes)) |
| Bluetooth | Works (audio requires [tweak](#notes)) |
| Wi-Fi | Works |
| SIM/Mobile Data/Voice | Works |
| VoLTE | Not tested |
| Fingerprint | Works |
| NFC | Works |
| Offline Charging | Works |
| Display Refresh rate | 60Hz |
| Screen Brightness | Works (buggy before [tweak](#notes)) |
| Volume scale | Works |
| 5G | N/A |
| SafetyNet post root | Passed |
| WideVine certification post flash and root | L1 |

# Notes

- For double tap to wake enable it in `Xiaomi features > Enable DT2W` (does not work with AOD)
- For headphone jack enable `Misc features > Use alternate way to detect headsets`
- If you want AOD enable it in `Misc features > Force allow Always-On Display`
- For brightness enable `Misc features > Force alternative backlight scale`
- For bluetooth audio enable `Misc features > Force-disable A2DP offload`
- If the sim card does not connect to the network, check the IMEI. It's a common problem on MTK based devices. If it is not present, try to define it. (There are different methods to do this. Be aware of what you are touching Network related operations are quite sensitives.)

# Useful links

- IMEI Backup : 'https://drive.google.com/file/d/1krl_rG2G-wFg80nhBGtbuxpUICVGfNI2/view'
- IMEI Write Procedure : 'https://youtu.be/dBChdd40EuU'
