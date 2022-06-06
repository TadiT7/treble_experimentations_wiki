# Realme 8 5G /Narzo 30 5G (RMX3241 / RMX3242)
## Steps to install
* Unlock bootloader (https://forum.xda-developers.com/t/a-guide-to-unlock-the-bootloader.4306487)
* Download any Phh based GSI
* Flash GSI in fastbootd mode
  ```sh
  fastboot flash system *.img
  fastboot -w
  fastboot reboot recovery
  ```
* Flash disabled vbmeta via fastboot (only for first time flashing ROM after using stock ColorOS) :
    ```sh
    fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img 
    ```

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Back Camera               | Working                                                   |
| Front facing Camera       | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | only BT media doesn't work                                     |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                              |
| VoLTE                     | Working after MTK IMS setup in phh settings                                              |
| Side Fingerprint sensor   | Working                                             |
| Offline Charging          | Working                                                   |
| Tethering                 | Working                                                   |
| Hotspot                   | Works after installing this [Hotspot fix magisk module](https://t.me/Realme85G_Narzo305G_Official/13103)                                     |
| Auto-Brightness           | Working                                              |
---
Notes:
 * Use alternative brightness scaling
 * TWRP won't work for now

Tested by members of [Telegram group for these devices](https://t.me/Realme85G_Narzo305G_Official)
Template created by @zguithues and @hackintosh5