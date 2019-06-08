# Moto G6 Play

## Steps to install

Decryption is not required, but it's recommended.  
* Follow this guide for up-to-date instructions: [[guide] [root] [oreo&pie] [jeter/aljeter] [twrp, decrypt, magisk] [stock firmware]](https://forum.xda-developers.com/g6-play/how-to/guide-t3929928)
* Even if you have the 32GB model, you need to use the TWRP built for the **16GB** model
* This thread contains a list of tested GSI ROMs: [ROMs that run on the G6 Play [GSI]](https://forum.xda-developers.com/g6-play/development/roms-run-g6-play-gsi-t3904067)
* (Any GSI that is ARM A-Only should boot, but hardware compatibility isn't guaranteed)
* Flash the image with the `fastboot` utility:
    ```
    $ fastboot flash system system-arm-aonly.img
    ```

    As an alternative you can flash via TWRP as "System Image"

## Hardware support

| Component                 |      Comment                                                    |
|---------------------------|-----------------------------------------------------------------|
| Camera                    | Works                                                           |
| Speaker / Mic             | Works                                                           |
| Bluetooth                 | Works                                                           |
| WiFi                      | Works                                                           |
| SIM / Mobile Data / Voice | Works (Tested with Boost Mobile, APNs need to be added manually)|
| VoLTE                     | Untested                                                        |
| Fingerprint               | Works                                                           |
| Offline Charging          | Untested                                                        |
---

Tested by @ry755 - XT1922-7 (Jeter, Boost Mobile, US), Pie vendor firmware - Tested on 6/8/19

Using a wiki template created by @zguithues and @hackintosh5