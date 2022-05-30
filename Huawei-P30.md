# Huawei P30 (ELE-L29)

Summary of what works and doesn't

## Steps to install

You need to do an unofficial Bootloader Unlock.  
(Software test points using DC-Phoneix and HCU clients etc...)  
Due to the specifications of EMUI, if you downgrade a terminal that has been updated to EMUI 11, you will not be able to use USB, so it is necessary to select individuals that have not been updated to EMUI 11 or higher.

## Confirmed problem
Other devices will not recognize this device even if I make a USB connection.
(Perhaps the limits imposed by Huawei.)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | ☑|
| Speaker / Mic / Calls     | ☑|
| Bluetooth                 | ☑|
| WiFi                      | ☑                                                     |
| SIM / Mobile Data / Voice | unconfirmed                                              |
| VoLTE                     | Doesn't works                                             |
| Fingerprint               | △(There is a problem if you do not specify the coordinates.)                                                     |
| NFC                       | unconfirmed                                                     |
| Bluetooth calls           | unconfirmed                                                     |
---

## Tested by
* @j7b3y - [lineage-18.1 treble_arm64_bvS](https://sourceforge.net/projects/andyyan-gsi/files/lineage-18.x/lineage-18.1-20220511-UNOFFICIAL-arm64_bvS.img.xz) - Tested the 2021.10.11 

_Template created by @zguithues and @hackintosh5_