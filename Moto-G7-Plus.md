# Moto G7 Plus

# Android 10 Q

  Some GSI ARM64 android 10 are starting, others are in bootloop.

# Android 11 R

 Android 11 R DP2 is bootloop. Android 11 R DP1 is untested.

---

## Steps to install with twrp

* Decryption is not required, but it's recommended
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

## Steps to Decryption

* On twrp wipe > Format Data > yes

* Download [DM-VERITY, FORCED ENCRYPTION, AND DISC QUOTA DISABLER
](https://zackptg5.com/android.php#disverfe)

* Push Decryption to /tmp 
  ```
  adb push Disable_Dm-Verity_ForceEncrypt_03.04.2020.zip /tmp/ForceEncrypt_quota.zip
  ```
* On twrp install > /tmp/ > dm_verity_ForceEncrypt_quota.zip > Swipe to confirm Flash 

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Work                                                      |
| Speaker / Mic             | Work                                                      |
| Bluetooth                 | Untested                                                  |
| WiFi                      | Work                                                      |
| SIM / Mobile Data / Voice | Work                                                      |
| VoLTE                     | Not Work                                                  |
| Fingerprint               | Work                                                      |
| NFC                       | Work                                                      |
| FM Radio                  | Untested                                                  |
---

Tested By: Sirherobrine23 - XT1965-3 (Lake, RETBR), QPWS30.61-21-9 - 01/06/2020 - Template created by @zguithues and @hackintosh5