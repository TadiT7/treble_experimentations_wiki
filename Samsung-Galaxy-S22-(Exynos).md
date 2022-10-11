# S22 (Exynos)

## Steps to install

* Unlock Bootloader (Enable OEM Unlocking in Developer Options, power the phone off, hold Vol+&- while plugging in to your PC)
* Download the latest firmware for your device (You can use e.g. Samfirm - google it)
* Extract the archive, open up the super archive via 7Zip Z-Standard (NOT THE REGULAR 7-Zip), extract the recovery archive and then extract that one to get your own recovery.img
* Patch your recovery image (you can patch it with **[Johnx22's Patch-Recovery Tool](https://github.com/Johx22/Patch-Recovery)**

* To flash the patched recovery, download **[Heimdall](https://glassechidna.com.au/heimdall/)**
* Extract it and put the patched recovery.img into the same directory as the heimdall.exe (or the Linux equivalent)
* Follow the README file, specifically the "Driver Installation Instructions" , in my case I had to replace the SAMSUNG USB device's with the WinUSB one (make sure it's NOT the "modem" one)
*  After that, try executing the following command within the root of Heimdall's directory: 
     `heimdall flash --RECOVERY <whatever your patched image is named>.img` 
                  
* Make sure to hold the power button and Volume Up as soon as the phone starts rebooting, otherwise the patched recovery will be overwritten by the Samsung one as soon as one boots into OneUI
* After entering recovery, choose "Enter fastboot"
* Flash an ARM64 A/B GSI with fastboot:    `fastboot flash system image.img`
* Go back into recovery and Wipe Data and Cache
* Reboot!

## Steps to root a GSI

* Download and install **[7-Zip Z Standard](https://github.com/mcmilk/7-Zip-zstd/releases)**
* Open the AP firmware file (that you'd usually flash via Odin) with 7-zip ZS
* Extract the boot.img.lz4
* Open the the boot.img.lz4 with 7-zip ZS
* Extract the boot.img
* Download and install the latest **[Magisk Manager apk](https://github.com/topjohnwu/Magisk/releases)**
* Copy boot.img to your phone
* Open the Magisk app
* Choose "Select and Patch a file"
* Pick your boot.img
* Take that patched image from Downloads and put it on your PC
* Boot into fastboot via the recovery
* `fastboot flash boot <patched boot image name or whatever>.img` 
* Reboot
* It will bootloop so make the phone go into recovery once more, where it'll offer you to Factory Reset since the phone is having a seizure
* Perform that factory reset and reboot

## Steps to fix video recording audio 
***You need to be rooted for this (you can hide Magisk from banking apps via Zygisk and pass CTS with the Kdragon's fix: [Kdragon's SafetyNet Fix](https://github.com/kdrag0n/safetynet-fix/releases))***
* Download and install the following Magisk module within the Magisk app: [Samsung Galaxy S22 Audio Policy Fix](https://www.mediafire.com/file/0iin55q7av3kl30/galaxy-s22-audio-policy-fix.zip/file)
* Reboot
* Go to Settings-> Phh Treble Settings -> Samsung features and enable **Use alternate audio policy**


## How to have working video recording audio without root
Long story short, this would encompass building a customized GSI.
I have made a modified device tree and a build script for building a Pixel Experience GSI, so feel free to clone this if you're feeling frisky:
https://github.com/jgudec/treble_build_pe

If you're too lazy, I've made rootless Pixel Experience Plus builds with Google Apps (and other fixes) that I upload in the Telegram group mentioned below.


## Telegram Group

[Telegram Group](https://t.me/+Ehf3IgzJw0k0NmE8)

## Hardware support

| Component                 |      Comment                                                      |
|---------------------------|-------------------------------------------------------------------|
| Camera                    | Works (Front and Back) - Haven't tested other back cams **           |
| Speaker / Mic             | Works                                                             |
| Bluetooth                 | Works (Tested only audio playback)                                      |
| WiFi                      | Works                                                             |
| SIM / Mobile Data / Voice | Works                                                             |
| VoLTE                     | Unknown                                                           |
| Fingerprint               | Works                                                             |
| NFC                       | Works (Used 2FA key)                                              |
| Offline Charging          | Broken                                                           |
| 120Hz                     | Enable in Settings > Phh Treble Settings > Misc features > Force FPS               |
| Auto-brightness            | Works (It can be a bit wonky so do personalize the brightness levels to your needs once and you should be good)               |
| Proximity sensor            | Broken              |
| Audio in video recording playback           | Fixed (see instructions above)            |
---

**In the stock camera, everything should work (except the nightmare fuel audio from video recordings) but the quality is ass. With GCam, however, you get better quality at the cost of instability that you yourself have to tinker with to reach some stability: https://www.ytechb.com/google-camera-for-samsung-galaxy-s22-plus-and-s22-ultra/
 - I personally recommend the 8.4 one (with its config and lib), and make sure to find and enable the "Exynos fix" to remove the color banding from photos.
 - As an alternative, try [MGC_8.1.101_A9_GV1zfix_MGC.apk](https://www.celsoazevedo.com/files/android/google-camera/dev-bsg/f/dl75/2/) along with [This XML config](https://www.mediafire.com/file/54ebe3prtq8y61b/Eric_JaJo_BSG_V8.1_%25283%2529.xml/file) (double tap between the shutter button and the gallery button while in the camera app in order to apply the config)

Feel free to edit if you find a better port/config.

Tested By: https://github.com/JeikWazTaken - SM-901B, DescendantOS 13.06.2022 v414 build - Tested on 26/06/2022 - Template created by @zguithues and @hackintosh5

