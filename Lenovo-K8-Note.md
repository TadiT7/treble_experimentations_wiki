# Lenovo K8 Note

GSIs run stable and can be used as daily driver. Most of the features are working. This device got unofficial treble support.
Details and download link can be found [here.](https://forum.xda-developers.com/k8-note/development/rom-lineageos-15-0-rom-lenovo-k8-note-t3914630)

## Steps to install

* Follow the steps given in the above link to flash the treblised rom.
* Flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (HDR Mode not working)                            |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not Working                                               |
| Fingerprint               | Working                                                   |
| NFC                       | N/A                                                       |
| SD Card                   | Working                                                   |
---

## Tested By:
* [Maanush Putcha](https://github.com/Maanush2004)
* Prem Vijay
* Sachin Jangir