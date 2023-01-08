Hello folks,

i could have system-squeak-arm64-ab-vanilla.img image flashed, 
what i did:

1) installed twrp-3.7.0_12-0-avicii.img, flashed to recovery
2) adb reboot fastboot
3) get vbmeta and vbmeta_system.img from lineage
    lineage-19.1-20221227-UNOFFICIAL-avicii-microG.zip
    by getting them out from payload.bin
4) used following flash.sh

~~~
#!/bin/sh
#
# Done from Angelo Dureghello

fastboot reboot fastboot
fastboot flash system system-squeak-arm64-ab-vanilla.img
fastboot --disable-verity flash vbmeta vbmeta.img
fastboot --disable-verity flash vbmeta_system vbmeta_system.img
fastboot -w
fastboot reboot
~~~