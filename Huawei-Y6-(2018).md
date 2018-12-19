# [Huawei Y6 (2018)](https://www.gsmarena.com/huawei_y6_(2018)-9162.php)
![Huawei Y6 (2018)](https://cdn2.gsmarena.com/vv/bigpic/huawei-y6-2018.jpg)

Device **mostly** supported.

Feedbacks from Huawei Y6 XDA for the

* ATU-L42 (nafis5566@XDA)
* ATU-L22/L21 (iDecrypt@XDA)
* ATU-L21 ([xBrownieCodez](https://github.com/BrownieCodeException)@GitHub)

**This device is A-only.**

## Known issues

* Bootloop on **all** Android 9.0 (Pie) ROMs **// Higher than v108 working finally!!**
* Bootloop on AOSP 8.1 v25

## Hardware support

* Camera:
> Stock LineageOS/Google AOSP-based Camera app takes extremely dark images without flash, use a different camera app. Video recording may also not work on certain apps (e.g. Google Camera).

* SIM
> Works

> ROM may ask to reboot device if SIM card is removed (and inserted) while it's turned on.

* Wi-Fi
> Works

* Mobile Data/RIL
> Signal indicator is always empty on 3G (H/H+), regardless of real signal level (you can still make calls, however). Shows the correct level on 2G (E) and 4G (LTE).

> Otherwise, it works. Phone calls loud and clear.

* GPS
> **Mostly works.** It sees satellites and is able to determine precise location, but is not able to lock on any of them.

* Mobile Tethering/Hotspot
> Works. USB Tethering not tested.

* Fingerprint Reader
> **Tested working on ATU-L42.** Other variants not tested.

* Face unlock
> Works with Google Face Unlock

> Broken on Pie ROM's

* Fast charging
> Works

## Installation process

A list of working ROMs for the Huawei Y6 (2018) are available [here (XDA)](https://forum.xda-developers.com/huawei-y6/development/index-list-roms-y62018-t3854167)

### Prerequisites:

* Stock Android 8 (Oreo) (tested from ATU-L22 8.0.0.143)
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