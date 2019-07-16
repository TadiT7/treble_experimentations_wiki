# Xiaomi Mi 9 SE

Although this device is A-only, you have to choose GSI for A/B devices because this device is "system-as-root".

Tested with LineageOS GSI from AndyYan (build 20190609)

## Steps to install
- Unlock bootloader
- Boot in Fastboot mode
- Flash TWRP
`fastboot flash recovery twrp-3.3.1-2-grus-20190609.img`
- Right after flashing press VOLUME UP + POWER to reboot in recovery
- In TWRP Swipe to allow modifications
- In TWRP reboot to bootloader
- Flash vbmeta to disable verified boot
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
- Reboot to TWRP
- Tap on advanced Wipe menu and wipe cache, dalvik, data and system (and optionally internal storage)
- Reboot to TWRP
- Copy GSI ROM and Gapps to phone
- Tap on Install > Install Image > select image, and flash it to system
- Reboot to TWRP
- Install GAPPS
If the installer gives error 70 go to Wipe > Advanced wipe > Select system > Repair > Resize filesystem
Then Flash again GAPPS
- Factory reset
- Reboot to System

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works, only front and middle back cameras available                                  |
| Speaker / Mic             | Works                                                   |
| Bluetooth                 | Works                                                    |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice |    Works, LTE+ works. Some GSI force 3G only, type \*#\*#4636#\*#\* and set LTE If that doesn't work use primary slot instead of secondary                                                 |
| VoLTE                     | Not tested                                                    |
| Fingerprint               | Works, broken on Always on Display (turn screen on first)                                                    |
| NFC                       | Not tested                                                    |
| Offline Charging          | Broken, the screen flashes light blue instead of showing charge animation                   |
---

Tested By: 
- @Nimayer - Mi 9 SE 128GB - 01/07/2019