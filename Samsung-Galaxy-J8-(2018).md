# Samsung Galaxy J8

Summary of what works and doesn't

Works by default
Camera(Only 1 of them though , secondary for live focus thing on stock is disabled)
Speaker / Mic,Bluetooth,WiFi , SIM / Mobile Data / Voice ,VoLTE,Offline Charging work (on android 10 vendor , on android 9 vendor offline charging works but you gotta reboot phone with holding down all keys for it to not be stuck on charge logo )

Works after installing patches
Lockscreen security(pin,password,graphic key) and fingerprint sensor

DOES NOT WORK
MTP

## Steps to install
To install gsi you need 
1. UNLOCKED BOOTLOADER ( THIS MANUAL WILL PRESUME YOU GONE AHEAD AND ALREADY DID THIS)
2. ALWAYS KEEP STOCK FIRMWARE FILES ON YOUR PC - IF YOU MESS UP EVEN 1 STEP OF THIS MANUAL - YOU MUST REFLASH STOCK
___
Depending on your vendor you must use twrp either from https://forum.xda-developers.com/android/development/recovery-twrp-3-3-1-0-galaxy-j8-j810m-f-t3962423 (android 9 ) or https://sourceforge.net/projects/samsung-j8y18lte/files/TWRP/ for android 10
1. Dowloand odin 3.14.4 for android 10 or if you have android 9 odin 3.13.3
2. Flash appropriate for your vendor twrp with auto-restart disabled
3. Format Data in wipe menu( Not factory reset )
4. Install AnyKernel3-j8y18lte-goldfish07.zip from android 10 twrp link ( its basically a combined together encryption and dm-verity disabler)
5. Install magisk , and reboot into system - and complete first setup wizard
6. Dowloand the gsi you picked and reboot into twrp
7. Make an advanced wipe in twrp of   “Dalvik / ART Cache”, “System”, “Data”, and “cache”
8. In the install menu in twrp select install image - and select the gsi image that you  downloaded , set as system image and install
9. Flash AnyKernel3-j8y18lte-goldfish07.zip, Disable-Force-Encryption-Treble.zip
10. Optionally flash tryfix_j8_lockscreen.zip


## Hardware support

| Component                 |      Comment                                                   |
|---------------------------|----------------------------------------------------------------|
| Camera                    | Status   Works                                                      |
| Speaker / Mic             | Status   Works                                                 |
| Bluetooth                 | Status   Works                                                 |
| WiFi                      | Status   Works                                                 |
| SIM / Mobile Data / Voice | Status   Works                                                 |
| VoLTE                     | Status   Works                                                 |
| Fingerprint,lockscreen    | Status   Needs fingerprint sensor patch for working            |
| Offline Charging          | Status   On android 10 vendor - fine, on android 9 vendor gets  stuck on charge logo        |                                           
---