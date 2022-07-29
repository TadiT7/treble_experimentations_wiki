# Tested/Working images
- [aosp_arm64-exp-TPB4.220624.008-8853201-2021523b.zip (A13-TPB4)](https://developer.android.com/about/versions/13/gsi-release-notes#downloads)
- [system-squeak-arm64-ab-vndklite-vanilla-secure.img.xz (upto v415)](https://github.com/phhusson/treble_experimentations/releases)
- [PixelExperience_Plus_arm64-ab-vndklite-12.1-20220722-UNOFFICIAL.img.xz (upto v415)](https://github.com/ponces/treble_build_pe/releases)
- [crDroid-8.7-arm64_bvN-vndklite-Unofficial.img.xz](https://sourceforge.net/projects/gsi-projects/files/v415/crDroid-8.7/crDroid-8.7-arm64_bvN-vndklite-Unofficial.img.xz/download)

# Not working
- [lineage-19.1-20220719-UNOFFICIAL-arm64_bvS-vndklite.img.xz](https://sourceforge.net/projects/andyyan-gsi/files/lineage-19.x) `Does not boot at all`

# Steps to install

```
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img
fastboot -w
```


# Hardware Support

| Component | State & Recommended tweaks  |
| --- | --- |
| Camera | Works (OpenCam & most of the GCam variants) |
| Speaker/Mic | Works ( Phh Settings > Qualcomm features > **Use alternate audio policy** & Misc features / **Disable audio effects** ) |
| Bluetooth | Works |
| Bluetooth Audio | Works ( Misc > **Force-disable A2DP offload** ) |
| Wi-Fi | Works |
| SIM/Mobile Data/Voice | Works ( Misc > **Install IMS Apk for Qualcomm vendor** ) |
| VoLTE | Works ( IMS features / **Request IMS network** & **Force the presense of 4G calling**) |
| Fingerprint | Works |
| NFC | Untested |
| Screen Brightness | Buggy ([PR to merge the fix](https://github.com/phhusson/vendor_hardware_overlay/pull/605)) |
| Auto Brightness | Doesn't exist ([PR to merge the fix](https://github.com/phhusson/vendor_hardware_overlay/pull/605)) |
| Volume scale | Works |
| 5G | N/A |
| SafetyNet post root | Passed (with [Redfin-Props](https://github.com/Pixel-Props/redfin/releases) & [safetynet-fix](https://github.com/kdrag0n/safetynet-fix/releases) in magisk) |
| WideVine certification post flash and root | L1 |
