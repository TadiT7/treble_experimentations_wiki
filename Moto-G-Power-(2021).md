# Moto G Power (2021) - borneo

## Known Bugs:
* Making a phone call disconnects cellular service or downgrades from LTE to EDGE (Tested on Google Fi)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                    |
| Speaker / Mic             | Works                                                    |
| Bluetooth                 | Works                                                    |
| WiFi                      | Works                                                    |
| SIM / Mobile Data / Voice | Works for accessing the internet, making phone calls disconnects it |
| VoLTE                     | Untested                                                 |
| Fingerprint               | Works                                                    |
| Offline Charging          | Works                                                   |
---

## Requirements
* Unlocked Bootloader 
Known unlockable models: RETAIL and Google Fi models
If there are any other models that are unlockable, you may add them to this page 
If you recently purchased a bootloader unlockable device, it must be connected to the internet for at least 3 days for the "OEM Unlock" option in developer settings to be togglable 

## Notes
* Device must be booted to fastbootd in order to flash the GSI (Can be done via PC by typing in either `adb reboot fastboot` (If booted to Android) or `fastboot reboot fastboot` (If booted to bootloader)
* Logical partitions system_a and system_b may need to be deleted and recreated in order to flash the GSI, otherwise the flash may fail with `insufficient storage on system_a/b`. That can be done by doing `fastboot delete-logical-partition system_a` and `fastboot delete-logical-partition system_b`, then recreating the partitions by doing `fastboot create-logical-partition system_a 100000` and `fastboot create-logical-partition system_b 100000`. After that, you can flash as normal by doing `fastboot flash system IMAGENAMEGOESHERE.img`

## Testing Information
* Tested by Alvin64DD on 04/05/2022 on AOSP 12.1 v411
* Model tested: XT2117-4 (4GB + 64GB Model)
