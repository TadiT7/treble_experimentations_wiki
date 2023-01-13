Installing GSI in Moto G52(rhode) is same like in many other devices. This device is a **Virtual A/B** device with recovery-as-boot.

Strange thing in this device is, even though it launched with Android 12, vndk and boot shows as Android 11 only. So we can even install Android 11 GSIs in this device.(Tested when I am in Moto Stock Android 12 S1SR32.38-132-3)

- `adb reboot fastboot` or if you are in fastboot mode run `fastboot reboot fastboot` to boot to fastbootd mode.
- `fastboot flash system system-gsi.img` to flash GSI. If this command fails, we have to remove product partition to get some space. `fastboot delete-logical-partition product_a`, replace product_a to product_b if active slot is b and rerun the system flash command.
- reboot to fastboot mode using `fastboot reboot bootloader`
- Download vbmeta from [here](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img) and flash using `fastboot flash vbmeta vbmeta.img`
- Wipe data using `fastboot erase userdata` and `fastboot erase metadata`
- Reboot to newly flashed system using `fastboot reboot`

For Indian Jio SIM Card users, signal may not show. To fix this, go to `Setting` -> `Network & internet` -> `SIMs` -> `Preferred network type` and choose `LTE (recommended)` instead of `3G`. Now Jio will work.

To fix VoLTE goto `Settings` -> `Phh Treble Settings` -> `IMS features` and check available options, tap on `Install IMS APK for Qualcomm pre-S vendor (Motorola)`. It will download a apk(check notification area). After download finish, install it by tapping on notification(it is a bug which not installs automatically) and go back to IMS settings and tap on `Create IMS APN`. Now reboot to use VoLTE.

<details>
<summary><b>My tests</b></summary>

- I installed phh AOSP 13 from [this](https://github.com/TrebleDroid/treble_experimentations/releases/download/ci-20230104/system-td-arm64-ab-vndklite-vanilla.img.xz)
- resized to increase space using `fastboot resize-logical-partition system_a 4294967296`
- Flashed NikGApps core from [here](https://sourceforge.net/projects/nikgapps/files/Canary-Releases/NikGapps-T/11-Jan-2023/NikGapps-core-arm64-13-20230111-signed.zip/download) using TWRP from [here](https://github.com/HemanthJabalpuri/twrp_motorola_rhode)
<!--
- Do below in TWRP to remove phh-su
  - Run below commands to make system r/w
    ```
    mount /system_root
    mount -o rw,remount /system_root
    ```
  - Remove below files
    ```
    /system_root/system/bin/phh-su
    /system_root/system/bin/su
    /system_root/system/etc/init/su.c
    /system_root/system/xbin/su
    ```
  - Flash Magisk or patched boot.img to root
  - Run below in Termux to securize
    ```
-->
</details>