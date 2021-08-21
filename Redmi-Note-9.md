Tested on:  
* LineageOS 18.1 20210808 from Andy Yan (with [modified rw-system.sh](https://github.com/notmyst33d/device_phh_treble/commit/81af8dbf47dcb1f20b836f9a9b22addae4d6e19e)), MIUI 12.5.1.0 vendor

## Hardware support
| Component | Status |
| --------- | ------ |
| WiFi (2.4 and 5 GHz) | Working |
| RIL | Working |
| Bluetooth | Working |
| USB tethering | Working |
| WiFi hotspot (2.4 and 5 GHz) | Working |
| Fingerprint | Working |
| Encryption | Working |
| Speaker / Microphone | Working |
| USB MTP/PTP/MIDI | Working |
| Camera | Working, auxiliary modules are not tested |
| NFC | Not tested |
| VoLTE | Not tested |
| IR blaster | Not tested |
| Offline charging | Broken, stays at OEM logo |

## Installing
You should have platform-tools and ADB/Fastboot driver installed
1. Download GSI and unpack it (you should have .img file at the end)
2. Reboot to fastboot (Power + Vol-)
3. Reboot to fastbootd: `fastboot reboot fastboot`
4. Disable vbmeta: `fastboot flash --disable-verification --disable-verity vbmeta (path to stock vbmeta.img)`
5. Flash GSI: `fastboot flash system (path to your GSI .img file)`
6. Wipe userdata: `fastboot format:ext4 userdata`
7. Reboot

## Installing with Magisk
You should have platform-tools and ADB/Fastboot driver installed
1. Download GSI and unpack it (you should have .img file at the end)
2. Download one of these recoveries: [OrangeFox R11.1](https://dl.uploadgram.me/60fd14cee2959h?dl), [SHRP](https://sourceforge.net/projects/shrp/files/merlin/SHRP_v3.1_stable-Official_merlin-1628943443.img/download), [TWRP 3.5.2_10.0](https://dl.uploadgram.me/611ff5e6e576dg?dl) (be aware that these links might be outdated, to get latest recoveries go to [@HelioG85_Updates](https://t.me/HelioG85_Updates))
3. Reboot to fastboot (Power + Vol-)
4. Disable vbmeta: `fastboot flash --disable-verification --disable-verity vbmeta (path to stock vbmeta.img)`
5. Flash recovery: `fastboot flash recovery (path to your recovery .img file)`
6. Reboot to fastbootd: `fastboot reboot fastboot`
7. Flash GSI: `fastboot flash system (path to your GSI .img file)`
8. Reboot to recovery: `fastboot reboot recovery`
9. Wipe->Format Data
10. Install Magisk
11. Reboot

## Fixing bugs
Currently Phh Treble settings cant apply presets for some reason, so you have to do enable these options:  
Misc features->Use alternative way to detect headsets (fixes headphone jack)  
Misc features->Force alternative backlight scale (fixes backlight)  
Misc features->Force-disable A2DP offload (fixes Bluetooth audio)

## Bugs and glitches
### Cant remount system as RW
For some reason blockdev errors out:
```
merlinnfc:/ # mount -o rw,remount /
'/dev/block/dm-0' is read-only
merlinnfc:/ # blockdev --setrw /dev/block/dm-0
blockdev: ioctl 125d: Permission denied
1|merlinnfc:/ #
```

### UI lagging
This problem was fixed by [this commit](https://github.com/notmyst33d/device_phh_treble/commit/81af8dbf47dcb1f20b836f9a9b22addae4d6e19e), however UI is still a bit laggy.