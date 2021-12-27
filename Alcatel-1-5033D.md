Works exceptionally well with v32 gsi.

## Steps to install
**THIS WILL ERASE ALL YOUR DATA**

### Setup
- Install
  - GSI rom ([v32](https://github.com/phhusson/treble_experimentations/releases/tag/v32) highly recommended)
- Unlock [bootloader](https://motorola-global-portal.custhelp.com/app/standalone/bootloader/unlock-your-device-a)
- Enable oem unlocking & USB debugging in developer settings
- Boot into fastboot using `adb reboot fastboot`
  - [Adb & fastboot](https://developer.android.com/studio#downloads); install latest command-line tools for your system
  - [Alcatel 1 USB drivers](https://www.alcatelmobile.com/support/software-drivers/)

### Installing GSI
- Flash system image using `fastboot flash system <path to gsi.img>`

## Hardware support

| Component                 | Status |
|---------------------------|--------|
| Camera                    | √ |
| Speaker / Mic             | √ |
| Bluetooth                 | √ |
| WiFi                      | √ |
| SIM / Mobile Data / Voice | ? |
---

@RFX-LEGEND - v32 - 2021/12/26