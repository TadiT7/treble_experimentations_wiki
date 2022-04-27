# S22 (Snapdragon)

## Steps to install

* Unlock Bootloader (Enable OEM Unlocking, power-off, hold Vol+&- while plugging in to PC)
* Patch and Flash recovery with fastbootd (you can patch recovery with https://github.com/Johx22/Patch-Recovery)
* Boot into recovery and enable fastbootd
* Flash arm64 GSI with fastboot (fastboot flash system image.img)
* Go back into recovery and Wipe Data and Cache
* Reboot!

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works (Front and Back) - Haven't tested other back cams   |
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Works (Haven't tested audio)                              |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Unknown                                                   |
| Fingerprint               | Broken (PHH has apparently gotten it to work)             |
| NFC                       | Works (Used 2FA key)                                      |
| Offline Charging          | Unknown                                                   |
---

Tested By: https://github.com/kuugan - SM-901E, PHH v412 - Tested on 28/04/2022 - Template created by @zguithues and @hackintosh5