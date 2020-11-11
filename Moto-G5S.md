# Moto G5S

Suitable for daily usage, on Android 9, 10, and 11

## Steps to install

### Android 11
* See [steps for Android 10](https://github.com/phhusson/treble_experimentations/wiki/Moto-G5S#android-10)

### Android 10

#### Clean install
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495)
* Flash [permissiver](https://androidfilehost.com/?fid=6006931924117940902) (no longer needed for Phh based gsi since october update)
* Flash a GSI (arm64 A/B)
* Reboot to system.

#### Dirty flash
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495) if needed.
* Flash [permissiver](https://androidfilehost.com/?fid=6006931924117940902) (no longer needed for Phh based gsi since october update)
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

## Android 11 Notes
To boot android 11, you HAVE to use at least the october update, also known as 1.8 to be able to boot, **_any Gsi from firmware collections will need permissiver to boot_** (see above), Phh's Roar Gsi and Google's own Android 11 Gsi **_dont need permissiver_**

---

Tested By: HowToRush (XT1794) Oreo Latest  1.1.2020-23.09.2020

Also tested by: Giv314, Comeb4ck, and other users from the [G5S Telegram](https://t.me/motog5schat)

Template created by @zguithues and @hackintosh5