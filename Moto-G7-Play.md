# Motorola Moto G7 Play (XT1952) (channel)

The Motorola Moto G7 Play uses the A/B system image type and requires arm32-binder64 images if based on stock firmware.

## Steps to install 32 Bit

Installation is as easy as it can get:

* Ensure no custom roms are installed
* Ensure your bootloader is unlocked. If not, head over to Motorola's website to get it unlocked.
* Get the GSI you want to flash (which could be any A/B arm32-binder64 GSI):
  https://github.com/phhusson/treble_experimentations/releases
* Put the phone into `fastboot` mode (switch it off, then press and hold "power" + "volume down"
  until you're in recovery mode)
* Perform a factory reset:
    ```
    $ fastboot -w
    ```
* Flash the GSI image with the `fastboot` utility:
    ```
    $ fastboot flash system system-quack-arm32_binder64-ab-vanilla.img
    ```
* After flashing during every boot before showing the "Android" boot logo the string "bad key" is
  shown on the screen. That's expected and a result of the system image not signed by Motorola's keys.

## Hardware support (Android 10 GSI)

| Component                 | coming from stock Android 9 | coming from stock Android 10 |
|---------------------------|-----------------------------|------------------------------|
| Camera                    | Works                       | Works                        |
| Speaker / Mic             | Works                       | Works                        |
| Bluetooth                 | Works                       | Works                        |
| A2DP                      | Works                       | Not working, see [#1404](https://github.com/phhusson/treble_experimentations/issues/1404) |
| WiFi                      | Works                       | Works                        |
| SIM / Mobile Data / Voice | Works, but microphone in calls requires certain audio settings, see [#1138](https://github.com/phhusson/treble_experimentations/issues/1138) | Works |
| VoLTE                     | Unknown, disabled in stock ROM | Unknown, disabled in stock ROM |
| Fingerprint               | Not working, see [#1072](https://github.com/phhusson/treble_experimentations/issues/1072) |  Not working, see [#1072](https://github.com/phhusson/treble_experimentations/issues/1072) |
| Offline Charging          | Works                       | Works                        |
| GNSS                      | Works                       | Works                        |
| Display                   | Works                       | Works                        |
| Automatic screen brightness | Not Working               | Works                        |


## Hardware support (Android 11 GSI)

| Component                 | coming from stock Android 10 |
|---------------------------|------------------------------|
| Camera                    | Works                        |
| Speaker / Mic             | Works                        |
| Bluetooth                 | Works                        |
| A2DP                      | Not working, see [#1404](https://github.com/phhusson/treble_experimentations/issues/1404) |
| WiFi                      | Works                        |
| SIM / Mobile Data / Voice | Works                        |
| VoLTE                     | Unknown, disabled in stock ROM |
| Fingerprint               | Works                        |
| Offline Charging          | Works                        |
| GNSS                      | Works                        |
| Display                   | Works                        |
| Automatic screen brightness | Works                      |

## Hardware support (Android 12 GSI)

* use at least version v412 to get everything working as shown below

| Component                 | coming from stock Android 10 |
|---------------------------|------------------------------|
| Camera                    | Works                        |
| Speaker / Mic             | Works                        |
| Bluetooth                 | Works                        |
| A2DP                      | Works                        |
| WiFi                      | Works                        |
| SIM / Mobile Data / Voice | Works                        |
| VoLTE                     | Unknown, disabled in stock ROM |
| Fingerprint               | Works                        |
| Offline Charging          | Works                        |
| GNSS                      | Works                        |
| Display                   | Works                        |
| Automatic screen brightness | Works                      |


## Stock ROMs

Motorola stock ROMs are available here for the
[Motorola Moto G7 Play (channel)](https://mirrors.lolinet.com/firmware/moto/channel/official/) in
case you want to go back to stock ROM. Make sure you use the correct ROM for your model, otherwise
you may run into weird issues.

---

Tested By: @Dunedan - XT1952-1 (Europe), AOSP 10 vanilla v212 and newer versions





# 64 Bit

## Steps to install 64 Bit

Installation is slightly more difficult:

* Ensure a custom rom is installed (LineageOS recommended)
* Ensure your bootloader is unlocked. If not, head over to Motorola's website to get it unlocked.
* Get the GSI you want to flash (which could be any A/B arm64 GSI):
  https://github.com/phhusson/treble_experimentations/releases
* Put the phone into `fastboot` mode (switch it off, then press and hold "power" + "volume down"
  until you're in recovery mode)
* Perform a factory reset:
    ```
    $ fastboot -w
    ```
* Flash the GSI image with the `fastboot` utility:
    ```
    $ fastboot flash system system-quack-arm364-ab-vanilla.img
    ```
* After flashing during every boot before showing the "Android" boot logo the string "bad key" is
  shown on the screen. That's expected and a result of the system image not signed by Motorola's keys.