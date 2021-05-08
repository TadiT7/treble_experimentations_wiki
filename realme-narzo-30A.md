# realme narzo 30A
## Requirement :
Since TWRP is not available yet for narzo 30A, full install method were using fastboot
* Unlock bootloader (Use realme 6 In-depth Test and make sure you are in A13 or A15 firmware)
* Make sure you use ADB Fastboot that support fastbootd (Like latest Google SDK Platform Tools in [here](https://developer.android.com/studio/releases/platform-tools))
* Download any Phh based GSI (A/B arm64 image)
* Download vbmeta and boot from here : https://t.me/RealmeNarzo30AIndonesia then type #boot and #vbmeta
* Make sure the boot.img that you downloaded is same with your current firmware version

## Steps to install :
* Extract and copy all GSI Image, vbmeta, and boot to ADB Fastboot folder
* Boot to system and make sure USB Debugging is active on your narzo 30A
* Open ADB Fastboot and type :    ```adb reboot fastboot    ```
* Wait till the device boot to recovery (Yes, recovery, not fastboot. Because realme UI using Dynamic Partition and realme UI supporting fastbootd on it's recovery.) If you doubt, you can check on Device Manager and check your device already detected as Bootloader Interface or not. If already detected as Bootloader Interface, you can go on.
* Then type :    ```fastboot flash system gsiimagename.img    ```
* If done, type :    ```fastboot reboot bootloader    ```
* After reboot to bootloader, type :    ```fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img && fastboot flash boot boot.img    ```
* Final touch, type :    ```fastboot -w``` to format the data
* Then    ```fastboot reboot``` to start booting to the system




## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Back Camera               | Working                                                   |
| Front facing Camera       | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working (Audio not tested)                                |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not tested                                                |
| Fingerprint Sensor        | Not Working                                               |
| Offline Charging          | Working                                                   |
| Tethering                 | Working                                                   |
| Hotspot                   | Working                                                   |
| Auto-Brightness           | Working (But have lower brightness issue)                 |
---

Tested By: Kamildotmus / whitefox9000 - [Pixel Experience 11 v306 by ponces](https://github.com/ponces/treble_build_pe/releases/tag/v306) - RMX3171 (ID) Firmware version RMX3171_11.A.15 - Date tested May 8, 2021.

Template created by @zguithues and @hackintosh5