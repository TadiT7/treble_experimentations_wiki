# Samsung Galaxy S10e

## Steps to install

* Enable developers settings
* Select OEM unlock in settings
* power off the phone, and unplug it
* boot into unlock mode: keep pressing bixby + vol down; plug-in usb
* follow instructions on-screen to oem unlock
* `sudo heimdall flash --SYSTEM system-arm64-ab-gapps-su.img`
* apply magisk's safedex disabler (   ./magiskboot hexpatch kernel 821B8012 E2FF8F12 )

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works                                                     |
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Not working                                               |
| WiFi                      | Status                                                    |
| SIM / Mobile Data / Voice | Works [2]                                               |
| VoLTE                     | Status                                                    |
| Fingerprint               | Not working [1]                                           |
| NFC                       | Unknown                                                   |
| Offline Charging          | Unknown                                                   |

---

[1] fixed with persist.sys.phh.samsung_fingerprint=0
[2] Requires SIM to be in SIM1 slot. Multisim probably broken, but probably fixed with `setprop persist.radio.multisim.config dsds`