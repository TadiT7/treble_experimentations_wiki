# Device

Seems to work fine with the base AOSP 11 image, vanilla and gapps; others get stuck or bootloop. This is on an SM-F700N - the Korean variant - but it will likely work on other bootloader-unlockable variants as well. I haven't tried this at all with Android 10.

Occasionally a reboot will go silly and just not want to work right; in that case, another reboot usually fixes it.

## Steps to install

* Update to the latest current firmware. As I recall, I had the May 2021 security patch when I started this process.
* Follow the instructions [here](https://forum.xda-developers.com/t/recovery-lineageos-recovery-for-f700f.4192011/) to install a suitable recovery. There is no need to disable encryption - Step 4 on 
* Boot into the just-installed recovery, switch it into fastbootd mode (Advanced -> Enter Fastboot), and flash the image:
    ```
    $ fastboot erase system
    $ fastboot flash system system-arm64-ab-gapps.img
    ```
* Return to recovery, wipe data, reboot.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                     |
| Speaker / Mic             | Speaker works, mic untested                               |
| Bluetooth                 | Untested                                                  |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | SIM works, mobile data works, voice untested              |
| VoLTE                     | Untested but unlikely                                     |
| Fingerprint               | Works                                                     |
| NFC                       | Untested                                                  |
| Offline Charging          | Untested                                                  |
| Wireless Charging         | Works                                                     |
| Automatic brightness      | Not working                                               |
| MTP                       | Untested                                                  |
| Cover display             | Behaves as a rotated mirror of the main display.          |
---

Tested By: Sarah Vandomelen (@irony_delerium on Telegram) - SM-F700N (Korea), firmware F700NKOU2DUD9 - Android 11, OneUI 3.1 - Jun 13, 2021 - Template created by @zguithues and @hackintosh5