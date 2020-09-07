# Moto G7 Plus

# Android 10 Q

  Some GSI ARM64 android 10 are starting, others are in bootloop. by any chance the lock screen does not save any mode like: pin, password etc ... after decryption.

# Android 11 R

 Android 11 R DP2 is bootloop. Android 11 R DP1 is untested.

---

## Steps to install with twrp

* Download twrp image [twrp 3.3.1-0](https://twrp.me/motorola/motorolamotog7plus.html)
* boot this image with the `fastboot` utility:
    ```
    $ fastboot boot twrp-3.3.1-0-lake.img
    ```
* push twrp image for /tmp/
  ```
  $ adb push twrp-3.3.1-0-lake.img /tmp
  ```
* on twrp go to Advanced > Install Recovery Ramdisk> (Up A Level) > tmp > select the twrp image > Swipe to install

## Steps to install with fastboot

* Recommend adb/fastboot v1.4+
  ```
  $ fastboot flash system System.img  #For System_a
  $ fastboot flash system_b Other_System.img   #For System_b
  ```
---
## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work                                                      |
| Speaker / Mic             | Work                                                      |
| Bluetooth                 | Only phone call works, media not working                                                  |
| WiFi                      | Work                                                      |
| SIM / Mobile Data / Voice | Work                                                      |
| VoLTE                     | Not Work                                                  |
| Fingerprint               | Work                                                      |
| NFC                       | Work                                                      |
| FM Radio                  | Untested                                                  |
---

Tested By:
1. Username: **@Sirherobrine23**
   - Model: XT1965-3 (Lake, RETBR)
   - Vendor: QPWS30.61-21-9
   - Date: 01/06/2020

2. Username: **@nicomix**
   - Model: XT1965-2 (Lake, TIGCO)
   - Vendor: QPWS30.61-21-11
   - Date: 07/Sep/2020

Template created by @zguithues and @hackintosh5