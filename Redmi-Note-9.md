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