# Gigaset GS290 (k63v2_64_bsp)

Seems to work great. 

## Steps to install

1.  This has been tested coming from OEM Android 10 stock ROM firmware
2.  Check that you have a recent version of fastboot on your local computer: `fastboot --version` should give version >= 29
3.  Get `vbmeta.img` from [https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img) __only for devices that came with Android 10 from the FACTORY (I don’t need this)__
4.  Get A/B GSI (for this phone, `arm64-ab-...` — the [Treble Info app](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck&hl=en&gl=US) can provide this information) from [https://github.com/phhusson/treble_experimentations/releases](https://github.com/phhusson/treble_experimentations/releases). There are various versions. I am using the version that comes with Free and Open Source apps: [system-roar-arm64-ab-floss.img.xz](https://github.com/phhusson/treble_experimentations/releases/download/v313/system-roar-arm64-ab-floss.img.xz). There is also a version without apps and a version with Google apps.
5.  Uncompress it with `unxz system-*.xz`
6.  From running Android, do `adb reboot bootloader`
7.  When the device is in the bootloader, run `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img` **only for devices that came with Android 10 from the FACTORY (I don’t need this). I need instead:** `fastboot --disable-verity --disable-verification flash boot boot.img` (using `boot.img` from the extracted OEM [stock ROM firmware](https://www.androidfilehost.com/?fid=17248734326145687642) zip)
8.  Reboot the phone with `fastboot reboot fastboot` .
9.  When dropped to a recovery menu, select “Wipe data/factory reset” and confirm
10.  Select “Reboot to bootloader”. It actually reboots to fastboot mode
11.  (Needed?) `fastboot erase system`
12.  Flash the system partition with `fastboot flash system system-...img`
13.  `fastboot reboot`
14.  Seeing Donald Duck bootlogo
15.  Enjoy PHH-Treble

### Notes

* To enter the recovery, power down the device. Hold the down + power keys
* To enter the recovery menu and/or fastboot: If the recovery menu does not show a menu ("No command"), press up + power keys together quickly repeatedly a couple of times (10 times or more)

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works, both front and rear                                |
| Speaker / Mic             | Works                                                     |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Untested                                                  |
| VoLTE                     | Untested                                                  |
| Fingerprint               | Untested                                                  |
| NFC                       | Works                                                     |
| Offline Charging          | Untested                                                  |
| GPS                       | Works                                                     |
| Other feature             |                                                           |
---
