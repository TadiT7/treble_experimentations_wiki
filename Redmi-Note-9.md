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