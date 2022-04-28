# S22 (Exynos)

## Steps to install

* Unlock Bootloader (Enable OEM Unlocking, power-off, hold Vol+&- while plugging in to PC)
* Patch and Flash recovery with fastbootd (you can patch recovery with https://github.com/Johx22/Patch-Recovery)
*     1) To flash the patched recovery, download Heimdall (https://glassechidna.com.au/heimdall/) extract it and put the patched recovery.img into the same directory as the heimdall.exe (or the Linux equivalent)
*     2) Follow the README file, specifically the "Driver Installation Instructions", in my case I had to replace the SAMSUNG USB device's with the WinUSB one (make sure it's NOT the "modem" one)
*     3) After that, try executing the following command within the root of Heimdall's directory: .\heimdall flash --RECOVERY r.img (".\" part was needed for me on Windows)
*      Make sure to hold the power button and Volume Up as soon as the phone starts rebooting as the patched recovery will be overwritten by the Samsung one as soon as one boots into OneUI
* Boot into recovery and enable fastbootd
* Flash arm64 GSI with fastboot (fastboot flash system image.img)
* Go back into recovery and Wipe Data and Cache
* Reboot!

## Hardware support

| Component                 |      Comment                                                      |
|---------------------------|-------------------------------------------------------------------|
| Camera                    | Works (Front and Back) - Haven't tested other back cams           |
| Speaker / Mic             | Works                                                             |
| Bluetooth                 | Works (Haven't tested audio)                                      |
| WiFi                      | Works                                                             |
| SIM / Mobile Data / Voice | Works                                                             |
| VoLTE                     | Unknown                                                           |
| Fingerprint               | broken (but works in PE Plus, Phhusson apparently fixed it )      |
| NFC                       | Works (Used 2FA key)                                              |
| Offline Charging          | Unknown                                                           |
| 120Hz                     | Broken, 60Hz is the highest, and 10Hz is the lowest**               |
---
**You can enforce 120Hz via ADB:
adb shell
settings put system peak_refresh_rate 120
settings put system min_refresh_rate 120

Tested By: https://github.com/JeikWazTaken - SM-901B, PE Plus GSI 2022-04-12 build - Tested on 28/04/2022 - Template created by @zguithues and @hackintosh5

