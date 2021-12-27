Seems to work pretty well except problems with radio fm and sim detection.

## Steps to install
**THIS WILL ERASE ALL YOUR DATA**

### Setup
- Install and store all of these on your phone's internal storage or sd card
  - terble-supported android rom version below gsi; _ex:_ if gsi version is 12, android version should be 11 ([LineageOS](https://download.lineageos.org/payton) recommended)
  - GSI rom
  - [TWRP](https://dl.twrp.me/payton/) recovery; install latest .img file; keep a copy on computer
- Unlock [bootloader](https://motorola-global-portal.custhelp.com/app/standalone/bootloader/unlock-your-device-a)
- Enable USB debugging in developer settings
- Boot into fastboot using `adb reboot fastboot`
  - [Adb & fastboot](https://developer.android.com/studio#downloads); install latest command-line tools for your system
  - [Moto X4 USB drivers](https://motorola-global-portal.custhelp.com/app/answers/prod_answer_detail/a_id/78248)
- Boot into twrp using `fastboot boot <path to twrp.img>`

### Installing GSI
- Installing base rom
  - After entering twrp select wipe > advanced wipe
  - Next select all the partitions (don't wipe internal storage if the rom is install on it) and swipe to wipe
  - Return home and select install
  - Find your Android rom and install it
  - Return home and select advanced
  - Select install recovery ramdisk then find the twrp.img and install it
  - Return home and select reboot
  - Select the opposite slot; _ex:_ if you're in slot a switch to slot b
  - Reboot to recovery
- Installing GSI rom
  - Select install
  - Select install img and find the gsi.img and install it
  - Reboot to system

## Hardware support

| Component                 | Status |
|---------------------------|--------|
| Camera                    | √ |
| Speaker / Mic             | √ |
| Bluetooth                 | √ |
| WiFi                      | √ |
| SIM / Mobile Data / Voice | X |
| VoLTE                     | ? |
| Fingerprint               | √ |
| NFC                       | ? |
| Offline Charging          | ? |
---

@RFX-LEGEND - v400.e - 2021/12/26