# Huawei Honor 10 Lite

Everything device-related works fine.

## Steps to install
Note 1: As an alternative of the following process, you can flash ROM via TWRP as "System Image" and format ART/Dalvik Cache, Cache, Data, and Internal Storage.

Note 2: Please note that the system partition size differs on different firmware versions (i.e. 1,33 GB on EMUI 9.**1**.x vs. 2,11 on EMUI 9.**0**.x). If you attempt to flash image, which size exceeds system partition's size, you'll get a "sparse flash write failure" error.

1. Download the right image for your device: it should have `arm64-ab-` in its name (`arm64_b` for some GSIs).
2. Make sure your bootloader is unlocked before proceeding; more info for doing that can be found on the [4PDA forum](https://4pda.to/forum/index.php?s=&showtopic=935415&view=findpost&p=104608410) (on Russian).
3. Also make sure that you have turned on OEM unlock in Developer options.
4. Reboot to Fastboot mode following these steps:
* Power off the phone completely.
* Press and hold the Volume Down button, and while doing that, connect your phone to the PC using the USB cable.
* Release the button when you see the Fastboot mode screen: a white colored screen with some text and the lying Android bot.
5. Make sure that both the bootloader and FRP are unlocked: you should see "PHONE Unlocked" and "FRP Unlock" captions under the Android bot.
6. Flash the image file with the `fastboot` utility and wait until the process is complete:
```
$ fastboot flash system system-(prefix)*-arm64-ab-vanilla.img
$ fastboot erase userdata
$ fastboot reboot
```
\* — `roar` for Android 11 GSIs, `squeak` for Android 12 GSIs

7. After that your phone will reboot. You should press and hold Volume Up during the "Your device has been unlocked and can't be trusted." screen to boot into eRecovery.
8. eRecovery will offer you data formatting; accept its offer, enter `yes` on the on-screen keyboard and tap on Format data.
9. After that tap on Reboot phone now.
10. Your phone will reboot again and show "android" splash screen after the bootloader unlock warning. You should see an installed ROM's launcher in a short time.
11. If you flashed a GSI image with GApps, just follow the steps of the Setup Wizard, and after that you should see an installed ROM's launcher.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK, both the rear and front cameras are working           |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | Not checked                                               |
| Fingerprint               | OK, but the scanner is a bit too sensitive                |
| NFC                       | Not checked                                               |
| Offline Charging          | OK                                                        |
---

## Tested

| User                 |      Device Model  |  Tested AOSP GSI version  |  Firmware  |  Date      |
|----------------------|--------------------|---------------------------|------------|------------|
| Neko-Monika          |      HRY-LX1(C10)  |                 11.0 v302 |  9.1.0.290 | 14.03.2021 |
