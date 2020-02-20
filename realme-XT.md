# Realme XT (RMX1921)
## Steps to install
* Unlock bootloader (https://c.realme.com/in/post-details/1184740422732218368)
* Download any Phh based GSI
* Download thesprinster's LineageOS and vbmeta (https://drive.google.com/drive/folders/1JwIpix76opSAToa-4X4YdT_SH5JUOxJQ)
* Take thesprinster LineageOS's boot.img
* Flash *.img file using thesprintster's TWRP (https://forum.xda-developers.com/realme-xt/development/recovery-unofficial-twrp-realme-5-pro-t3985459) or via fastboot :
    ```
    $ fastboot flash system *.img && fastboot -w && fastboot reboot recovery 
    ```
* Flash thesprinster's boot.img from TWRP
* Flash thesprinster's vbmeta via fastboot (only for first time flashing ROM after using stock ColorOS) :
    ```
    $ fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img 
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Back Camera               | Working                                                   |
| Front facing Camera       | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | BT media doesn't work                                     |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | SIM-1 messages doesn't work                               |
| VoLTE                     | Not Working                                               |
| In-display Fingerprint    | Not Working                                               |
| Offline Charging          | Working                                                   |
| Tethering                 | Working                                                   |
| Hotspot                   | Working                                                   |
| Auto-Brightness           | Working                                                   |
---

Tested By: Kamildotmus / whitefox9000 - RMX1921 , Firmware version - RMX1921EX_11.A.11, Date tested - 04/11/2019.

Tested By: pjgowtham/ Lineage 17.1 GSI -RMX1921 , Firmware version - RMX1921EX_11.A.14, Date tested - 06/01/2020.

Template created by @zguithues and @hackintosh5