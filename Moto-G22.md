Tested & Working with [android_13.0.0_r41 ci-20230417](https://github.com/TrebleDroid/treble_experimentations/releases/tag/ci-20230417)
## Hardware Support (Android 13)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ✓                                                         |
| Speaker / Mic             | ✓ (Volume bar is too large so audio could distort, need workaround idk how atm)   |
| Bluetooth                 | ✓                                                         |
| WiFi                      | ✓                                                         |
| SIM / Mobile Data / Voice | ✓                                                         |
| VoLTE                     | ? (Needs further testing, i will update)                  |

Since this device has MTK SoC, i really suggest to dump all partitions using [MTKClient](https://github.com/bkerler/mtkclient)
just type
-`python mtk rl foldername --skip userdata` to dump all partitions except userdata, copy boot_*.bin, vbmeta_*.bin
after complete, follow the steps to unlock bootloader, search the commands in MTKClient readme
and flash vbmeta_*.bin from dump in fastboot with this command
-`fastboot --disable-verity --disable-verification flash vbmeta vbmeta_*.bin`

Now the actual installation begins
- `fastboot reboot fastboot` to boot into fastbootd, this is necessary to access system/vendor/product/... partitions
- in this mode if `fastboot devices` throws nothing, install [Rescue and Smart Assistant](https://www.motorola.com/us/rescue-and-smart-assistant/p) to get fastbootd drivers
- now flash system as usual `fastboot flash system.img`
- if this command fails, image is too big, delete product partition to get some space with `fastboot delete-logical-partition product_a`, replace product_a to product_b if active slot is b and rerun the system flash command.
- now in the phone move with vol and select with power, don't reboot yet, go to into recovery mode and here wipe data factory reset, dont wipe in fastboot to avoid encryption issues
- reboot

## Workarounds
If you don't have internet but wifi/mobile is really working, see [here](https://forum.xda-developers.com/t/gsi-13-lineageos-20-light.4509315/#post-87620773) for workaround 

If 3.5mm jack is not detected
- Go to Settings
- Phh Treble Settings
- Misc Features
- Check Use alternate way to detect headsets
- Reboot 

No adaptative brightness
Needs overlay, i will make one Soon™