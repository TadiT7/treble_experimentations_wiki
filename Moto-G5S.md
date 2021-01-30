# Moto G5S

Suitable for daily usage, on Android 9, 10, and 11

## Steps to install

### Android 11
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://t.me/motog5s) (XDA post is down ATM)
* Flash [this zip](https://zackptg5.com/android.php#disverfe).
* Flash a GSI (arm64 A/B)
* Reboot to system.



### Android 10

#### Clean install
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://t.me/motog5s) (XDA post is down ATM)
* Flash a GSI (arm64 A/B)
* Reboot to system.

#### Dirty flash
* Reboot to TWRP.
* Flash [LineageOS 17.1](https://t.me/motog5s) (XDA post is down ATM) if needed.
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
| Other feature             | Encryption - Working (Android 10+, 11 Phh broken)                |

---

## Android 11 Notes
Any GSI from firmware collections will need [permissiver](https://androidfilehost.com/?fid=6006931924117940902) to boot, Phh's Roar GSI and Google's own Android 11 GSI don't need it.

If Android 11 still doesn't boot, contact @HowToRush over in [his telegram](t.me/howtorush), he will try to help you boot Android 11. 

Nusantara's official GSI _needs_ Magisk to boot.

---

Tested By: HowToRush (XT1794) Oreo Latest  1.1.2020-23.09.2020

Also tested by: Giv314, Comeb4ck, and other users from the [G5S Telegram](https://t.me/motog5schat)

Template created by @zguithues and @hackintosh5