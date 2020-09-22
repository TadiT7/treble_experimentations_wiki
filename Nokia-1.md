# [Nokia 1] - [frt]

[OEM's support](#oems-support-vendor-and-kernel)

[Android's support](#android-raw-build-support)
# Android RAW build support
## Overview

> These Android builds only works and works best with 00WW_0_39L up to 00WW_1_550 Vendor/Kernel builds.

> It would probably works with Android 9's Vendor/Kernel too if there is System-as-Root build for ARM-A phones (Husson suggests using ARM-AB variant, not tested). But the screen probably will not work since it blanked out in Android 8.1's last Maintain release (00WW_1_550_SP1, not 00WW_1_550).

## Common bugs in All builds
~~- Builds with Google Play Services crashes a lot. Install OpenGapps with the vanilla builds to fix this.~~ (Only true with older builds, or use a Go build)

- You should skip setup wizard because it took a lot of time to complete the "additional" installations.

~~- SMS permission is allowed for Google Play Services app by default but it was faked to be allowed and need to manually switch on/off in settings.~~ (Edit the gapps permissions properly and this won't happen again)

- Edit the device's fingerprint property in /system/etc/prop.default, /system/build.prop, /vendor/default.prop and /vendor/build.prop to stop Google screaming out that this ROM isn't a legit ROM.

- TWRP formats the /data folder in ext4. While we need f2fs to make system work. So only Stock recovery or "fastboot -w" (Only works when bootloader unlocked) can wipe the phone's user data properly.

- USSD incoming message without replies will get fixed in Android 9. (It is completely fixed)

- 1st SIM slot will never get incoming call notification. Android will ignore it completely. (Other mtk-based device do not have this bug or it was already fixed)

## Android 10
- Very unstable.

~~- Wi-Fi will kinda hang system. Sometimes will not work at all.~~ (Maybe older builds suffers this)

~~- Quickstep/SystemUI lock screen will hang the system and shows blank screen with System UI bar after a long while (Usually overnight sleep).~~ (Older builds only)

- Don't set a lock screen. Will hang system and no password has been set after that (Encryption issues). That means you can't even use your existing user data from Android 8.1 or 9 to upgrade it. It will ask for Non-existent password when done with the upgrade. So backup before doing stuff.
- Video codec is kinda broken (It will stutters and will not play the video smoothly or properly. For example, Settings/Setup wizard illustration videos.)
- If you happen to get a Soft-reboot, modem software will never work again until a full reboot is initiated.
## Android 9
~~-Wi-Fi hotspot will always broken with any form of Google Apps installed. In older builds without Google Apps it would work, but newer builds will completely break this feature. (Except Android 8.1 has the Wi-Fi hotspot working perfectly. Android 10 will have some sort of problems with Wi-Fi or Wi-Fi tethering)~~ [Because there used to be no Go variant builds so out of the box, Wi-Fi hotspot is not working properly when you're attempting to install GMS on it manually. But since there is now. This is not true, it will work fine, even with Android 10 too.]

- Used to has storage limitation to be flashed with v107. So far can flashed with v119 (With no built-in gapps).
- Technically you can downgrade 9 to 8.1. But you can't get pass the lock screen. Because keyguard won't respond to your touches.
- FRP lock doesn't work correctly (Tested with Google Pixel 1 Setup Wizard). It only unlocks with your Google Account.
## Android 8
- Nothing, except some quirks like lacking internal thermal values like battery capacity (edit framwork-res\xml\power_profile.xml) or its health and voltage? Though it's literally Android 8.1 so this one will get the best compatibility.


# OEM's support (Vendor and Kernel)
## Overview
> No tests has been made for newer Android 9 and 10 builds. Sorry.
> Build since 00WW_1_550_SP1 (Android 8.1) will break the screen. Still works though.
> Build 00WW_1_550 (Last Maintain Release of Android 8.1) will work the best of all Kernel/Vendor builds.
## Build since 00WW_0_39L and above (Android 8.1)
> Here is a compatibility list. It will not mention the perfectly working features or known bugs in newer table (See oldest build to learn more).

| Component                 | Is it working?                                                                                          |
|---------------------------|---------------------------------------------------------------------------------------------------------|
| SIM / Mobile Data / Voice | ✓/✕                                                                                                     |

"It fixed itself":
- The RIL works fine again in any Android. Except some quirks in known bugs. (Vendor)
- MediaTek's DocumentsUI overlay (/vendor/overlay) won't break Files app anymore.

## Build since 00WW_1_33A and up (Android 8.1)

| Component                 | Is it working?                                                                                          |
|---------------------------|---------------------------------------------------------------------------------------------------------|
| Camera                    | ✓                                                                                                       |
| Speaker / Mic             | ✓                                                                                                       |
| Bluetooth / Hotspot       | ✓                                                                                                       |
| Wi-Fi                     | ✓                                                                                                       |
| Wi-Fi Hotspot             | ✓/✕ (GMS broke this feature, if you know how to configure that you can fix this)                       |
| USB Tethering             | ✓                                                                                                       |
| SIM / Mobile Data / Voice | ✓/✕ (No signal on SIMs, modem software crashes, LTE/WCDMA broken)                                      |
| VoLTE                     | ✕ (Can't confirm it will work or not because VoLTE carriers doesn't support this at that time)         |
| Thermal Sensors           | ✕ (For example: Battery's temperature, Battery's voltage)					              |
| GPS			    | ✓ (You don't need to keep any MediaTek's app in vendor/app to get this working, because it will not installed anyway because it can't find mediatek's framework resources.)                                                                                        |
| Camera		    | ✓/✕ (Low light with Camera2 app. Use Google Camera 2.7 or 2.5. Note that 2.7 will have unsigned apk and broken settings. Even if you set it as a system app)|
| Adaptive Brightness       | ✓/✕ (Out of the box, this "feature" will be off in Android framework. Go to bool.xml and change "config_automatic_brightness_available" from false to true)|
| Night lights              | ✓/✕ (Same thing above but "config_nightDisplayAvailable" is true, forget the reference to "config_setColorTransformAccelerated")|
| Doze screen       	    | ✓/✕ (config_dozeAlwaysOnDisplayAvailable=true; config_dozeAlwaysOnEnabled=false (fail-safe because it will blank out the screen once you put in the pocket and you can't turn it on, even screen copy can't save this.); config_displayBlanksAfterDoze=false (same reason)|
| Screen            	    | ✓                                                                                                       |

"It fixed itself":
- The modem works fine again in Android 10. You can choose Network band in testing settings but there are still some quirks in known bugs.

Known bugs/Workarounds:
- Because this is a Go device, MediaTek created DocumentsUI overlay to hide System's files app away (/vendor/overlay) to prevent duplication from Google's Files app. It will break the actual system's files app once you clicked "Show internal storage" so you should delete it.
- Secure boot: Broken in Android 9 and up. For Android 9 will kinda work properly while Android 10 will be broken completely (And don't even try to upgrade the OS from Android 9. It won't work and will ask you for a "non-existent password".)
- In Android 9 (Maybe "and up" too if Android 10 fixed encryption thing). If you pre-lock and enabled lock on boot and happen to enter the wrong password in the first place. System will forced you to press Reset Phone button because you entered the wrong password "too much". Reboot the phone and try again.
- You can't set any form screen locking in Android 10. Even if it's a Swipe one.
- Phone modem: 1st SIM slot will never get incoming call and is the only slot that work as Data SIM with All networks like 4/3/2G. No proper network band selecting. 2nd SIM slot will only work as a Non data SIM with 2G only. Forcing system choosing this slot as data SIM will freaks out the modem software (com.android.phone) and it kept going back and forth switching SIM. Some early Android 9 builds will make the system hangs hard if you can't switch back sooner.
- Pre-locking SIM with a PIN will make the phone bootlooped while the phone is completing the initial setup process (First boot on a Boot Animation screen).
- Wi-Fi in Android 10: Probably unusable.
- Wi-Fi Hotspot in Android 9+: GMS broke it, not vendor's fault.
- Booting into Android causes screen went out for a few secs and the phone will reboot a few times after reboot (Sometimes, not always).
- Try to use the same Vendor/Kernel build. Different builds might cause hardware driver issues like Bluetooth will keep crashing.
- Camera: Low light in newer Camera2 app. Use Android 6 or 5's Camera2. Or Google Camera from 2.7 or 2.4 (Android 9+). You can't use 2.4 in Android 10, it will ask you to insert an SD card (while you obviously did) and you can't take photo or record videos. 2.7 built for Android 6 so it will have better compatibility with Android 10 with permission thing.

## Tested by:
- Kutiz w/ Nokia 1 (TA-1047 Dual-SIM)

## Tested builds:
- Android 8.1 build v26 w/ Google apps and OpenGapps.
- Android 9.0 build v107 w/ no Google apps and OpenGapps.
- Android 9.0 build v119 w/ no Google apps and OpenGapps.
- Android 10 build v200.d w/o Google apps and OpenGapps.
- Android 10 build v204.d w/o Google apps and OpenGapps.
- Android 10 build v222 Go variant on Revoview/Mobell S41.

_**Last update:** 8:34 PM; September 22nd, 2020_

_**There are tons of changes that I've found and saw them fixed with another Go device I own but please note that I am no longer owning the phone so I can't contribute anything here anymore. But overall, this is a bad phone to use GSI. Maybe it will get better in Android 11. Heck, I didn't even have opportunity to try Android 10 on this phone yet.**_