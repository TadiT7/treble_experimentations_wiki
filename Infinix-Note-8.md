# [Infinix Note 8] - [x692]

Helio G80 (MT6768)

Overall excellent, things are working as expected.

Tested with Havoc-OS GSI 3.12 (Android 10)

## Steps to install

* Grab an ARM64 A/B GSI ROM image [here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list) or from other source
* Grab the modified vbmeta image from [here](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img)
* Unlock the bootloader and go into bootloader mode
* Flash the vbmeta image with the `fastboot` utility:
    ```
    $ fastboot flash vbmeta vbmeta.img
    ```
* Reboot to fastbootd
* Flash the system image with the `fastboot` utility:
    ```
    $ fastboot flash system system-image.img
    ```

* Tip: If you're running out of space, you could resize the `product` partition to be smaller by doing this:
    ```
    $ fastboot resize-logical-partition product [SIZE]
    $ fastboot format:ext4 product
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                    |
| Speaker / Mic             | OK                                                    |
| Bluetooth                 | OK                                                    |
| WiFi                      | OK                                                    |
| Hotspot / Tethering         | OK                                                    |
| SIM / Mobile Data / Voice | OK                                                    |
| VoLTE                     | OK                                                    |
| Fingerprint               | OK                                                    |
| NFC                       | Unsupported                                                    |
| Offline Charging          | OK                                                    |
---

## Additional Notes

* `product` partition must NOT be deleted. Otherwise it wouldn't boot.
* This device uses ARM64 CPU architecture and A/B image (because of system-as-root partition scheme), but does not support seamless update.

Tested By: [リェンーゆく (ryenyuku)](https://github.com/ryenyuku) @ Infinix Note 8 (x692), X692-H694KLMX-Q-GL-201016V237 - 28/03/2021 - Template created by @zguithues and @hackintosh5