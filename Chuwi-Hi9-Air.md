# Chuwi Hi9 Air (Mediatek Helio X20 chipset)

Pretty complete [hardware](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) support and good stability with **8.1** Treble GSI (Oreo).

## Steps to install

Baseline: Hi9 Air with Chuwi 20181122 stock ROM.
* enable "OEM unlock" in Android developer options (type on build number seven times to unlock developer mode in Android system seetings)
* use factory settings reset in Android system settings and power off
* start device with `power` and `vol+` simultaneously for bootloader menu, select "Fastboot Mode" via 'vol+', then confirm OK via 'vol-'
* unlock bootloader (this will persist, unless stock ROM is [restored](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) using the MTK flash toolkit)
    ```
    $ fastboot oem unlock (confirm onscreen)
    ```
    > Caveat: When relocking the bootloader again via `fastboot oem lock` the device won't boot any custom image...
* flash [image](https://github.com/phhusson/treble_experimentations/releases) with the `fastboot` utility (after uncompressing downloaded xz archive) -> this may be repeated for later image releases with fixes and Android security patches:
    ```
    $ fastboot erase system
    $ fastboot erase cache
    $ fastboot -u flash system system-arm64-aonly-gapps-su.img
    $ fastboot reboot
    ```
     > Alternatively, you could flash via TWRP as "System Image" and format data: [Link](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)
* wait patiently for initial boot to complete (this will take several minutes, you may monitor progress via `adb shell top` for instance) 

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both work, front cam orientation upside down)        |
| Speaker / Mic             | yes / yes                                                 |
| Bluetooth                 | yes                                                       |
| WiFi                      | yes                                                       |
| SIM / Mobile Data         | yes (SIM1 only, may not reactivate from standby occasionally)|
| Voice                     | yes                                                       |
| SMS                       | yes                                                       |
| VoLTE                     | no (MTK 6797)                                             |
| Fingerprint               | n/a                                                       |
| NFC                       | n/a                                                       |
| SD Card                   | yes                                                       |
| Casting                   | no, only via Google Home (as for Chuwi stock ROM)         |
---

Tested by bofh2k - phh-treble 8.1 v31 (arm64-aonly-gapps-su) - 2019-05-31