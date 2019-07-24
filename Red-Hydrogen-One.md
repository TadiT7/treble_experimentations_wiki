# [Red Hydrogen One] - [HydrogenONE]

## Hardware Support (AOSP 8.1)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | TBA                                                         |
| Speaker / Mic             | TBA                                                         |
| Bluetooth                 | TBA                                                         |
| WiFi                      | TBA                                                         |
| SIM / Mobile Data / Voice | TBA                                                         |
| VoLTE                     | TBA                                                         |
| Fingerprint               | TBA                                                         |
| NFC                       | TBA                                                         |


## Hardware Support (AOSP 9)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | TBA                                                         |
| Speaker / Mic             | TBA                                                         |
| Bluetooth                 | TBA                                                         |
| WiFi                      | TBA                                                         |
| SIM / Mobile Data / Voice | TBA                                                         |
| VoLTE                     | TBA                                                         |
| Fingerprint               | TBA                                                         |
| NFC                       | TBA                                                         |


***
## Additional Notes

Bootloader Unlock procedure is pretty regular, I strongly recommend you to perform both flashing unlock_critical and flashing unlock.

To prevent flashing error, you need to add parameter "-S 131073K".

e.g. 
`fastboot flash system_b E:\system-arm64-ab-gapps-su.img -S 131073K`
***


## Tested By:
* Calyx Hikari (HikariCalyx) @ Red Hydrogen One (Verizon Wireless) H1A1000.010ho.01.01.01r.109 @ 24/07/2019


Template created by @zguithues