# Moto G5

Not suitable for daily usage.

## Steps to install

### Clean flash
* Flash [this TWRP](https://drive.google.com/open?id=1XqpR6vYEbSXKZFD7StXc69jsh6YAOr3m) as "Recovery" in your existing recovery.
* Reboot again to TWRP.
* Format System, Data, Cache and Dalvik/ART Cache.
* Flash [this ROM](https://drive.google.com/a/al.educacao.sp.gov.br/uc?id=1onmjOKJAPFeiws8MXTyeMGwIIF6gguYj&export=download).

**Optional:**
* Reboot to TWRP.
* Format System.
* Flash a GSI as "System Image". Or alternatively use fastboot to flash the GSI:
```
fastboot flash system path/to/gsi.img
```
* Reboot to system.

### Dirty flash

**Whole system:**
* Reboot to TWRP.
* Flash the latest LineageOS Treble zip.
* Format system and reinstall your GSI.
* Reboot to system.

### Android 10
* Follow the clean flashing steps. Do **not** reboot.
* Flash [this](https://github.com/montanadevelopment/releases/releases/download/Android10Fixes-1/allzygotefix2.zip), then [this](https://github.com/montanadevelopment/releases/releases/download/Android10Fixes-1/lagfix-for-a_and_ab.zip).
* Reboot to system.

[Some more info](https://t.me/g5treble)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Not Working                                               |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not Working                                               |
| Fingerprint               | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | -                                                         |

## GSI support

<details><summary>Booting:</summary>
<p>

TBD
</p>
</details>

<details><summary>Not Booting:</summary>
<p>

TBD
</p>
</details>

---

Tested By: Brickador - XT1672 (Brazil), Firmware Version: Oreo B831, Date tested: TBD

Also tested by: ludke (SludkeSP)

Template created by @zguithues and @hackintosh5