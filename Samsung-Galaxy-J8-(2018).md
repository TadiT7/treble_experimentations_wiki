# Samsung Galaxy J8

Summary of what works and what doesn't

Works by default:
Camera (Only 1 of them though , secondary for live focus thing on stock is disabled)
Speaker / Mic, Bluetooth, WiFi, SIM / Mobile Data / Voice ,VoLTE, Offline Charging works (on Android 10 vendor , on Android 9 vendor offline charging works but you gotta reboot phone with holding down all keys for it to not be stuck on charge logo)

Works after installing patches:
Lockscreen Security (Pin, password, pattern lock and fingerprint sensor)
MTP

## Steps to install:
To install the GSI you need:
1. A UNLOCKED BOOTLOADER (THIS MANUAL WILL PRESUME YOU GONE AHEAD AND ALREADY DID THIS)
2. ALWAYS KEEP STOCK FIRMWARE FILES ON YOUR PC - IF YOU MESS UP EVEN 1 STEP OF THIS MANUAL - YOU MUST REFLASH STOCK
___
Depending on your vendor you must use TWRP either from https://forum.xda-developers.com/android/development/recovery-twrp-3-3-1-0-galaxy-j8-j810m-f-t3962423 (Android 9) or https://sourceforge.net/projects/samsung-j8y18lte/files/TWRP/ for Android 10

**1.** Dowloand Odin 3.14.4 for Android 10 (or if you have Android 9 use Odin 3.13.3)

**2.** Flash appropriate TWRP for your vendor with auto-restart disabled

**3.** Format Data in Wipe menu (Not factory Reset)

**4.** Install AnyKernel3-j8y18lte-goldfish07.zip from Android 10 TWRP link (It's basically a combined together encryption and dm-verity disabler)

**5.** Install Magisk, and reboot into system - and complete first setup wizard

**6.** Dowloand the GSI you picked and reboot into TWRP

**7.** Make an advanced wipe in twrp of   “Dalvik / ART Cache”, “System”, “Data”, and “cache”

**8.** In the install menu in TWRP select Install Image - and select the GSI image that you downloaded, set as System Image and install

**9.** Flash AnyKernel3-j8y18lte-goldfish07.zip, Disable-Force-Encryption-Treble.zip (https://t.me/galaxyj8/12863)

**10.** Optionally flash tryfix_j8_lockscreen.zip (https://t.me/j8_devlopment_group/1589) or UpstreamKernel-GSI-j8-goldfish07.zip (https://sourceforge.net/projects/samsung-j8y18lte/files/CustomKernel/GSI/) for MTP to work


## Hardware support:

| Component                 |       | Comment                                                   |
|---------------------------|-------|--------------------------------------------------------|
| Camera                    | Status|  Works                                                      |
| Speaker / Mic             | Status|   Works                                                 |
| Bluetooth                 | Status|   Works                                                 |
| WiFi                      | Status|   Works                                                 |
| SIM / Mobile Data / Voice | Status|   Works                                                 |
| VoLTE                     | Status|   Works                                                 |
| Fingerprint,lockscreen    | Status|   Needs flashing the Lockscreen and Fingerprint sensor patch to work            |
| Offline Charging          | Status|  On Android 10 vendor - fine, on android 9 vendor gets stuck on charge logo but still charges        | 
| MTP                       | Status|  Need to flash UpstreamKernel patch for GSI to work     |                                           
---