# Samsung Galaxy J4+ (MSM8917) report
Tested by [SebaUbuntu](https://github.com/SebaUbuntu)

## Procedure
1) Start from clean stock One UI rom (so reflash it from Odin)
2) Install [TWRP and Encryption disabler](https://forum.xda-developers.com/galaxy-j4+/development/recovery-twrp-3-2-3-1-galaxy-j4-j415f-t3876876)
3) From TWRP, format /data, then wipe system, cache and dalvik
4) Install Pie or Q GSI from Phh releases
5) Flash custom kernel
 - [If you wanna install Pie GSI](https://forum.xda-developers.com/galaxy-j4+/development/kernel-phizero-kernel-j4-t3943817)
 or 
[If you wanna install Q GSI](https://drive.google.com/open?id=1OLGZ09e367s3ZD__B4eeCkPc7Sdl9g-p)
6) Flash [this](https://www.androidfilehost.com/?fid=6006931924117930007)
7) Install Magisk and/or Gapps as you wish
8) Reboot

## Report of Q GSI (v200.D)

### Hardware issues
- Everything related to 2D video rendering not working (3D working)
- MTP broken (only work SD card transfer, Internal memory does not)
- Sound volume can't be controlled, even with SELinux Permissive

Everything else works

## Report of Pie GSI (v119)

### Hardware issues
- None