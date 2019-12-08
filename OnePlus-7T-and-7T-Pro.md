OP 7T (tested GApps + su version 203+204)
* boots Q, P does not boot.

working
* GSM network + LTE data
* WiFi
* Camera (also gcam)
* brightness (seems no auto brightness)
* BT
* Video playback

Not Working
* Fingerprint
* Headset: audio still comes out of speakers (USB c dongle)

Not yet tested
* NFC

How to install
* reboot to bootloader
* fastboot -w
* fastboot reboot fastboot
* fastboot erase system
* fastboot flash system <system.img>
* fastboot reboot recovery
* wipe *everything* in stock recovery
* reboot