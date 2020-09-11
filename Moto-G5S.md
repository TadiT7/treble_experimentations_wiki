# Moto G5S

Suitable for daily usage, on both Android 9 and 10

## Steps to install

### Clean Install Android 9  (A-Only)
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Flash [this Vendor](https://t.me/MotoXProject/448).
* Flash a suiting Gsi (Arm64 A-Only)
* Reboot to system.

### Dirty flash

**Whole system:**
* Reboot to TWRP.
* Flash the latest [Vendor](https://t.me/MotoXProject/448) zip.
* Flash the updated Gsi (Arm64 A-Only)
* Reboot to system.

<!--**Vendor & Boot Images only:**
* Download the latest vendor & boot images (flashable zip) [here](https://t.me/MotoXProject/448).
* Reboot to TWRP.
* Flash the images (Install > Install Image > select partition > select image).
* Reboot to system.-->

### Install Android 10 (A/B)
* Flash [this TWRP](https://twrp.me/motorola/motorolamotog5s.html) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Vendor, Data, Cache and Dalvik/ART Cache.
* Flash [Lineage 17.1by JarlPenguin](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495), using TWRP
* Flash [Disable Force Encrypt](https://androidfilehost.com/?fid=1322778262904004415)
* Flash [Permissiver V5](https://androidfilehost.com/?fid=6006931924117940902) for Proper boot.
* Flash an Arm64 A/B Gsi
* Reboot to system.
* Enjoy!

### Dirty flash Android 10 (Whole system)
* Reboot to TWRP.
* Flash the latest [ROM](https://forum.xda-developers.com/moto-g5s/development/rom-lineageos-17-1-t4160495) zip.
* Flash the updated Gsi (Arm64 A-Only)
* Reboot to system.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (fully on Q, partially on P)                      |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working                                                   |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | Encryption - Partially working (Android Q)                |
## GSI support

<details><summary>Booting:</summary>
<p>

`Everything except in the "didnt boot" category`

</p>
</details>

<details><summary>Not Booting:</summary>
<p>

`Any Dynamic Partition ErfanGSI`

`RealmeUI`

`Moto Stock Q`

`Nubia`

`RedMagic`

`Xperia`

`One UI - GSI is too big for /system`
</p>
</details>

---

Tested By: HowToRush (XT1794) Oreo Latest  1.1.2020-11.09.2020

Also tested by: Giv314, Comeb4ck, and several other members of the montana community over at @Montanalabtesters!

Template created by @zguithues and @hackintosh5