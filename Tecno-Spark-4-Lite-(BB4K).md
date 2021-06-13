# Device
Tecno Spark 4 Lite (BB4K)

***
Will work on most MediaTek Devices

## Steps to install

## Initial Steps:
* Download ADB and Fastboot from link below:
* https://developer.android.com/studio/releases/platform-tools
* Connect your mobile to Laptop/PC.
* Open CMD in ADB and Fastboot folder.
* Type `adb devices`
* Then `adb reboot bootloader`
* Next `fastboot flashing unlock` (This will erase all data).
* Lastly `fastboot reboot`

##Installing GSI
* Download GSI of your choice.
* Download Vbmeta File from link below: 
* https://drive.google.com/file/d/1ifnXCIdkqKnk_a1HII9RqQd5CVFWz1xR/view
* Place both in ADB and Fastboot folder.
* Perform a factory reset.
* Now 
*        $:adb reboot bootloader
*        $:fastboot flash vbmeta Name_of_Vbmeta_file.img
*        $:fastboot flash system Name_of_GSI_image.img
*        $:fastboot -w 
*        $:fastboot reboot
       
     Some more info

    As an alternative you can download [TWRP](https://androidfilehost.com/?fid=8889791610682912002) and flash image as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (Front and Back)                                                    |
| Speaker / Mic             |  Working                                                  |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Broken                                                 |
| Fingerprint               | Working                                                    |
| NFC                       | ------                                                   |
| Offline Charging          | Broken                                                   |
| Other feature             | Adaptive brightness is broken (Every thing else is working)                                                    |
---

* Tested By: Shahrukh Abrar
* Model-Number:Tecno Spark 4 Lite (BB4K)
* Region:Pakistan
* Firmware Version:BB4K-H6114UVW-PGO-200212V76
* Date tested:30/7/2020