# Moto G5S

Suitable for daily usage, on both Android 9 and 10

## Steps to install

### Android 10

#### Clean install
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495)
* Flash [permissiver](https://androidfilehost.com/?fid=6006931924117940902)
* Flash a GSI (arm64 A/B)
* Reboot to system.

#### Dirty flash
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495) if needed.
* Flash [permissiver](https://androidfilehost.com/?fid=6006931924117940902)
* Flash the updated GSI (arm64 A/B)
* Reboot to system.

### Android 9

#### Clean install
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Flash [this vendor](https://t.me/MotoXProject/448).
* Flash a GSI (arm64 A-only)
* Reboot to system.

#### Dirty flash
* Reboot to TWRP.
* Flash the latest [vendor](https://t.me/MotoXProject/448) zip if needed.
* Flash the updated GSI (arm64 A-only)
* Reboot to system.


## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                      |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working                                                   |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | Encryption - Working (Android 10)                |

---

Tested By: HowToRush (XT1794) Oreo Latest  1.1.2020-23.09.2020

Also tested by: Giv314, Comeb4ck, and others

Template created by @zguithues and @hackintosh5