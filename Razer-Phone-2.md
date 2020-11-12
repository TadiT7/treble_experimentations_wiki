Phone 2 by Razer

So here's the things that are not working for me:
* SIM Card/VoLTE (on Verizon... others may have more luck on different carriers)
* Bluetooth (moving or deleting BluetoothResCommon.apk from /vendor/overlay fixes Bluetooth immediately for audio (couldn't test phone calls since they don't work for me)
* Compass

### Unlock the bootloader
[Follow Razer's Instructions here](https://developer.razer.com/razer-phone-dev-tools/general-instructions/?_ga=2.262586380.1842452119.1605102124-783954625.1600236093?_ga=2.262586380.1842452119.1605102124-783954625.1600236093)

## Steps to Install (Windows)

* Step 1\
    Download [Phone 2 firmware Android Pie MR3 v3141](https://s3.amazonaws.com/cheryl-factory-images/aura-p-release-3141-user-full.zip)\
    Download [phusson's AOSP Android 11.0 v300.i](https://github.com/phhusson/treble_experimentations/releases/download/v300.i/system-roar-arm64-ab-floss.img.xz)
* Step 2:
Turn phone on in fastboot mode by holding volume down while powering on\
    Connect to computer
* Step 3:
Flash the entire phone to factory settings:
    ```
    flash_all.bat
    ```
    Then login into the phone and get all updates, reboot, get more updates etc.\
    Once complete, reboot the phone into fastboot again by holding volume down as the phone turns on\
    Go to recovery and run a factory reset
* Step 4: Erase the current slot's system partition
    ```
    fastboot erase system
    ```
* Step 5: Flash the GSI system partition
    ```
    fastboot flash system system-roar-arm64-ab-floss.img
    ```
* Step 6: Check which slot you're on by running
    ```
    fastboot getvar all
    ```
    and look for **(bootloader) current-slot** text it should have an '**a**' or a '**b**' as the slot.
* Step 7: Disable Android Verified Boot using the vbmeta.img from the Original Razer firmware posted above.  Replace the **@** symbol below with the proper letter for the slot you are on and run the command below to disable verified boot
    ```
    fastboot --disable-verity --disable-verification flash vbmeta_@ vbmeta.img
    ```
* Step 8: Cross your fingers, and tell the phone to reboot! It should boot into AOSP Android 11
    ```
    fastboot reboot
    ```

## Steps to Install (Linux)

* Step 1\
    Download [Phone 2 firmware Android Pie MR3 v3141](https://s3.amazonaws.com/cheryl-factory-images/aura-p-release-3141-user-full.zip)\
    Download [phusson's AOSP Android 11.0 v300.i](https://github.com/phhusson/treble_experimentations/releases/download/v300.i/system-roar-arm64-ab-floss.img.xz)
* Step 2:
Turn phone on in fastboot mode by holding volume down while powering on\
    Connect to computer
* Step 3:
Flash the entire phone to factory settings:
    ```
    sudo ./flash_all.sh
    ```
    Then login into the phone and get all updates, reboot, get more updates etc.\
    Once complete, reboot the phone into fastboot again by holding volume down as the phone turns on\
    Go to recovery and run a factory reset
* Step 4: Erase the current slot's system partition
    ```
    sudo fastboot erase system
    ```
* Step 5: Flash the GSI system partition
    ```
    sudo fastboot flash system system-roar-arm64-ab-floss.img
    ```
* Step 6: Check which slot you're on by running
    ```
    sudo fastboot getvar all
    ```
    and look for **(bootloader) current-slot** text it should have an '**a**' or a '**b**' as the slot.
* Step 7: Disable Android Verified Boot using the vbmeta.img from the Original Razer firmware posted above.  Replace the **@** symbol below with the proper letter for the slot you are on and run the command below to disable verified boot
    ```
    sudo fastboot --disable-verity --disable-verification flash vbmeta_@ vbmeta.img
    ```
* Step 8: Cross your fingers, and tell the phone to reboot! It should boot into AOSP Android 11
    ```
    sudo fastboot reboot
    ```
## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ✔️                                                     |
| Speaker / Mic             | ✔️                                                     |
| Bluetooth                 | ❌                                                     |
| WiFi                      | ✔️                                                      |
| SIM / Mobile Data / Voice | ❌ (tested on Verizon, YMMV)                             |
| VoLTE                     | ❌                                                     |
| Fingerprint               | ✔️                                                     |
| NFC                       | ✔️                                                     |
| Offline Charging          | ❌                                                     |
| GPS             | ✔️                                                     |
| Compass    |   ❌ 
---

Tested By: translucentfocus- Phone 2 (Global), Android Version: P-SMR5-RC002-RZR-200910.3195 - Date tested: 11/10/2020 - Template created by @zguithues and @hackintosh5