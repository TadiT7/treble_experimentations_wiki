OP 7T (tested GApps + su version)
* boots 

working
* WiFi
* Camera (also gcam)
* brightness

Not Working
* Fingerprint

Not yet tested
* NFC
* BT

How to install
* reboot to bootloader
* fastboot -w
* fastboot reboot fastboot
* fastboot erase system
* fastboot flash system <system.img>
* fastboot reboot recovery
* wipe *everything* in stock recovery
* reboot