# [Honor 7A 2018](https://www.gsmarena.com/honor_7a-9075.php)
![Honor 7A 2018)](https://www.gsmarena.com/honor_7a-pictures-9075.php)

Device supported.

Devices tested:

* AUM-L29

**This device is A-only.**

## Known booting issues

* Bootloop on Android 9.0 GSIs **based on v127 below** (requires vendor patching to fix).
* Bootloop on all Android 8.x GSIs based on Phh-AOSP **v25 and above**.

## Hardware support

* Camera:
> Stock Camera app takes extremely dark images without flash, use a different camera app.

> Camera works on all Oreo GSIs

> Camera and/or flashlight **(not flash)** is broken on most Pie GSIs.

* SIM
> Works

> Certain GSIs may ask to reboot if a SIM card is removed (and inserted) while it's turned on.

* Wi-Fi
> Works

* Mobile Data/RIL
> Signal indicator is always empty on HSPA(P), regardless of real signal level **(you can still make calls, SMS/MMS, and use mobile data however).** Shows the correct level on 2G (E) and 4G (LTE). Refer to [this issue](https://github.com/phhusson/treble_experimentations/issues/272) for more information.

> Otherwise, it works. Phone calls loud and clear, SMS/MMS are sent and received on time, and mobile data works.

* GPS
> Works reliably on GSIs that include the AUM overlay.

* Mobile Tethering/Hotspot
> Works well on Oreo.

> Currently buggy on certain Android Pie GSIs.

* Fingerprint Reader
> Tested working on AUM-L29.

* Face unlock
> Works with Google Face Unlock

* Fast charging
> Non

## Installation process

A list of working ROMs for the Honor 7A (2018) are available [here (XDA)](https://forum.xda-developers.com/huawei-y6/development/index-list-roms-y62018-t3854167)

### Prerequisites:

* Stock Android 8 (Oreo) (tested from AUM-L29 8.0.0.154)
* Bootloader is unlocked

### Installation steps:

1. Backup everything in the internal storage. This will also get wiped when you perform a factory reset.
2. Perform factory reset using **eRecovery/stock recovery**.
3. Install GSI image using fastboot as described on XDA.

### Superuser (root, Magisk only):

* A way to root the device (if not present) is available [here (XDA)](https://forum.xda-developers.com/huawei-y6/development/root-magisk-huawei-y6-2018-root-atomu-t3853511)

> This may not work on other custom kernels (only tested with stock kernel)

> **NEVER install any Magisk module or you will bootloop.**



Template created by @zguithues