Razer Phone 2 generally works fine with this Android 11.0.

Things that may (not) be working:
* SIM Card/VoLTE (on certain carries such as Verizon)
* Bluetooth (moving or deleting BluetoothResCommon.apk from /vendor/overlay fixes it)
* Compass

## Steps to Install (Windows & Linux)
* **Step 1:** Unlock bootloader\
[Follow Razer's instructions](https://developer.razer.com/razer-phone-dev-tools/general-instructions/?_ga=2.262586380.1842452119.1605102124-783954625.1600236093?_ga=2.262586380.1842452119.1605102124-783954625.1600236093)<br/>

* **Step 2:** Download firmwares\
 [Phone 2 Stock Firmware](https://s3.amazonaws.com/cheryl-factory-images/aura-p-release-3141-user-full.zip) and
 [phhusson's AOSP Android 11.0 v300.i](https://github.com/phhusson/treble_experimentations/releases/download/v300.i/system-roar-arm64-ab-floss.img.xz)<br/>

* **Step 3:** Enter fastboot\
    Hold down volume button while powering on\
    Connect to computer via USB<br/>

* **Step 4:** Flash phone to factory settings\
 Windows: `flash_all.bat`\
 Linux: `sudo ./flash_all.sh`\
 Once complete, reboot the phone into fastboot again by holding volume down as the phone turns on.\
 For the following commands, remove `sudo` if you are using Windows.


* **Step 5:** Erase active system partition
```
sudo fastboot erase system
```
<br/>


* **Step 6:** Flash GSI on system partition
```
sudo fastboot flash system system-roar-arm64-ab-floss.img
```
<br/>


* **Step 7:** Check active slot you're running on
```
sudo fastboot getvar all
```

Look for `(bootloader) current-slot` text, it should have an '**a**' or a '**b**' as the slot.<br/><br/>

* **Step 8:** Disable Android Verified Boot using the vbmeta.img from the Original Razer firmware posted above. Replace the **@** symbol below with the proper letter for the slot you are on and run the command below to disable verified boot
```
sudo fastboot --disable-verity --disable-verification flash vbmeta_@ vbmeta.img
```
<br/>

* **Step 9:** Cross your fingers, and tell the phone to reboot! It should boot into AOSP Android 11. It may take some time for its maiden boot though.
```
sudo fastboot reboot
```

## Hardware Support
| Component                 | Status |      Comment                                         |
|---------------------------|--------|------------------------------------------------------|
| Camera                    | ✔️     |                                                      |
| Speaker / Mic             | ✔️     |                                                      |
| Bluetooth                 | ⚠️     | Remove /vendor/overlayBluetoothResCommon.apk to make it work |
| WiFi                      | ✔️     |                                                      |
| SIM / Mobile Data / Voice | ⚠️     | ✔️ SmarTone; ❌ Verizon                             |
| VoLTE                     | ⚠️     |                                                      |
| Fingerprint               | ✔️     |                                                      |
| NFC                       | ✔️     |                                                      |
| Offline Charging          | ❌     |                                                      |
| GPS                       | ✔️     |                                                      |
| Compass                   | ⚠️     | Might (not) work on some Phone 2's                   |
---

Tested By:
* translucentfocus - Phone 2 (Global), Android Version: P-SMR5-RC002-RZR-200910.3195 - Date tested: 11/10/2020
* haruki-taka8 - Phone 2 (Global), Android Version: P-SMR6-RC001-RZR-201022 - Date tested: 10/3/2021

Template created by @zguithues and @hackintosh5