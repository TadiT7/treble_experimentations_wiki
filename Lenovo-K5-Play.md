Device
It booted fine, WiFi and hotspot doesn't work, testing fix soon. Every other thing works fine, camera is a bit dark but third party camera should fix it, no auto brightness overlay is needed to fix that, I don't really know how to compile one but I'll work on it.
The ROM is smooth and good as daily driver. (As far as WiFi and hotspot is fixed.)

Steps to install
Step 1

Step 2

Step 3

flash this image with the fastboot utility:

$ a-command
$ fastboot flash system system-arm64-aonly-gapps-su.img
Some more info

As an alternative you can flash via TWRP as "System Image" and format data.

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