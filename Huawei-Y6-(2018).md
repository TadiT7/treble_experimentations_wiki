# [Huawei Y6 (2018)](https://www.gsmarena.com/huawei_y6_(2018)-9162.php)
![Huawei Y6 (2018)](https://cdn2.gsmarena.com/vv/bigpic/huawei-y6-2018.jpg)

Device **mostly** supported.

Feedbacks from Huawei Y6 XDA for the

* ATU-L42 (nafis5566@XDA)
* ATU-L22 ([TenSeventy7@XDA](https://github.com/TenSeventy7), pascua28@XDA)
* ATU-L21 (iDecrypt@XDA, [xBrownieCodez](https://github.com/BrownieCodeException)@GitHub)

**This device is A-only.**

## Known issues

* Bootloop on Android 9.0 GSIs **based on v127 below** (requires vendor patching to fix).
* Bootloop on Android 8.x GSIs based on Phh-AOSP **v25 and above**.

## Hardware support

* Camera:
> Stock Camera app takes extremely dark images without flash, use a different camera app. Video recording may also not work on certain apps (e.g. Google Camera).

> Stock camera crashes on Pie. **Use a different camera app.**

* SIM
> Works

> ROM may ask to reboot device if SIM card is removed (and inserted) while it's turned on.

* Wi-Fi
> Works

* Mobile Data/RIL
> Signal indicator is always null on HSPA(P), regardless of real signal level (you can still make calls, however). Shows the correct level on 2G (E) and 4G (LTE). Refer to [this issue](https://github.com/phhusson/treble_experimentations/issues/272) for more information.

> Otherwise, it works. Phone calls loud and clear.

* GPS
> Works.

* Mobile Tethering/Hotspot
> Works.

> Wi-Fi Hotspot currently broken on **all** Android Pie builds.

* Fingerprint Reader
> Tested working on ATU-L42.

* Face unlock
> Works with Google Face Unlock

> Broken on Pie ROMs with incompliant/incomplete Google Apps installations.

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


For information and support, please [visit this Telegram group.](https://t.me/HwAtomu_EN)


Template created by @zguithues