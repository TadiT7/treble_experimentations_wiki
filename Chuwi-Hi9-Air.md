# Chuwi Hi9 Air (Mediatek Helio X20 chipset)

Pretty complete [hardware](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) support and good stability with **8.1** image.

## Steps to install

Baseline: Hi9 Air with Chuwi 20181122 stock ROM.
* enable "OEM unlock" in Android developer options (type on build number seven times)
* use factory settings reset in Android system settings and power off
* start device with `power` and `vol+` simultaneously for bootloader menu, select "Fastboot Mode" via 'vol+', then confirm OK via 'vol-'
* flash [image](https://github.com/phhusson/treble_experimentations/releases) with the `fastboot` utility:
    ```
    $ fastboot oem unlock (confirm onscreen)
    $ fastboot erase system
    $ fastboot -u flash system system-arm64-aonly-gapps-su.img
    ```

Alternativly, you could flash via TWRP as "System Image" and format data: [Link](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both work, but front cam upside down)                |
| Speaker / Mic             | yes / yes                                                 |
| Bluetooth                 | yes                                                       |
| WiFi                      | yes                                                       |
| SIM / Mobile Data         | yes (only SIM1 tested, may not reactivate from standby occasionally)|
| Voice                     | yes                                                       |
| SMS                       | yes                                                       |
| VoLTE                     | no (MTK6797)                                              |
| Fingerprint               | n/a                                                       |
| NFC                       | n/a                                                       |
| SD Card                   | yes                                                       |
| Casting                   | not from menu, only via Google Home (as in Chuwi stock ROM)|
---

Tested By: bofh2k - phh-treble 8.1 v31 (arm64-aonly-gapps-su) - 2019-05-31