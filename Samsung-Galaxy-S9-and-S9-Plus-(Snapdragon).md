# Samsung Galaxy S9 and S9 Plus (Snapdragon)

There are a lot of things that are not working. I wouldn't rely on it as a daily driver.

## Steps to install

* For unlocked U.S. devices (SM-G960U and SM-G965U,) follow the instructions [here](https://forum.xda-developers.com/galaxy-s9/how-to/guide-install-gsi-s-snapdragon-s9-s9-t4044125).
* For international devices (SM-G9600 and SM-G965U,) follow the instructions [here](https://forum.xda-developers.com/galaxy-s9/how-to/guide-install-gsi-galaxy-s9-snapdragon-t3942302#:~:text=xda-developers%20Samsung%20Galaxy%20S9%20Samsung%20Galaxy%20S9%20Guides%2C,the%20look%20and%20feel%20to%20adding%20new%20functionality.).


## Hardware support
### G960U (Galaxy S9, U.S.)
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Rear camera functions, but front camera does not          |
| Speaker / Mic             | Speaker works, but headphone jack does not. Microphone untested. |
| Bluetooth                 | Untested                                                  |
| WiFi                      | Works on AOSP 9, Broken on AOSP 10                        |
| SIM / Mobile Data / Voice | Not working. Modem firmware is unstable on AOSP 9         |
| VoLTE                     | Not working                                               |
| Fingerprint               | Not working                                               |
| NFC                       | Untested                                                  |
| Offline Charging          | Not working, because boot and recovery partitions are swapped. |
---

Tested By: @NoodleFork - SM-G960U(USA), AOSP 9.0 v123 - AOSP 10 v213

## Additional Information
### G960U (Galaxy S9, U.S.)
An earlier version of this page states that:
>Everything work except brightness that is always at max and fingerprint and lockscreen that cant bee set, if try to set any tipe of lock systemui will crash after reboot

However, when using AOSP 9.0 v123, there appears to be no problems when controlling the brightness of the screen. Biometrics will not work, but setting up a PIN will work just fine. The headphone jack **does not** appear to work; the internal speakers will be used whether something is plugged in the jack or not.

As of AOSP 9.0 v123 and AOSP 10.0 v213, Mobile data is not working. On a phone from Spectrum Wireless, Wireless settings shows only an APN for Verizon (VZWINTERNET). Tapping "Mobile plan" shows the message "Verizon has no known provisioning website". FYI: Spectrum is an MVNO that uses Verizon's towers. On a phone from Sprint, Inserting a Sprint SIM card in the phone results in the software going haywire. The cell status would change rapidly from normal to Roaming. One could probably make a call if they were fast enough, but the Modem firmware kept crashing, resulting in the entire OS to halt abruptly.