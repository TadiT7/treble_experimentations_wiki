# F(x)tec Pro1

Pretty much everything works. Keybord lacks backlight (except for capslock state), the special yellow arrow buttons do nothing, their role is replaced by shift.

## Steps to install

* Download the latest platform tools from https://developer.android.com/studio/releases/platform-tools and unpack them
* Download a GSI of your choice and (if present) unpack the xz file, for example through 7zip
* Download the vbmeta from https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img
* Go into the unpacked platform tools, open terminal there and flash vbmeta using `fastboot flash vbmeta vbmeta.img`. No extra parameters required.
* Flash the system image using `fastboot flash system yourgsifilename.img`
* Format and wipe userdata using `fastboot format userdata` and `fastboot erase userdata` commands
* Reboot the device

## Hardware support on Q

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works, but the stock camera app refuses to run, install any other|
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Works, tested only pairing and file sharing               |
| WiFi                      | Works, along with hotspot                                 |
| SIM / Mobile Data / Voice | Didn't test                                               |
| VoLTE                     | Didn't test                                               |
| Fingerprint               | Works                                                     |
| NFC                       | Didn't test                                               |
| Offline Charging          | Stuck on boot logo (needs to be enabled through fastboot first by `fastboot oem off-mode-charge 1` and `fastboot oem enable-charger-screen` commands)|
| Other feature             | Keyboard backlight is dead, special yellow arrow keys do nothing|
---

Tested By: @TadiT7 - QX1000 EEA, AOSP 10.0 v206 on `QX1000_user_20191203104306_7ec9dab` - 15.12.2019