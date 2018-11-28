# BV9500 Pro (MT6763)

## Testers

* [Jim-Bar](https://github.com/Jim-Bar)

## Hardware

Has been tested on:
* BV9500 Pro MT6763

## GSI tested

[Phh-Treble 8.1.0 v25](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) and [Phh-Treble 9.0.0 v107](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/aosp-9-0-phh-treble-t3831915). Both work to some degree.

1. Phh-Treble 8.1.0 v25 sha256: a2b0e2b5e236850f0c27bec1728eaa9796586800f94aead68600a14c341e88ad
2. Phh-Treble 9.0.0 v107 sha256: 2065a92d7e5cfdaa70eab7e86e21e2ce7b7f6560f1b089064b19ae020eb13e40

## Procedure used

**Warning:** there is no way to restore the phone back to its original state. I couldn't find the official firmware anywhere, and there is only one slot for each partition (not A/B).

**Warning:** unlocking the bootloader voids the guarantee **definitively**.

Tested on top of the version BV_BV9500Pro_V1.0_20180827_20180904-1729.

1. Reboot to fastboot (see below), then erase the system partition: `fastboot erase system`
2. Flash the system image: `fastboot flash system system-arm64-a-vanilla-nosu.img`
3. Erase the data partition: `fastboot -w`
4. Boot the phone: `fastboot reboot`
5. When rebooting, the mobile asks for a password. Enter anything, it will say the password is correct but the data corrupted, then suggest to wipe data. Do that, it will reboot fine next time.

## Entering the fastboot mode

**Warning:** unlocking the bootloader voids the guarantee **definitively**.

When the phone is powering on, press Volume Up until the screen displays "No command". Then press Power and immediately press Volume Up while holding Power. A menu is displayed in which you can choose to reboot to the bootloader.

It seems that there is a more direct way for entering the bootloader without passing by the recovery menu, but so far it has not been found. 

## Status of features

For both Phh-Treble 8.1.0 and 9.0.0:

1. The proximity sensor doesn't work (always in "close to" state). This result in a black screen during GSM calls
2. The GPS doesn't work
3. The mobile data doesn't work
4. The extra physical buttons have no effect

Everything else seems to work fine.