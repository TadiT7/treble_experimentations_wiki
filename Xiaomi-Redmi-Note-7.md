# Redmi Note 7 (lavender)
The device works with phh-treble almost perfectly. Some issues that are currently seen include:
1. Brightness flickering
2. Adaptive brightness doesn't work
3. Proximity sensor has some issues if you enable->disable the adaptive brightness (to fix it, just enable->disable adaptive brightness again)

NOTE: Fingerprint sensor will now not work if you disable forceencrypt - [Issue #409](https://github.com/phhusson/treble_experimentations/issues/409)

## Steps to Install
### Step 1: Unlocking the Bootloader
- Unlock the bootloader using Xiaomi's own [Mi Unlock](https://en.miui.com/unlock/download_en.html), which is only on Windows or you can use Franesco Tescari's [MiUnlockTool](xiaomitool.com/MiUnlockTool) which is available on Linux, MacOS and Windows. 
- Once the bootloader is unlocked, you will see the text "Unlocked", with a unlock symbol, on the bottom of your boot screen. 

### Step 2: Enable Debugging Permissions
- Enable USB debugging on your device and make sure ADB is authorized and the reboot to fastboot mode and validate that fastboot can access your device by executing:
```
$ adb devices
$ adb reboot bootloader # Alternative: hold the power and vol-down button
$ fastboot devices
```

### Step 3: Factory Reset
- Run the following command on fastboot to factory reset your device
```
$ fastboot -w
```

### Step 4: Flash TWRP
- Download the latest version of the unofficial TWRP from XDA (The link to the TWRP I tested is located below)
- Flash TWRP with fastboot
```
$ fastboot flash recovery recovery.img
```

### Step 5: Install phh-treble AOSP 9.0
- Download the latest version of phh-treble AOSP 9.0 from [here](https://github.com/phhusson/treble_experimentations/releases)
- Extract the *.xz file to retrieve your system.img (naming scheme will be different)
- If you're flashing with fastboot, run the following command:
```
# Replace the system-*.img with whatever image you have downloaded
$ fastboot flash system system-*.img
```

- If you're flashing with TWRP, load the system-*.img to your internal storage using ADB push or similar
```
$ adb push system-*.img /sdcard/TWRP/system-*.img
```
- Perform a factory reset and then perform the following sequence of steps: _Install > Install Image > Navigate to TWRP > Select "system-*.img"_

### Step 6: Install Magisk
- Download Magisk from the XDA forums (v19.0 worked for me)
- Load the Magisk-*.zip to your internal storage using ADB push or similar:
```
$ adb push Magisk-*.zip /sdcard/TWRP/Magisk-*.zip
```

- Install Magisk-*.zip using TWRP by following the sequence of steps: _Install > Navigate to TWRP > Select Magisk zip_

### Step 7: Install GAPPS
- Install GAPPS in the same way as Step 6, if you haven't selected the gapps package

### Step 8: Reboot to System
- Wait for the device encryption to complete on the first boot. If you don't want to enable force encryption, you can disable it before this first boot by flashing a zip in TWRP (you should find it on Google)
- The device will reboot and initate the first-boot process. Let it complete and you should be entering the Setup Wizard

### Step 9: Additional Fixes
- You will need to fix the brightness flickering bug by executing the following command through adb shell (however, it's not guaranteed that it will fix the issue - it didn't for me):
```
adb shell
su
setprop persist.sys.qcom-brightness 4095
```
- To get SafetyNet to pass on this you will need to enable late_service_start for Magisk. Find the link below.

#### Helpful Links:
- XDA All-in-One - https://forum.xda-developers.com/redmi-note-7/how-to/one-redmi-note-7-unlock-bootloader-t3890751
- SafetyNet Workaround - https://github.com/phhusson/treble_experimentations/issues/116

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Status: Working                                           |
| Speaker / Mic             | Status: Working                                           |
| Bluetooth                 | Status: Working                                           |
| WiFi                      | Status: Working                                           |
| SIM / Mobile Data / Voice | Status: Working                                           |
| VoLTE                     | Status: *Untested*                                        |
| Fingerprint               | Status: Working                                           |
| Offline Charging          | Status: *Untested*                                        |
| Adaptive Brightness       | Status: **Not Working**                                   |

Please add other features, if I have missed anything.

---

Tested By:
1. Username: **@satadi**
   - Model: Redmi Note 7 (lavender)
   - Region: India
   - MIUI Vendor: MIUI India Stable 10.2.11

Template created by @zguithues and @hackintosh5