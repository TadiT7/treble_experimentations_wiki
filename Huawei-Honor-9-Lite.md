Most stuff works fine except every 5 seconds there are some green lines on the camera and the brightness is stuck at 40% and can't be adjusted. I also can't get the play store to start a download. Steps to install: Unlock your bootloader using this guide: https://forum.xda-developers.com/honor-7x/how-to/how-to-unlock-huawei-bootloader-removal-t3780903

After that reboot to system, enable developer settings and disable FRP lock. Then reboot to recovery (it should tell you bootloader is unlocked and FRP is unlocked) and run these 2 commands: 
fastboot -w
fastboot flash system system-arm64-aonly-gapps-su.img

Then the device will bootloop 3 times. This is FINE! After the third boot the recovery tells you that the data partition has to be low level formatted. Click on okay and after that the device will boot just fine! :)

Hardware Support
Camera:
Front and back camera works fine, but every 5 seconds there are minor green lines. There is a screenshot of that posted on XDA

Speaker / Microphone
Speaker and microphone work fine

Bluetooth
not tested yet

Wifi
Wifi works fine

SIM / Mobile Data / Voice
not tested yet

VoLTE
I will not be able to test VoLTE

Fingerprint Reader
works fine

Additional Notes
Put any additional info/notes regarding treble support for this device.

Tested By:
kaiomatico - LLD-L31(C432, so a German Device), Firmware 8.0.0.128 - 05/03/2018
Template created by @zguithues