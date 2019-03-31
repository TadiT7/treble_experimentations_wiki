# Pixel (Sailfish)

## Testers

* [Jim-Bar](https://github.com/Jim-Bar)

## Hardware

Has been tested on:
* Sailfish US 128Go
* Sailfish ROW 32Go

## GSI tested

[phh](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) and [LineageOS](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690). Both work.

## Procedure used

**Warning:** this has an [issue](https://github.com/phhusson/treble_experimentations/issues/55) which prevents the phone from booting more than three time. The workaround is in the linked issue.

1. Download latest Google image available [here](https://developers.google.com/android/images#sailfish). For me it was 8.1.0 (OPM2.171019.029, Apr 2018).
2. `./flash-all.sh`
3. Reboot to fastboot, then erase the system partition: `fastboot erase system`
4. Flash the system image: `fastboot flash system system-arm64-ab-vanilla-nosu.img` (phh v18 2018-05-14, sha256: `302d2dc6dc55bce68f1ac1216fc05dd49eba3bab29bc3fef4d591bffd050dbcb`) or `fastboot flash system system-arm64-ab.img` (LineageOS v4 2018-05-19, sha256: `3f67636ba164d1c0f7b750070b6db16349e761e1e4dea2ee193b176477152b91`)
5. Erase the data partition: `fastboot -w`
6. Boot the phone

## Notes
- SIM is not detrecting on latest Pie furmwares
- but all other majors functionalities seems to work: camera, flash, wifi, bluetooth, sounds.

# Pixel XL (Marlin)

## Testers

* [Gabriel Howard](https://github.com/TheGabrielHoward)
* [Jim-Bar](https://github.com/Jim-Bar)

## Hardware

Has been tested on:
* Marlin EU 32GB
* Marlin US 32Go

## GSI tested

[phh](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) and [LineageOS](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690). Both work.

## Procedure used

**Warning:** this has an [issue](https://github.com/phhusson/treble_experimentations/issues/55) which prevents the phone from booting more than three time. The workaround is in the linked issue.

1. Download latest Google image available [here](https://developers.google.com/android/images#marlin). For me it was 8.1.0 (OPM4.171019.021.D1, Jun 2018).
2. `./flash-all.sh`
3. Reboot to fastboot, then erase the system partition: `fastboot erase system`
4. Flash the system image: `fastboot flash system system-arm64-ab-vanilla-nosu.img` (phh v19 2018-06-03, sha256: `9d130f709f063953a9d941f1ed4f33e050a60e61794cef459e22b3ac8f7eca20`) or `fastboot flash system system-arm64-ab.img` (LineageOS v4 2018-05-19, sha256: `3f67636ba164d1c0f7b750070b6db16349e761e1e4dea2ee193b176477152b91`)
5. Erase the data partition: `fastboot -w`
6. Boot the phone

## Notes
- SIM is not detecting