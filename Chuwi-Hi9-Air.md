# Chuwi Hi9 Air (Mediatek Helio X20 chipset)

Pretty complete [hardware](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) support and good stability with **8.1** (Oreo) and **9.0** (Pie) Treble GSI.

## Steps to install

Baseline: Hi9 Air with Chuwi 20181122 stock ROM.
Restore Chuwi stock ROM via the MTK [SP Flash](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) Windows toolkit using the `Format All + Download` option, in case anything goes wrong.
* enable "OEM unlock" in Android developer options
  >:information_source: type on build number seven times to unlock developer mode in Android system settings: System>About
* use factory settings reset in Android system settings
* wait for erase to finish and power off (long press)
* start device with `power` and `vol+` simultaneously for bootloader menu, select "Fastboot Mode" via 'vol+', then confirm OK via 'vol-'
* unlock bootloader
    > ℹ️ You may keep the bootloader locked, if [TWRP](https://drive.google.com/open?id=1pl3XaTkKen9yL98toJX-Y_0uanwuEL4d) is installed via SP Flash as well and you subsequently install the system image and OpenGApps via TWRP...    ```
    $ fastboot oem unlock
    ```
    Confirm OK on screen via 'vol+'.
    > :warning: When relocking the bootloader again via `fastboot oem lock` the device won't boot custom images any longer...
    
* flash [image](https://github.com/phhusson/treble_experimentations/releases) with the `fastboot` utility (after uncompressing downloaded xz archive):
    ```
    $ fastboot erase system
    $ fastboot -u flash system system-arm64-aonly-vanilla-nosu.img
    $ fastboot reboot
    ```
    :repeat: This step may be repeated for later image releases with fixes and Android security patches (tested successfully for v31>32)...
     > Alternatively, you could flash via TWRP as "System Image". Refrain from formatting data, as the device will fail to boot then :-1:: [Link](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)
* wait patiently for another erase job to finish and initial boot (which now displays android animation instead of CHUWI) to complete: This will take several minutes 

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both work, front cam orientation upside down)        |
| Speaker / Mic             | yes / yes                                                 |
| Bluetooth                 | yes (works for 8.1 GSI, with 9 GSI enable the Mediatek workaround under phh treble settings > misc features > bluetooth workarounds  )                       |
| WiFi                      | yes (but signal seems worse compared to stock ROM)        |
| SIM / Mobile Data         | partial (SIM1 only, does not reactivate after standby - reboot required)|
| Voice                     | yes                                                       |
| SMS                       | yes                                                       |
| VoLTE                     | no (MTK 6797)                                             |
| Fingerprint               | n/a                                                       |
| NFC                       | n/a                                                       |
| SD Card                   | yes                                                       |
| Casting                   | no, only via Google Home (as for Chuwi stock ROM)         |
---

Tested by bofh2k - phh-treble 8.1 v32 & 9 v123 (arm64-aonly-vanilla-nosu) - 2020-02-29