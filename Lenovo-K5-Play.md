Flashed AOSP 9 with gapps and su, I flashed it over stock rom (Chinese variant), should work same way with global variant.
It booted fine, WiFi and hotspot doesn't work, testing fix soon. Every other thing works fine, camera is a bit dark but third party camera should fix it, no auto brightness overlay is needed to fix that, I don't really know how to compile one but I'll work on it.
The ROM is smooth and good as daily driver. (As far as WiFi and hotspot is fixed.)

**Steps to install:**
Please follow this thread, it's more detailed.
[How to flash GSI image](https://www.google.com/amp/s/www.xda-developers.com/flash-generic-system-image-project-treble-device/amp/)

**Make sure everything is stock, no magisk or Xposed. boot, recovery e.t.c must be stock.**

**Step 1**
* Perform factory reset on your stock ROM (search how to do that if you don't know)

**Step 2**
* Reboot into fastboot (volume down key plus power key pressed down together and hold) and connect your device to pc

**Step 3**

Copy the GSI image to the adb folder and rename to "system.img"
flash this image with the fastboot utility:
Firstly type this command and press enter

`fastboot erase system`

Then

`fastboot flash system system.img`

Reboot your Device, should boot straight up. 
_If it ask for password to decrypt data, just type whatever, it will sort itself out_

Hardware support Component:

Camera	                      working,

Speaker / Mic	              working,

Bluetooth	              working,

WiFi	                   not working,

SIM / Mobile Data / Voice     working,

VoLTE	                      unknown,

Fingerprint	              working,

NFC	                      unknown,

Offline Charging	      unknown,

Other feature	              working,



Tested By: kingfeargod (mitcano7) - K5 Play(L38011), ZUI 3.7.088 (CHINESE VARIANT) - 20/03/2019.
Template created by @zguithues and @hackintosh5