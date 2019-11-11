# Samsung Galaxy A50 (Exynos)

**Samsung Galaxy A50 (SEE) (SM-A505FN/DS Exynos) Quack Compatibility Report (Android 10 v203)**

**What works out of the box:**
- RIL (network)
- Mobile data (4G+/4G, 3G)
- WiFi (5GHz and 2.4GHz)
- Internet Access
- Calls (incoming and outgoing, both 2G and 3G)
- SMS (incoming and outgoing, auto network switching)
- Touch screen
- Audio while playing accelerated video
- H264 video acceleration
- YouTube app
- SD Card
- Root on GSI
- Camera (both front and back)
- Audio recording in camera
- Video recording in camera
- SIM Toolkit
- Chrome
- Double tap to wake (in Samsung settings of Treble-App)

**What works with fixes:**
- Smooth animations (see https://gist.github.com/milankragujevic/7ec6d3bffbc56fd36b9291471caa9f04)
- Notch (requires overlay, push https://projects.milankragujevic.com/a505fn/treble-overlay-samsung-a50.apk into /system/overlay/)

**What doesn't work:**
- Fingerprint reader
- Dual SIM (SIM2 doesn't appear)
- Power management (battery lasts 6 hours max., phone is often hot)
- Auto brightness
- Proximity sensor (??? not enough testing)
- MTP (crashes Nautilus or Explorer on PC's side)
- VoLTE

**What needs more testing:**
- Bluetooth (maybe?)
- NFC (so far it reads my work access card and bus card)

Notice: Testing was done after flashing phh-magisk. I am unsure if the phone would work without it, as I haven't tried it.

## Steps to install

- Unlock bootloader
- ??? (somehow avoid RMM state Prenormal)
- Wipe data from stock recovery
- Flash TWRP (https://forum.xda-developers.com/galaxy-a50/development/recovery-twrp-galaxy-a50-t3916199)
- Boot directly into TWRP
- Format Data
- Reboot into TWRP
- Flash multidisabler
- Flash phh-magisk
- Flash SYSTEM (system-quack-arm64-ab-gapps.img)
- Modify build.prop to fix animations
- Push overlay
- Reboot into OS with adb (rebooting into OS from TWRP menu may cause the NAND chip to be erased, because of a bug)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works completely                                          |
| Speaker / Mic             | Works completely                                          |
| Bluetooth                 | Untested, sees other devices                              |
| WiFi                      | Works, both 5GHz and 2.4GHz                               |
| SIM / Mobile Data / Voice | Works on SIM1                                             |
| VoLTE                     | No                                                        |
| Fingerprint               | No                                                        |
| NFC                       | Yes                                                       |
| Offline Charging          | Yes                                                       |
| Dual SIM                  | No                                                        |
---

Tested By: milankragujevic - SM-A505FN/DS(SEE), A505FNXXS2ASJ1 - 10.11.2019. - Template created by @zguithues and @hackintosh5