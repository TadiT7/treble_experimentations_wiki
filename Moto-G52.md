Installing GSI in Moto G52(rhode) is same like in many other devices. This device is a **Virtual A/B** device with recovery-as-boot.

Strange thing in this device is, even though it launched with Android 12, vndk and boot shows as Android 11 only. So we can even install Android 11 GSIs in this device.(Tested when I am in Moto Stock Android 12 S1SR32.38-132-3)

- `adb reboot fastboot` or if you are in fastboot mode run `fastboot reboot fastboot` to boot to fastbootd mode.
- `fastboot flash system system-gsi.img` to flash GSI. If this command fails, we have to remove product partition to get some space. `fastboot delete-logical-partition product_a`, replace product_a to product_b if active slot is b and rerun the system flash command.
- reboot to fastboot mode using `fastboot reboot bootloader`
- Download vbmeta from [here](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img) and flash using `fastboot flash vbmeta vbmeta.img`
- Wipe data using `fastboot erase userdata` and `fastboot erase metadata`
- Reboot to newly flashed system using `fastboot reboot`