# Chuwi Hi9 Air (Mediatek Helio X20 chipset)

Pretty complete [hardware](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) support and good stability with **8.1** (Oreo), **9.0** (Pie), **10** and **11** Treble GSIs.

**CAVEAT: Please note that the standby battery [drain](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682/post82724665#post82724665) is way higher for Pie and 11 GSIs (compared to Oreo)** ~~and Ten GSIs still seem to be stuck on [boot](https://github.com/phhusson/treble_experimentations/issues/1305#issuecomment-674668358)~~.

Ten GSIs stuck-on-boot problem is solved by following [these steps](https://github.com/phhusson/treble_experimentations/issues/1305#issue-615321725) or installing [this zip](https://forum.xda-developers.com/attachments/testmodhi9air-signed-zip.5125591/) through TWRP recovery. For Magisk users, it's also necessary to use the [phh-magisk](https://github.com/ExpressLuke/phh-magisk-builder/releases) instead of the official one to avoid problems with Zygote crashing. An expanded tutorial for installing Ten GSIs can be found [here](https://forum.xda-developers.com/t/chuwi-hi9-air-64gb-mt6797-x20-deca-core-10-1-inch-2k-screen-android-8-dual-4g-tablet.3775682/post-83659003), and a working overlay for Ten GSI builds can be downloaded [here](https://forum.xda-developers.com/t/chuwi-hi9-air-64gb-mt6797-x20-deca-core-10-1-inch-2k-screen-android-8-dual-4g-tablet.3775682/post-83996833).

## Steps to install

Baseline: Hi9 Air with Chuwi 20181122 stock ROM.
Restore Chuwi stock ROM via the MTK [SP Flash](https://forum.xda-developers.com/general/device-reviews-and-information/chuwi-hi9-air-64gb-mt6797-x20-deca-core-t3775682) Windows toolkit using the `Format All + Download` option, in case anything goes wrong.
* enable "OEM unlock" in Android developer options
  >:information_source: type on build number seven times to unlock developer mode in Android system settings: System>About
* use factory settings reset in Android system settings
* wait for erase to finish and power off (long press)
* start device with `power` and `vol+` simultaneously for bootloader menu, select "Fastboot Mode" via 'vol+', then confirm OK via 'vol-'
* unlock bootloader
    > ℹ️ You may keep the bootloader locked if [TWRP](https://drive.google.com/open?id=1pl3XaTkKen9yL98toJX-Y_0uanwuEL4d) is installed via SP Flash as well and you subsequently install the system image and OpenGApps via TWRP...

    ```
    $ fastboot oem unlock
    ```
    Confirm OK on-screen via 'vol+'.
    > :warning: When relocking the bootloader again via `fastboot oem lock` the device won't boot custom images any longer...
    
* flash [image](https://github.com/phhusson/treble_experimentations/releases) with the `fastboot` utility (_after_ uncompressing the downloaded xz archive):
    ```
    $ fastboot erase system
    $ fastboot -u flash system system-arm64-aonly-vanilla-nosu.img
    $ fastboot reboot
    ```
    :repeat: This step may be repeated for later image releases with fixes and Android security patches (tested successfully for v31>32>123)...
     > Alternatively, you could flash the img file via TWRP as "System Image". Refrain from formatting data, as the device will _fail to boot_ then: -1: ([Link](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)) - unless you remove device encryption first: Using TWRP you have to install [remove_encryption_97.zip](https://4pda.ru/forum/index.php?showtopic=907162&st=600#entry79417598) and reboot to recovery before proceeding by reformatting the data partition in TWRP.
* wait patiently for another erase job to finish and initial boot (which now displays an "Android" animation instead of "CHUWI") to complete: This will take several minutes

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | yes (both works, front cam orientation may be upside down)        |
| Speaker / Mic             | yes / yes                                                 |
| Bluetooth                 | yes (works for 8.1 GSI, with 9 GSI and above enable the Mediatek workaround under ```phh treble settings > misc features > Bluetooth workarounds ```)                       |
| WiFi                      | yes (but signal reception seems worse compared to stock ROM)        |
| SIM / Mobile Data         | partial (SIM1 only, does not always reactivate after standby - reboot required)|
| Voice                     | yes                                                       |
| SMS                       | yes                                                       |
| VoLTE                     | no (unresolved issue for MTK 6797)                                             |
| Fingerprint               | n/a                                                       |
| NFC                       | n/a                                                       |
| SD Card                   | yes                                                       |
| Casting                   | no, only via Google Home (as for Chuwi stock ROM)         |

---

Tested by bofh2k - phh-treble 8.1 GSI v32 & 9 GSI v123 (arm64-aonly-vanilla-nosu) - 2020-02-29

Tested by santosst3 - phh-treble quack GSI v222 & roar GSI v300.l (arm64-aonly-vanilla) - 2021-02-08