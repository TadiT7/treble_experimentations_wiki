# Lenovo Smart Tab M8

TB-8505XS "With Google Assistant and SmartDock"

Not to be confused with **Lenovo Smart Tab M8 FHD** although the same installation procedure applies

A-only, but takes A/B roms due to system-as-root

Full 64 bit armv8

## Steps to install

* Recommended: Download the stock ROM, using for example [the official tool](https://pcsupport.lenovo.com/ph/sl/products/tablets/m-series-tablets/smart-tab-m8/downloads/driver-list/component?name=Software%20and%20Utilities) (registration required); in which case it will be stored in ```\ProgramData\LMSA\Download\RomFiles\\*\```.
* Unlock the bootloader:
    ```
    # after enabling unlocking in developer settings...
    fastboot flashing unlock
    # press volume+
    ```
* flash this image with the `fastboot` utility:
    ```
    fastboot flash --disable-verification --disable-verity vbmeta RomFiles\TB_8505XS_S300088_201220_BMP\vbmeta.img
    fastboot flash system system-roar-arm64-ab-vanilla.img
    fastboot erase userdata
    fastboot reboot
    ```

## Hardware support

### PHH AOSP 11.0 v300.m:

⚠️ Will bootloop if secure boot (enabled by agreeing to it while configuring a protected lockscreen) is not enabled

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| MicroSD                   | Working                                                   |
| WiFi                      | Working (802.11ac 5GHz)                                   |
| Bluetooth                 | Working (search, OBEX)                                    |
| Camera                    | Working (AOSP camera, photo & video)                      |
| Speakers                  | Working                                                   |
| Mic                       | Working (stereo sound unverified)                         |
| SIM / Mobile Data / Voice | Untested (IMEI detected)                                  |
| VoLTE                     | Untested (is it even supported?)                          |
| Wired headphones          | Working                                                   |
| Wired remote/mic          | Untested                                                  |
| ADB                       | Working                                                   |
| MTP                       | Working                                                   |
| OTG                       | Working                                                   |
| Dock + OTG                | Working                                                   |
| Offline Charging          | Broken (freezes on unlocked bootloader warning)           |
| Root                      | Working (PHH Superuser)                                   |
| First boot                | < 3 minutes                                               |

---

Tested By: Ryccardo (@rboninsegna) - TB-8505XS ZA5D0038SE (Swedish model sold in Italy), official firmware TB_8505XS_S300088_201220_BMP - 2021.2.16