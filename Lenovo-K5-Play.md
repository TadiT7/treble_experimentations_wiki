# AOSP 10
Flashed Android 10 A only variant with gapps and su. The device is booted successfully, but mobile data and camera is not working. Other features like fingerprint scanner or bluetooth work properly. Still as good as a daily driver if mobile network and camera is fixed.<br/><br/>
**Steps for installing** <br/>
Same as the procedure stated in Android Pie

Hardware support Component:

Camera	                   not working,

Speaker / Mic	              working,

Bluetooth	              working,

WiFi	                      working,

SIM / Mobile Data / Voice   not working,

VoLTE	                    not working,

Fingerprint	              working,

NFC	                      n/a,

Offline Charging	      unknown,

Other feature	              working,
 
Tested By: littlephone - K5 Play(L38011), ZUI 3.7.088 (GLOBAL VARIANT)

# AOSP 9
Flashed AOSP 9 with gapps and su, I flashed it over stock rom (Chinese variant), should work same way with global variant.
It booted fine, WiFi and hotspot doesn't work, testing fix soon. Every other thing works fine, camera is a bit dark but third party camera should fix it, no auto brightness overlay is needed to fix that, I don't really know how to compile one but I'll work on it.
The ROM is smooth and good as daily driver. (As far as WiFi and hotspot is fixed.)
**UPDATE**--- Wifi and hotspot works now. make sure to flash stock rom afresh, boot to fastboot immediately, wipe system with fastboot then flash GSI system.

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