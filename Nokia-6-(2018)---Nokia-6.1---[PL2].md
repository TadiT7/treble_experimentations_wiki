## Hardware Support

- Boot: Ok
- Partitions (Data) : Ext4 supported
- Bluetooth: Ok
- WiFi: Ok
- Hotspot: Ok
- RIL - Phone - Data: Ok
- GPS: Ok
- Camera: Ok
- Camcorder: Ok [**No 4K video recording support**]
- MicroSD: Ok
- Accelerometer: Ok
- Compass: Ok
- Gyroscope: Ok
- AOSP sensors: Ok
- Touchscreen: Ok
- FM Radio: **Unavailable**
- Fingerprint: Ok [**Fingerprint data gets lost on reboot on pre-Q firmware due to enforcing SELinux**]
- Vibrator: Ok
- Microphone: Ok
- Audio & music: OK on Pre-Q firmware [**No Audio from Notifications and Ringtones on Q firmware**]
- Bluetooth audio: **Broken**
- Kernel: Ok
- Graphics: Ok
- 3D Rendering: Ok
- Clock: Ok
- DRM: Ok
- Offline Charging: Ok [**Broken on pre-Q firmware due to init script changes required since Q**]
- USB: Ok
- USB OTG: Ok
- Encryption : Ok
- SEPolicies: Enforcing
- NFC: Ok [**Payment apps doesn't work**]

## Additional Notes

- This device uses AVB. Therefore, either a kernel with it disabled or a disabled vbmetaimage must be flashed to make the GSI images boot.

- All Nokia SDM660 based devices utilize the same kernel and vendor (almost). Kernel sources are available at [Official Website](https://www.nokia.com/phones/en_int/opensource). 

- TWRP is available at XDA. 

### Tested by

superium @ Nokia 6.1 @ 2018-06-30

AOSP 10: * Calyx Hikari (HikariCalyx) @ Nokia 6.1 TA-1050 00WW_4_060 (PL2-4060-0-00WW-B01) @ 05/11/2019

theimpulson@xda-developers

Template created by @zguithues