# Motorola Moto G7 Play (XT1952) (channel)

The Motorola Moto G7 Play uses the A/B system image type and requires arm32-binder64 images.

## Steps to install

Installation is as easy as it can get:

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
* Once you flashed the GSI you might want to the hardware overlay for the Motorola Moto G7 Play,
  which isn't yet included by default:
  https://github.com/phhusson/vendor_hardware_overlay/pull/182. This adds some device specifc
  properties to properly support notch, battery and other components.

## Hardware support (Android 10)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                     |
| Speaker / Mic             | Works, but audio effects are disabled as a workaround for working Bluetooth audio for now                                                     |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works, but microphone in calls requires certain audio settings, see https://github.com/phhusson/treble_experimentations/issues/1138 |
| VoLTE                     | Unknown, disabled in stock ROM                            |
| Fingerprint               | Not working, see https://github.com/phhusson/treble_experimentations/issues/1072 |
| Offline Charging          | Works                                                     |
| GNSS                      | Works                                                     |
| Display                   | Works, except for automatic brightness adjustment         |


## Stock ROMs

Motorola stock ROMs are available here for the
[Motorola Moto G7 Play (channel)](https://mirrors.lolinet.com/firmware/moto/channel/official/) in
case you want to go back to stock ROM. Make sure you use the correct ROM for your model, otherwise
you may run into weird issues.

---

Tested By: @Dunedan - XT1952-1 (Europe), AOSP 10 vanilla v212 and newer versions
