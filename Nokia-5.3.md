# [Nokia 5.3] - [CaptainAmerica / CAP]

Bootloader Unlock : https://forum.xda-developers.com/t/guide-heres-how-to-unlock-the-bootloader-of-nokia-5-3.4568619/

## Hardware Support (Android 13)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| NFC                       | ?                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | √                                                         |
| Fingerprint               | √                                                         |


## Additional Notes

Tested GSI: https://forum.xda-developers.com/t/gsi-13-lineageos-20-trebledroid-based.4517345/ , arm64 bgN variant.

You'll need stock firmware for this phone to install GSI properly, to do that:
1. The stock firmware I used has filename "HMDSW_TA-1229-340A-0-00WW-B01_user_devicekit.zip". Extract it twice.
2. Assuming you're using Windows. Extract fastboot.exe, AdbUsbApi.dll and AdbWinUsbApi.dll from latest Platform Tools (**DO NOT USE MINIMAL ADB AND FASTBOOT!**) into the stock firmware directory. Edit `sm6125_fastboot_all_images.bat` as follows, then open it:
```
@echo off
fastboot flash  xbl_a  xbl.elf
fastboot flash  xbl_b  xbl.elf
fastboot flash  xbl_config_a  xbl_config.elf
fastboot flash  xbl_config_b  xbl_config.elf
fastboot flash tz_a tz.mbn
fastboot flash tz_b tz.mbn
fastboot flash rpm_a rpm.mbn
fastboot flash rpm_b rpm.mbn
fastboot flash hyp_a hyp.mbn
fastboot flash hyp_b hyp.mbn
fastboot flash boot_a boot.img
fastboot flash boot_b boot.img
fastboot flash vbmeta_system_a vbmeta_system.img
fastboot flash vbmeta_system_b vbmeta_system.img
fastboot flash recovery_a recovery.img
fastboot flash recovery_b recovery.img
fastboot flash keymaster_a km4.mbn
fastboot flash keymaster_b km4.mbn
fastboot flash cmnlib_a cmnlib.mbn
fastboot flash cmnlib_b cmnlib.mbn
fastboot flash cmnlib64_a cmnlib64.mbn
fastboot flash cmnlib64_b cmnlib64.mbn
fastboot flash modem_a NON-HLOS.bin
fastboot flash modem_b NON-HLOS.bin
fastboot flash dsp_a dspso.bin
fastboot flash dsp_b dspso.bin
fastboot flash abl_a abl.elf
fastboot flash abl_b abl.elf
fastboot flash bluetooth_a BTFM.bin
fastboot flash bluetooth_b BTFM.bin
fastboot flash dtbo_a dtbo.img
fastboot flash dtbo_b dtbo.img
fastboot flash imagefv_a imagefv.elf
fastboot flash imagefv_b imagefv.elf
fastboot flash uefisecapp_a uefi_sec.mbn
fastboot flash uefisecapp_b uefi_sec.mbn
fastboot flash metadata metadata.img
fastboot flash devcfg_a devcfg.mbn
fastboot flash devcfg_b devcfg.mbn
fastboot flash qupfw_a qupv3fw.elf
fastboot flash qupfw_b qupv3fw.elf
fastboot flash super super.img
fastboot flash userdata userdata.img
fastboot --disable-verity --disable-verification flash vbmeta_a vbmeta.img
fastboot --disable-verity --disable-verification flash vbmeta_b vbmeta.img
fastboot flash logfs logfs_ufs_8mb.bin
fastboot flash storsec storsec.mbn
fastboot --set-active=a reboot-fastboot
fastboot delete-logical-partition system
fastboot delete-logical-partition product
fastboot delete-logical-partition system_ext
fastboot delete-logical-partition vendor
fastboot delete-logical-partition system_a
fastboot delete-logical-partition product_a
fastboot delete-logical-partition system_ext_a
fastboot delete-logical-partition vendor_a
fastboot delete-logical-partition system_b
fastboot create-logical-partition vendor_a 1024
fastboot create-logical-partition system_ext_a 1024
fastboot create-logical-partition system_a 1024
fastboot flash vendor_a vendor.img
fastboot flash system_ext_a system.img
fastboot flash system_a your_gsi_image.img
fastboot reboot-recovery
```

3. Choose wipe data/factory reset there to perform a factory reset, and reboot, otherwise internal storage space will only have 16GB. If you forget to perform factory reset, then you'll need to perform regular factory reset in settings.

To restore it back to stock firmware, you'll have to flash entire super partition under Bootloader mode (not Fastbootd):
```
fastboot flash super super.img
fastboot flash userdata userdata.img
fastboot reboot
```

## Tested By:

@HikariCalyx @ Nokia 5.3 TA-1223 00WW_3_40A (CAP-340A-0-00WW-B01) @ 28/03/2023


Template created by @zguithues