# Samsung Galaxy M31s (SM-M317F/DS)

Summary of what works and doesn't
Very Low Latency with some stutters, Some slight bugs that are rehashed by rebooting(non repeating).

Safetynet does not pass on it's own. Need to do something with Root explorer.

## Steps to install

* Fastboot installation has not been tested
generic flash guide
  flash this image with the `fastboot` utility:
    ```
    $ a-command
    $ fastboot flash system system-arm64-aonly-gapps-su.img
    ```
    Some more info

* Tested by flashing via TWRP as "System Image" and format data.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works(but with no pixel binning)                          |
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Not Working                                               |
| VoWiFi                    | Not Working/Implemented                                   |
| Fingerprint               | Doesn't work on AOSP 12.1 v412                            |
| Offline Charging          | Maybe                                                     |
| Wi-Fi Hotspot             | 2.4 GHz Works, 5 GHz doesn't work on Corvus OS            |
| Other feature             | Status                                                    |
---

Tested By: khushtaur3123 - SM-M317F(INS), Bootloader/Radio - M317FXXU3CVC2

