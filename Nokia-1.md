# [Nokia 1] - [frt]

[OEM's support](#oems-support-vendor-and-kernel)

[Android's support](#android-raw-build-support)
# Android RAW build support
## Overview

> These Android builds only works and works best with 00WW_0_39L up to 00WW_1_550.

> It would probably works with Android 9's Vendor/Kernel too if there is System-as-Root build for ARM-A phones. But the screen probably will not work since it blanked out in Android 8.1's last Maintain release (00WW_1_550_SP1, not 00WW_1_550).

## Common bugs in All builds
~~- Builds with Google Play Services crashes a lot. Install OpenGapps with the vanilla builds to fix this.~~ (Only true with older builds)

~~- You should skip setup wizard because it takes a lot of time to complete.~~ (Edit the gapps properly and this won't happen again)

~~- Fake allowed SMS permissions.~~ (Edit the gapps properly and this won't happen again)

- Please edit the device fingerprint property in /system/etc/prop.default, /system/build.prop, /vendor/default.prop and /vendor/build.prop so it would not make Google apps freaks out that your phone loaded with "Unofficial" build.

- TWRP formats the /data in ext4. While we need f2fs to make system work. Only use Stock Android recovery or "fastboot -w" (Only works when bootloader unlocked) can wipe the phone's user data properly.

- USSD incoming message without replies will get fixed in Android 9.
- Wi-Fi hotspot always broken (Android 9+).

- No 1st SIM incoming calls though.

## Android 10
- Very unstable.
- Wi-Fi will kinda hang system.
- Don't set a lock screen. Will hang system and no password has been set after that.
- Video codec kinda broken (As seen in Google's looped static videos in Pixel Setup Wizard, Gesture settings illustration video)
## Android 9
- Not sure. But there's a point of time where I can make Wi-Fi hotspot works with Android 9. But currently, it will not work.
- Used to has storage limitation to be flashed with v107. So far can flashed with v119 (With no built-in gapps of course).
## Android 8
- Nothing, except OEM's? Though it's literally Android 8.1 so this one will get the best compatibilty.


# OEM's support (Vendor and Kernel)
## Overview
> Build since 00WW_1_550_SP1 will break the screen.
## Build since 00WW_0_39L and above (Android 8.1)
> Won't mention the perfectly working features or known bugs (See older builds below).

| Component                 | Is it working?                                                                                          |
|---------------------------|---------------------------------------------------------------------------------------------------------|
| SIM / Mobile Data / Voice | ✓/✕                                                                                                     |

Bugs that automatically fixed in newer Android or Vendor builds:
- The RIL works fine again in any Android. Except some quirks like in known bugs. (Vendor)

Known bugs/Workarounds:
- MediaTek's DocumentsUI overlay (/vendor/overlay) will not hide the Files app anymore.
## Build since 00WW_1_33A and up (Android 8.1)

| Component                 | Is it working?                                                                                          |
|---------------------------|---------------------------------------------------------------------------------------------------------|
| Camera                    | ✓                                                                                                       |
| Speaker / Mic             | ✓                                                                                                       |
| Bluetooth / Hotspot       | ✓                                                                                                       |
| Wi-Fi                     | ✓                                                                                                       |
| Wi-Fi Hotspot             | ✓/✕ (Gapps somehow broke it in Android 9)                                                               |
| USB Tethering             | ✓                                                                                                       |
| SIM / Mobile Data / Voice | ✓/✕ (No signal on SIMs, modem software crashes, LTE/WCDMA broken)                                       |
| VoLTE                     | ✕ (Can't confirm it will work or not)  			                                                      |
| Thermal Sensors           | ✕ (For example: Battery's temp, Battery's voltage) 										              |
| GPS				        | ✓                                                                                                       |
| Camera		            | ✓/✕ (Low light on Camera2 app)                                                                          |
| Adaptive Brightness		| ✕                                                                                                       |
| Night lights      		| ✕                                                                                                       |
| Doze screen       		| ✕                                                                                                       |
| Screen            		| ✓                                                                                                       |

Bugs that automatically fixed in newer Android:
- The RIL works fine again in Android 10. Also true with Network band. Except some quirks like in known bugs.

Known bugs/Workarounds:
- MediaTek's DocumentsUI overlay (/vendor/overlay) will hide the Files launcher app. It also break Files app when trying to show Internal Storage. Delete it.
- Secure boot: Broken in Android 9 and up. For Android 9 will sort of works properly while Android 10 will broken completely (And don't even try to upgrade the OS from Android 9. It won't work and will ask you for "non-existent password".
)
- In Android 9. If you pre-lock and enabled lock on boot and happen to enter the wrong password in the first place. System will forced you to press Reset Phone button because you entered the wrong password "too much". Reboot the phone and try again.
- You can't set any form screen locking in Android 10.
- RIL modem: No 1st SIM incoming call, 2nd SIM as Data SIM/LTE (2G only). No proper network band selecting.
- Prelocking SIM with a PIN will make the phone bootlooped in the initial setup process.
- Wi-Fi in Android 10: Probably unstable.
- Wi-Fi Hotspot in Android 9+: Can't figured out yet. But at least Android 10 won't freak out the OS and soft reboot.
- Booting into Android causes screen went out for a few secs.
- The phone will reboot a few times after reboot (Sometimes, not always).
- For Adaptive Brightness, Night Lights, Doze Screen. You need to edit the framework-res or make an overlay app overlays framework-res to enable them in res/values.xml.
- Flashing a very different Vendor/Kernel will make Bluetooth crashes.
- Camera: Low light in newer Camera2 app. Use Android 6 or 5's Camera2. Or Google Camera from 2.7 or 2.4 (Android 9+). This feature slowly broken in newer Android incrementals.

## Tested by:
- Kutiz w/ Nokia 1 (TA-1047 Dual-SIM)

## Tested builds:
- Android 8.1 build v26 w/ Google apps and OpenGapps.
- Android 9.0 build v107 w/ no Google apps and OpenGapps.
- Android 9.0 build v119 w/ no Google apps and OpenGapps.
- Android 10 build v200.d w/o Google apps and OpenGapps

_**Last update:** 8:40 PM; November 20th, 2019_