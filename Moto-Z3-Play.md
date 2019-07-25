# Moto Z3 Play (Beckham) arm64 A/B

Summary of what works and doesn't
- **DO NOT USE STOCK VENDOR**
## Steps to install

* Step 1
- Obtain bootloader unlock from Motorola
* Step 2
- Flash latest TWRP by @jleeblanch and follow directions on XDA for Resurrection Remix
* Step 3
* flash this image with the `fastboot` utility:
    ```
    $ fastboot erase userdata
    $ fastboot flash system system-arm64-b-gapps-su.img
    ```
    Some more info

    As an alternative you can flash via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                    |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works but aptX Adaptive unavailable unlike stock                                                    |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Definitely works on GSM network but CDMA like Verizon may have issues                                                    |
| VoLTE                     | Not working on any CDMA network tested, may have issues with other network                                                 |
| Fingerprint               | Works but may have issues with apps using fingerprint authentication                                                    |
| NFC                       | Works                                                    |
| Offline Charging          | Works                                                   |
| Moto Mods                 | Not working                                                    |
---

Tested By: alexa-v2, jleeblanch, people in our Telegram group
- Region/model: Should work on any that allows bootloader unlock, mainly because it needs a custom ROM vendor to work correctly
- Firmware: Resurrection Remix latest (stock vendor has issues), or latest lineage (less testing done here though)
- Tested 05/2019 - now
- Template created by @zguithues and @hackintosh5

