# Nokia 8 (TA-1004)

## Important note

First things first: this device does not support Project Treble out of the box. You need to _infect_ your device with [T-Virus](https://github.com/resident-nokia/t-virus). That custom ROM comes with TWRP.

## Steps to install

* IMPORTANT: Make sure you have an unlock.key in order to unlock your bootloader, nowadays HMD servers got down for getting this key.
* Step 1: Flash the T-Virus image (.qlz, use NOST). You must unlock your bootloader first providing your unlock.key.
* Step 2: At this point you can flash in either A or B slot a GSI. Best way is using the built-in TWRP in the image.

More info in Nokia 8 XDA Forums:

* https://forum.xda-developers.com/nokia-8/development/t-virus-infect-nokia-8-project-treble-t3946249
* https://forum.xda-developers.com/nokia-8/how-to/unofficial-official-nokia-8-bootloader-t3898418

## Hardware support (AOSP 9)

| Component                 |      Comment                                             |
|---------------------------|----------------------------------------------------------|
| Camera                    | They work, you need to enable them.                      |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works, not fully tested                                  |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Not fully tested                                         |
| Fingerprint               | Works                                                    |
| NFC                       | Not fully tested                                         |
| Others                    | Vibration on haptic buttons is not working               |
---


## Hardware support (AOSP 10)

| Component                 |      Comment                                             |
|---------------------------|----------------------------------------------------------|
| Camera                    | They work, you need to enable them.                      |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works, not fully tested                                  |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works                                                    |
| VoLTE                     | Not fully tested                                         |
| Fingerprint               | Doesn't work                                             |
| NFC                       | Not fully tested                                         |
| Others                    | Haptic buttons are not working. Lights do.               |
---

Tested By: 

- Suzamax (AOSP 9, AOSP 10) - Nokia 8 TA-1004 (Europe) NB1-0-488B-00WW - May 1 2020

Template created by @zguithues and @hackintosh5
