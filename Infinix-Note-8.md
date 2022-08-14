# [Infinix Note 8] - [x692]

Helio G80 (MT6769)

Overall excellent, things are working as expected.

Tested with Phh's GSI, LineageOS, CAOS, and PixelExperience (Android 10, 11 & 12)

## Steps to install

* Grab an ARM64 A/B GSI ROM image [here](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list) or from other source
* Unlock the bootloader and go into bootloader mode
* Reflash the original vbmeta image but with verification disabled using the `fastboot` utility:
    ```
    $ fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
    ```
* Reboot to fastbootd
* Flash the system image with the `fastboot` utility:
    ```
    $ fastboot flash system system-image.img
    ```

* Tip: If you're running out of space, you could remove the `product` partition by doing this (this might be destructive):
    ```
    $ fastboot delete-logical-partition product
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | OK                                                        |
| Speaker / Mic             | OK                                                        |
| Bluetooth                 | OK                                                        |
| WiFi                      | OK                                                        |
| Hotspot / Tethering       | OK                                                        |
| SIM / Mobile Data / Voice | OK                                                        |
| VoLTE                     | OK (Android ≥11)                                          |
| Fingerprint               | OK                                                        |
| NFC                       | Unsupported                                               |
| Offline Charging          | OK                                                        |
---

## Additional Notes

* This device uses ARM64 CPU architecture and A/B image (because of system-as-root partition scheme), but does not support seamless update.

Tested By: [リェンーゆく (ryenyuku)](https://github.com/ryenyuku) @ Infinix Note 8 (x692), X692-H694KLMX-Q-GL-220311V412 - Last edited on 08/08/2022 - Template created by @zguithues and @hackintosh5