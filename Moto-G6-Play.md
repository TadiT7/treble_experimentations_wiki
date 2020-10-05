# Moto G6 Play

Any GSI that is ARM A-Only should boot, but full compatibility isn't guaranteed  

***If you are flashing an Android 10 GSI:*** make sure you don't have Magisk installed, as it will cause bootloops  

**Note:** Boot animations don't work on some models. While booting, it might only show the bootloader logo ("bad key" or "N/A" screen)  
Be patient, the first boot will take a while

## Steps to install

* Decryption is not required, but it's recommended
* Follow this guide for up-to-date instructions: [[guide] [root] [oreo&pie] [jeter/aljeter] [twrp, decrypt, magisk] [stock firmware]](https://forum.xda-developers.com/g6-play/how-to/guide-t3929928)
* If your phone is running Pie, you will need to use TWRP built for the **16GB** model, even if you have the 32GB model
* This thread contains a list of tested GSI ROMs: [ROMs that run on the G6 Play [GSI]](https://forum.xda-developers.com/g6-play/development/roms-run-g6-play-gsi-t3904067)
* Flash the image with the `fastboot` utility:
    ```
    $ fastboot flash system system-arm-aonly.img
    ```
* As an alternative you can flash via TWRP as **System Image**

## Hardware Support (Pie)

| Component                 |      Comment                                                    |
|---------------------------|-----------------------------------------------------------------|
| Camera                    | Works                                                           |
| Speaker / Mic             | Works                                                           |
| Bluetooth                 | Has issues with audio                                           |
| WiFi                      | Works                                                           |
| SIM / Mobile Data / Voice | Works (Tested with Boost Mobile, APNs may need to be added manually)|
| VoLTE                     | Untested                                                        |
| Fingerprint               | Works                                                           |
| Offline Charging          | Works                                                           |

## Hardware Support (10/Q)

| Component                 |      Comment                                                    |
|---------------------------|-----------------------------------------------------------------|
| Camera                    | Works                                                           |
| Speaker / Mic             | Works                                                           |
| Bluetooth                 | Has issues with audio                                           |
| WiFi                      | Works                                                           |
| SIM / Mobile Data / Voice | Works (Tested with Boost Mobile, APNs may need to be added manually)|
| VoLTE                     | Untested                                                        |
| Fingerprint               | Works                                                           |
| Offline Charging          | Works                                                           |

## Hardware Support (11/R)

| Component                 |      Comment                                                    |
|---------------------------|-----------------------------------------------------------------|
| Camera                    | Works (Video recording only with third-party camera applications)|
| Speaker / Mic             | Works                                                           |
| Bluetooth                 | Works                                                           |
| Audio of Notifications    | Not Works                                                       |
| WiFi                      | Works                                                           |
| SIM / Mobile Data / Voice | Works                                                           |
| VoLTE                     | Untested                                                        |
| Fingerprint               | Works                                                           |
| Offline Charging          | Works                                                           |
| GPS                       | Works                                                           |
| Sensors                   | Works                                                           |
| Lantern                   | Works                                                           |

## Stock ROMs

Motorola stock ROMs are available [here for aljeter](https://mirrors.lolinet.com/firmware/moto/aljeter/official/), and [here for jeter](https://mirrors.lolinet.com/firmware/moto/jeter/official/). Make sure you use the correct ROM for your model, otherwise you may run into weird issues.

---

Pie: tested by @ry755 - XT1922-7 (jeter, US), Pie vendor, tested on 10/9/2019 with AOSP v119  
10/Q: tested by @ry755 - XT1922-7 (jeter, US), Pie vendor, tested on 12/2/2019 with AOSP v204  
11/R: tested by @ruben8ap - XT1922-2 (aljeter, EU), Oreo vendor, tested on 05/10/2020 with AOSP v300.f  

Using a wiki template created by @zguithues and @hackintosh5