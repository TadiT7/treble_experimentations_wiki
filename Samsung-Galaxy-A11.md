# Samsung Galaxy A11

   Summary: This device uses `a64` GSI variants. GSI images should work, so long as they're based on [v413](https://github.com/phhusson/treble_experimentations/releases/tag/v413) or later. 

   Note: Android 11-based GSI images (ie. dotOS 5.2) may suffer from watchdog issues related to /dev/watchdog0. Android 12-based GSI images do not have this issue.



## Flashing Quirks

   **You will need to install GSI images using TWRP or OrangeFox's `Flash as System Image` option.**

   Some ROMs may need to be resized using `resize2fs` before they'll fit on /system_root. See below for hardware and partition support information.
   

***


## Hardware Support

| Component                 |      Status                                               |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                        |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | Not available on Samsung devices with Qualcomm processors. See [this message](https://t.me/phhtreble/570295) from the official Telegram group.|
| Fingerprint               | OK                                                        |
| NFC                       | Not applicable for this device.                           |
| Offline Charging          | OK                                                        |
---

## Partition Information

| Partition      |      Maximum Filesize       |
|----------------|-----------------------------|
| /system_root   | 2.6GB                       |
| /product       | 692MB                       |
| /vendor        | 522MB                       |

## Resizing GSI Images
  * `e2fsck -f /path/to/GSI/image.img`
  * `resize2fs /path/to/GSI/image.img -s <partition size, 2.5G for example>`



***


## Metadata:

Tested By: @starfoxdot64 

Test Date: 10/31/2022

Model: [SM-A115U](https://samfw.com/firmware/SM-A115U1)

Firmware Version: [A115U1UES7BVF1](https://samfw.com/firmware/SM-A115U1/ATT/A115U1UES7BVF1)

