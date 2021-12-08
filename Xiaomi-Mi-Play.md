## Xiaomi Mi Play
It's an arm64 A-only vndklite device.

Rom tested: lineage-16.0-20191017-UNOFFICIAL-treble_arm64_avN.img

What does not work:
* secure boot

### Steps to install

You need an unlocked bootloader and the stock firmare

1. Download the stock firmware and lineage-16.0-20191017-UNOFFICIAL-treble_arm64_avN.img rom.

1. Extract all files in the same folder.

1. Flash this image with the fastboot utility:

`$ fastboot --disable-verity --disable-verification flash vbmeta `

`$ fastboot flash system lineage-16.0-20191017-UNOFFICIAL-treble_arm64_avN.img`

`$ fastboot flash cache cache.img`

`$ fastboot flash userdata userdata.img`

`$ fastboot reboot`

Some more info

As an alternative you can flash via TWRP as "System Image" and format data.

### Hardware support
***

| Component     | Comment           |
| ------------- |:-------------:|
| Camera | Working | 
| Speaker / Mic | Working |  
| Bluetooth | Working | 
| WiFi | Working | 
| SIM / Mobile Data / Voice  | Working | 
| VoLTE | Not Tested | 
| Fingerprint | Working | 
| NFC | N/A | 
| Offline Charging | Working |
| Camera | Working |   
| Secure boot | Not working |   

***

Tested By: gokur20 - Xiaomi Mi Play(Europe), lotus_global_images_V11.0.10.0.OFIMIXM_20210108.0000.00_8.1_global  - 26/08/2021

