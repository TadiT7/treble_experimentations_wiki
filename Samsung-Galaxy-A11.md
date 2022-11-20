# Samsung Galaxy A11 

![galaxya11](https://user-images.githubusercontent.com/46762446/199036043-3ffd82ce-db40-493e-b423-cdc000e3a3a5.png)


###   Summary: This device uses `a64` GSI variants. GSI images should work, so long as they're based on [v413](https://github.com/phhusson/treble_experimentations/releases/tag/v413) or later. 

   Please note the following: 
* Android 11-based GSI images (ie. dotOS 5.2) may suffer from watchdog issues related to /dev/watchdog0. Android 12-based GSI images do not have this issue.
* This device has multiple variants, but this doc only applies to the North American version of the Galaxy A11. 
* **Other variants (ie. SM-A115F/DS) may have different OEM unlock instructions and methods,** but the rest of the information here should still apply.



## Flashing Quirks

### This device will require cross-flashing to enable the OEM Unlock toggle.

   Currently the SM-A115U and SM-A115U1 models are common, but the A115U variant has no unlock toggle. 
   Both variants have interchangeable firmware, luckily, and will need to be switched to continue. **Please check XDA if you don't know how to do this, as the Telegram group may not provide reliable support.**

### You will need to install GSI images using TWRP or OrangeFox's `Flash as System Image` option.

   Some ROMs may need to be resized using `resize2fs` before they'll fit on /system_root. See below for hardware and partition support information.
   

***


## Hardware Support

| Component                 |      Status                                               |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                        |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | SIM/Data OK, but VoLTE is required for calls.             |
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

## Resizing GSI Images **(Experimental, not supported!)**
  * `e2fsck -f /path/to/GSI/image.img`
  * `resize2fs /path/to/GSI/image.img 2590M`

![image](https://user-images.githubusercontent.com/46762446/199031383-da9319df-02d4-4008-842a-3435b212a47e.png)


***


## Metadata:

Tested By: @starfoxdot64 

Test Date: 10/31/2022

Model: [SM-A115U](https://samfw.com/firmware/SM-A115U1)

Firmware Version: [A115U1UES7BVF1](https://samfw.com/firmware/SM-A115U1/ATT/A115U1UES7BVF1)

