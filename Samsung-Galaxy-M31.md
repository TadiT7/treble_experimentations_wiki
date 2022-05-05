# Samsung Galaxy M31 (SM-M315F)
Summary of what works and doesn't.
# Installation guide
* Fastboot installation is untested since I'm having issues with Yillie's TWRP.
### Flashing guide using Fastboot.
Enable USB debugging. Reboot your device into Fastbootd if your recovery supports it:
  ```
  $ adb reboot bootloader
  $ fastboot reboot fastboot
  ```
or:
  ```
  $ adb reboot fastboot
  ```
Now flash the GSI image you downloaded:
  ```
  $ fastboot flash system /path/to/file.img
  ```
If you're on Linux or macOS, use `sudo fastboot`.
### Flashing guide using TWRP
If you're on Android 11, download TWRP using [this link](https://github.com/soulr344/android_device_samsung_m31). If you're on Android 12, use the TWRP provided by [this Telegram group](https://t.me/galaxym31development). **You will need to flash a nulled vbmeta before flashing the Android 12 TWRP!**
* Enter TWRP recovery.
* Do a clean flash if you're not upgrading a GSI version. To do that: `Wipe > Dalvik/ART Cache, Data, Cache`. If you have already installed a GSI, you don't need to wipe Data (unless it's an Android update).
* Start installing: `Install > Install Image > nameofthegsi.img > System Image > Swipe to confirm Flash`.
* Enjoy!
# Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working  (No Pixel Binning)                               |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working, 5 & 2.4 GHz                                      |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not Working (a common issue among Samsung devices)        |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| USB headset               | Not Working (from my experience)                          |
---
# Bluetooth issues
If your headset isn't recognized or not working, change these settings from **PHH settings**:
* Misc features > Force-disable A2DP hardware offload: On
* Misc features > Use alternate way to detect headsets: On
If your system crashes when using Bluetooth, please turn off media recommendations. 

**Note**: The camera quality and access to sensors depend on what camera app you're using and whether you enabled Camera2 HAL3 API.

Tested By: vitalitk - SM-M315F(SEK) - M315FXXU2BUH8 - 5/5/2022