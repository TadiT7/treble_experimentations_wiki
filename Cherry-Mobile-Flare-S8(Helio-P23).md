# Device Info

- Name: Cherry Mobile Flare S8 (X930)  
- Architecture: arm64
- System partitions: ab system partition
- System-as-root: Yes

## Steps to install
Refer to XDA Thread
https://www.xda-developers.com/flash-generic-system-image-project-treble-device/

*Some info*

- This device has a pre-installed Google Android 9 as Factory Version from Qiku [OEM] (No Specific OEM yet)
- To root, you may have to manually install magisk manager then patch the stock boot image of your device and then, flash it through your PC. You can use the ADB (Android Debug Bridge) Method or the SPFT (SP Flash Tool) Method.
- ROMs that didn't work are MIUI 10 or 11, Oxygen OS, One UI and Siberia OS. (What do you expect? Those are heavily-modified ROMs only for Manufacturers :P)
- If you are having difficulties modifying your device, don't forget to join our Facebook Groups here [Main Group](https://www.facebook.com/groups/746336425785682) and [Dev Group](https://www.facebook.com/groups/468424323767473)
- Don't forget to hit the subscribe button and ring the bell in Alfredo's YouTube Channel, [here](https://www.youtube.com/channel/UCzpW0hWPTSkPzqzVgZ-5bjg)

*Note*

- Starting in the Security Patch (2020-03-05), Many GSI images are having trouble to booting up because of its OEM restricting GSI images to fully write in System Partition. The solution is to downgrade to Security Patch (2019-12-05) by flashing its firmware using SP Flash Tool. Always Un-tick Preloader LK1 and LK2 for the new batch of Flare S8 in October 2019
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

*TWRP Builds (Compiled by Alfredo Cortez)*

- For Oct 2019 Security Patch: [Download Link](https://drive.google.com/file/d/1-05l9vfdq-jcn3CqjeNOkOyAqnBEJyvU/view?usp=drivesdk)
- For Dec 2019 Security Patch: [Download Link](https://drive.google.com/file/d/1-xmMRWiHw_PsFFX0g5z6eGTozuEE44RH/view?usp=drivesdk)
- For October and December (Also Working in March 2020): [Download Link](https://drive.google.com/file/d/1-8OxY5HaOECEVhJSpvXMZD9AFyLvxsWO/view?usp=drivesdk)

Credits 
- @AljunCortez: The first one who started the development of Flare S8 in the Community
- @androidist1204: For improving this thread and for supporting the development community
- DC Salinas Sumcio: For allowing Custom ROM Development in the Community
  
Tested Roms:
- [Android 10] CAOSP
- [Android 10] Lineage OS 17
- [Android 10] Lineage OS 17.1
- [Android 10] Stag OS
- [Android 9/10] Havoc OS
- [Android 9] Bootleggers ROM
- [Android 9] Descendant OS 4.0
- [Android 9] Resurrection Remix OS
- [Android 9] Syberia OS
        
Template created by @zguithues and @hackintosh5