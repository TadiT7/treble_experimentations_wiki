# realme C3/Narzo 10A
## Requirement :
Since TWRP/PBRP is available but we cant install GSI using custom recovery due to dynamic partitions
* Unlock bootloader
* Make sure you use ADB Fastboot that support fastbootd (Like latest Google SDK Platform Tools in [here](https://developer.android.com/studio/releases/platform-tools))
* Download any Phh based GSI (A/B arm64 image)
* Download vbmeta and boot from here : https://t.me/RealmeC310a then type #boot and #vbmeta
* Make sure the boot.img that you downloaded is same with your current firmware version

## Steps to install :
* Extract and copy all GSI Image, vbmeta, and boot to ADB Fastboot folder
* Boot to system and make sure USB Debugging is active on your device
* Open ADB Fastboot and type:    ```adb reboot fastboot    ```
* Wait till the device boot to recovery (Yes, recovery, not fastboot. Because realme UI using Dynamic Partition and realme UI supporting fastbootd on it's recovery.) If you doubt, you can check on Device Manager and check your device already detected as Bootloader Interface or not. If already detected as Bootloader Interface, you can go on.
* Then type :    ```fastboot flash system gsiimagename.img    ```
* If done, type :    ```fastboot reboot bootloader    ```
* After reboot to bootloader, type :    ```fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img && fastboot flash boot boot.img    ```
* Final touch, type :    ```fastboot -w``` or Stock recovery to format the data
* Then    ```fastboot reboot``` to start booting to the system




## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Back Camera               | Working                                                   |
| Front facing Camera       | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working                                                   |
| Fingerprint Sensor        | Not Working                                               |
| Offline Charging          | Working                                                   |
| Tethering                 | Working                                                   |
| Hotspot                   | Working                                                   |
| Auto-Brightness           | Working (But have lower brightness issue)                 |
---

Tested By: [me](https://t.me/sarthakroy2002) and my tester - RMX2020 Firmware version RMX2020_11.A.59 - Date tested April 15, 2021.

Tested By: [@rjaakash](https://t.me/rjaakash) - RMX2020 Firmware version RMX2020_11.A.61 - Date tested May 23, 2021.

Template created by @zguithues and @hackintosh5