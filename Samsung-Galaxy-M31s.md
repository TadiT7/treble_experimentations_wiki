# Samsung Galaxy M31s (SM-M317F/DS)

Telegram Support Group: https://t.me/samsungm31sup

Safetynet does not pass out of the box. Use Universal SafetyNet fix module by kdragon, with magisk denylist to hide sensitive apps

## Steps to install

* Fastboot installation via custom recovery has been tested, and working
    ```
    $ fastboot flash system <system.img>
    ```

* Flashing in TWRP as "System Image", then wiping data & cache also works (recommended)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works(but with no pixel binning)                          |
| Speaker / Mic             | Works(Volume Level not working, see Workarounds)          |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Not Working                                               |
| VoWiFi                    | Not Working.                                              |
| Fingerprint               | Works on PHH AOSP v413                                    |
| Offline Charging          | Maybe                                                     |
| Wi-Fi Hotspot             | Doesn't work on One UI 4 firmware (See Workarounds)       |                                                 
---

## Workarounds:
### Hotspot
1) Reboot to Recovery
2) Backup BOOT & DTBO
3) Flash [this kernel](https://t.me/physwizz2/544)
4) Reboot to system (hotspot won't work yet)
5) Again, reboot to recovery and restore your stock BOOT and DTBO that you backed up
6) Now hotspot will work

### Volume Level
1) Open settings app
2) Navigate to PHH Treble Settings>Samsung Features
3) Disable 'Use alternate audio policy'
4) Reboot and volume level will become normal again, but BT Calls won't work

Tested By: khushtaur3123 - rufus582 - SM-M317F(INS), Bootloader/Radio - M317FXXU3DVF3 and SM-M317F(INS), Bootloader/Radio - M317FXXU3CVC2
Updated Date: 27 July 2022

