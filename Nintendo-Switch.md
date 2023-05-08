# Nintendo Switch (icosa)

Nintendo Switch isn't an android device but switchroot team ported android for it. First release was android lineage os 15 8.1.0 but non-treble. Currently the compiled android 9 build from source is Treble compatible. But there will be some problems, as the devs said they have framework patches of switchroot android images but GSI images somehow works on this device. Running android requires hacked Nintendo Switch v1 (Erista) unit. Android on Switch runs from SDcard, not from eMMC, so there will be speed issue.

Currently, Mariko-based Switch (including Lite, OLED) are unsupported - codenames of them are lowa, hoag, aula respectively.

## Steps to install

* Step 1
    In Hekate, select Tools - Partition SD Card and create partitions for Android.
* Step 2
    Copy Android installation files to your SD card via UMS.
* Step 3 flash this image with the `fastboot` utility:
    ```
    $ fastboot devices
    $ fastboot flash system system-arm64-ab.img
    ```
    
## Known issues
phh AOSP didn't booted but HavocOS and RR booted. Not all GSIs will boot currently due to early build of android, most of them will bootloop like RR but some of them will boot perfectly like HavocOS.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | This device don't have this hardware                      |
| Speaker / Mic             | Working (This device don't have microphone)               |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | This device don't have this hardware                      |
| VoLTE                     | This device don't have this hardware                      |
| Fingerprint               | This device don't have this hardware                      |
| NFC                       | This device don't have this hardware except controller                                                    |
| Offline Charging          | Not available                                             |
| Other feature             | Joycons connected via wired works                         |
---

Tested By: Fahim732 - Model-Grey Joycons (US), Firmware Version - depends on boot.scr and coreboot.rom Date tested - 10 April 2020