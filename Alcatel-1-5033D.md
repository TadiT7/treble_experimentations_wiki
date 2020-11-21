# Device

Only bluetooth doesn't seem to be working.

## Steps to install

Credits to: https://forum.xda-developers.com/alcatel-1/development/alcatel-1-root-achieved-t3970713

* In developer setttings, enable `OEM Unlocking`
* While powering on, hold power + volume up. Release power when the logo appears. Don't release volume up.
* Select `reboot to bootloader` with volume keys, confirm with power. On a PC run `fastboot oem unlock`.
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-quack-arm-aonly-vanilla.img
    ```
I have not heard of any 3rd party recovery to be working. 

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                    |
| Speaker / Mic             | √                                                    |
| Bluetooth                 | × fails to enable                                                    |
| WiFi                      | √                                                    |
| SIM / Mobile Data / Voice | mobile data works (germany, O2)                                                    |
| VoLTE                     | not tested                                                    |
| Fingerprint               | -                                                    |
| NFC                       | -                                                    |
| Offline Charging          | Status                                                    |
| Other feature             | Status                                                    |
---

Tested By: haagch - Model-Number(region): Alcatel 5033D-2BALWE1, Firmware Version: ?? - Date tested 21.11.2020, has been working for many months - Template created by @zguithues and @hackintosh5

Version tested: v222

Only 32 bit image system-quack-arm-aonly-vanilla.img was tested due to small system partition. CPU should be able to run 64 bit image. May be possible to delete partitions and expand system partition or use mtk flash tool. Supposed scatter file here, not tested by me: https://forum.xda-developers.com/alcatel-1/development/alcatel-1-3gb-partiton-scatter-progress-t4149465 / https://github.com/yag-dev-xda/Alcatel-5033-System-Resize