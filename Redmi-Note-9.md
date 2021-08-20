Tested on:  
* LineageOS 18.1 20210808 from Andy Yan (with [modified rw-system.sh](https://github.com/notmyst33d/device_phh_treble/commit/81af8dbf47dcb1f20b836f9a9b22addae4d6e19e)), MIUI 12.5.1.0 vendor

## Hardware support
| Component | Status |
| --------- | ------ |
| WiFi (2.4 and 5 GHz) | Working |
| RIL | Working |
| Bluetooth | Working |
| NFC | Not tested |
| Camera | Working, auxillary modules are not tested |

## Bugs and glitches
### Cant remount system as RW
For some reason blockdev errors out:

### UI lagging
This problem was