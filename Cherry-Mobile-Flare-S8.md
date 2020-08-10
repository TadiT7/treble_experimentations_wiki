# Device Info

- Name: Cherry Mobile Flare S8 (X930)  
- Architecture: arm64
- System partitions: a/b system partition
- System-as-root: Yes
- Stock Android Version: 9

## Steps to install
Refer to XDA Thread
https://www.xda-developers.com/flash-generic-system-image-project-treble-device/

*Some info*

- This device has a pre-installed Google Android 9 as Factory Version from Qiku [OEM]
- In order to root, you may have to manually install magisk manager then patch the stock boot image of your device and then, flash it through your PC. You can use the ADB (Android Debug Bridge)(Required Unlock Bootloader) Method or the SPFT (SP Flash Tool) Method.
- ROMs that didn't work are MIUI 10 or 11, Oxygen OS, One UI and Siberia OS. (What do you expect? Those are heavily-modified ROMs only for Manufacturers :P)
- If you are having difficulties modifying your device, don't forget to join our Facebook Groups here [Main Group](https://www.facebook.com/groups/746336425785682) and [Development Group](https://www.facebook.com/groups/468424323767473)
- Don't forget to hit the subscribe button and ring the bell in Alfredo Cortez' YouTube Channel, [here](https://www.youtube.com/channel/UCzpW0hWPTSkPzqzVgZ-5bjg)
- Visit the [XDA Thread](https://forum.xda-developers.com/android/development/guide-cherry-mobile-flare-s8-rooting-t4133827) for more infos regarding on how to unlock the bootloader, rooting the device, etc.
- Visit this [XDA Thread](https://forum.xda-developers.com/android/development/recovery-twrp-3-4-0-cherry-mobile-flare-t4145129) for a list of TWRP builds compiled by different developers.

*Note*

- Starting in the Security Patch (2020-03-05), many GSI images are having trouble booting up because of its OEM restricting GSI images to fully write in the system partition. The solution is to downgrade to Security Patch (2019-12-05) by flashing its firmware using SP Flash Tool. Always Un-tick Preloader LK1 and LK2 for the new batch of Flare S8 in October 2019
- There's also a problem where the screen goes black (No Display Issue), it is because of the LCD Drivers are being mismatched in the new batch,

## Hardware support

| Component                 |      Pie                             |              10                |
|---------------------------|--------------------------------------|--------------------------------|
| Camera                    | Working                              | Working                        |
| Speaker / Mic             | Working                              | Working                       |
| Bluetooth                 | Working                              | Working                       |
| WiFi                      | Working                              | Working                       |
| SIM / Mobile Data / Voice | Working                              | Working                       |
| Offline Charging          | Working                              | Working                       |
| Magisk                    | Working after patching boot image | Working after patching boot image |
| Root (phh-su) | Working | Working |
| Adoptable Storage         | Working                              | Working                       |
---

*TWRP Builds (Compiled by Alfredo Cortez and Hadenix)*

- For Oct 2019 Security Patch: [Download Link](https://drive.google.com/file/d/1-05l9vfdq-jcn3CqjeNOkOyAqnBEJyvU/view?usp=drivesdk)
- For Dec 2019 Security Patch: [Download Link](https://drive.google.com/file/d/1-xmMRWiHw_PsFFX0g5z6eGTozuEE44RH/view?usp=drivesdk)
- For October and December (Also Working in March 2020): [Download Link](https://drive.google.com/file/d/1-8OxY5HaOECEVhJSpvXMZD9AFyLvxsWO/view?usp=drivesdk)
- For July 5 2020 Security Patch: [Download Link](https://drive.google.com/file/d/1-CcQM4s_7UloUbA5HJN8bru7kw_jSaTG/view?usp=drivesdk)

*PBRP Builds (Source-built by @lovelyz)*

- PitchBlack Recovery: [XDA Thread](https://forum.xda-developers.com/android/development/recovery-pbrp-3-0-0-cherry-mobile-flare-t4145107)

*OrangeFox Builds (Source-built by @lovelyz)*

- OrangeFox Recovery: [XDA Thread](https://forum.xda-developers.com/android/development/experimental-orangefox-recovery-project-t4145125)

Credits 
- @AljunCortez: The first one who started the development of Flare S8 in the Community
- @Hadenix: For compiling some of the TWRP builds
- @androidist1204: For improving this thread and for supporting the development community
  
Tested ROMs:
- [Android 10] CAOSP
- [Android 10] Lineage OS 17
- [Android 10] Lineage OS 17.1
- [Android 10] Stag OS
- [Android 10] AospExtended 7.0
- [Android 10] MSM Extended
- [Android 10] Legion OS
- [Android 9/10] Havoc OS
- [Android 9/10] Evolution X
- [Android 9] Bootleggers ROM
- [Android 9] Descendant OS 4.0
- [Android 9] Resurrection Remix OS
- [Android 9] Syberia OS
- [On-Testing] Umidigi A7 Pro

Notice: GSI images are now working in the 2020-03-05 (March 2020) Security Patch.
        
Template created by @zguithues and @hackintosh5