# Huawei Honor 9 Lite

Everything device-related works fine.

## Steps to install
Note: As an alternative of the following process, you can flash via TWRP as "System Image" and format data.

1. Download the right image for your device: aonly- if you are on EMUI 8.x, ab- if you have updated to EMUI 9.x.
2. Make sure your bootloader is unlocked before proceeding. More info for doing that can be found on the [XDA forum](https://forum.xda-developers.com/f/honor-9-lite-guides-news-discussion.7288/).
3. Reboot to fastboot mode following these steps:
* Power off the phone completely.
* Press and hold the Volume Down button, and while doing that, connect your phone to the PC using the USB cable.
* Release the button when you see the fastboot screen: a white colored screen with some text and the Android bot.
4. Make sure that both the bootloader and FRP are unlocked. If not, you should not proceed with the next step.
5. Flash the image file with the `fastboot` utility and wait until the process is complete:
    ```
    $ fastboot -w
    $ fastboot flash system system-arm64-type-type-type.img
    ```
   The device might bootloop a couple of times, this is OK. It might also tell you that the data partition has to be low level formatted. Click on OK and after that the device will boot just fine!

6. If the device did not reboot automatically, reboot using the following command and then unplug your phone:
   ```
    $ fastboot reboot
   ```
7. Enjoy your new ROM!

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                        |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| WiFi                      | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| Hotspot                   | OK                                                        |
| VoLTE                     | Broken, of course                                         |
| Fingerprint               | OK                                                        |
| NFC                       | OK                                                        |
| Offline Charging          | OK                                                        |
---

## Tested

| User                 |      Device Model  |  Firmware  |  Date      |
|----------------------|--------------------|------------|------------|
| tetris4              |      LLD-L31C432   |  9.1.0.168 | 29/12/2020 |
| hackintosh5          |      LLD-L31C432   |  8.0.0.132 | 27/01/2019 |
| kaiomatico           |      LLD-L31C432   |  8.0.0.128 | 05/03/2018 |



Template created by @zguithues