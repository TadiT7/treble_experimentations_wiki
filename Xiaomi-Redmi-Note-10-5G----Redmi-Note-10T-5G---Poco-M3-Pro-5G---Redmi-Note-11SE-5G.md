## Xiaomi Redmi Note 10 5G  / Redmi Note 10T 5G / Poco M3 Pro 5G / Redmi Note 11SE 5G (camellian)

**Supported GSI : A/B**

**Architecture : ARM64**


## Hardware Support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Front, back and auxiliary cam working. Recommended to enable "Expose Aux cameras" at Phh Treble Settings and use 3rd party GCam. |
| Speaker / Mic / Calls     | All works, but sometimes can't switch properly from Call mode to Loudspeaker.  |
| Bluetooth                 | Works, recommended to enable "Bluetooth workarounds" to Mediatek at Phh Treble Settings. |
| WiFi                      | Works.                                                    |
| SIM / Mobile Data / Voice | Works.                                                    |
| VoLTE                     | Works. Make sure install IMS for Mediatek and enable Force|
| Fingerprint               | Works.                                                    |
| NFC                       | Works.                                                    |
| Bluetooth calls           | Not Tested.                                               |
| Brightness                | ~~Flickering when switching brightness. Enable "Force alternative backlight scale", "Use linear screen brightness slider", and "Allows setting to the lowest possible" at Phh Treble Settings.~~ <br> ***Worked, check out overlays hotfix below.*** |
---

### Reboot the device to apply all changes.

## Tutorial

**!! THIS WILL ERASE YOUR INTERNAL DATA !!**

**Prerequisite:**
* Unlocked bootloader (obviously, duh)
* **NOT ROOTED**
* Fastbootd drivers (recommend to use [Google USB](https://developer.android.com/studio/run/win-usb)/[Xiaomi USB](https://developer.android.com/studio/run/oem-usb) drivers)
* [Patched vbmeta.img](https://t.me/pocom3proofficial/26442)

**How to:**
1. Connect your device to PC and open command prompt
2. Reboot your device to fastboot mode by pressing **Power + Volume Down** button
3. Make sure you do `fastboot devices` first before you proceed and make sure your devices are detected on list
4. After the device is detected, then do `fastboot reboot fastboot`
5. Do `fastboot devices` and make sure your devices are detected on list and your device is on fastbootd screen
6. Execute this command below
```
fastboot set_active a
fastboot delete-logical-partition product
fastboot erase system
```
7. After erase system partition, then we flash the GSI using command below:

```
fastboot flash system system-(prefix)*-arm64-ab-vanilla.img (change it to gsi file that you downloaded)
```

If there's invalid sparse file at flashing system, just ignore.

8. After that, we must flash vbmeta with the command below
```
fastboot --disable-verity --disable-verification flash vbmeta (vbmeta.img mod or patch)
fastboot flash vbmeta_b (vbmeta.img mod or patch)
fastboot set_active a
```
9. Then we reboot the device to recovery by using `fastboot reboot recovery`
10. In recovery, you select the wipe data and then reboot to your system.

***

If you are rooted with Magisk, you can flash [this hotfix module](https://t.me/pocom3proofficial/49907) for brightness and overlays. If not, enable "Force alternative backlight scale", "Use linear screen brightness slider", and "Allows setting to the lowest possible" at Phh Treble Settings.

## Tested Roms
*Feel free to contribute here if you ever tested other GSIs*
* NaokoShoto - camellian @ PixelExperience_arm64-ab-12.0-20211218 (Ponces build)
* KucingAbu - camellian @ ProjectElixir-3.6-gsi-13.0-20230223-1108-OFFICIAL (KrutosX & Lynix build)
* NaokoShoto - camellian @ evolutionX_arm64-ab-vndklite-7.6-unofficial-20230216 (Ponces build)