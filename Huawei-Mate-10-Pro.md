# Huawei Mate 10 Pro (Blanc)

## Testers

* [Jim-Bar](https://github.com/Jim-Bar)

## Hardware

Has been tested on:
* Blanc BLA-L09 128Go

## GSI tested

[phh](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) and [LineageOS](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/lineage-phh-treble-t3767690). Both work.

## Procedure used

This [post on XDA](https://forum.xda-developers.com/mate-10/how-to/guide-treble-compatible-rom-t3761927) and this [guide](https://gist.github.com/Jim-Bar/37066cb916ec6044e9ec2a8d931cc6fb) may be of some help.

1. Perform a factory reset
2. Reboot to fastboot, then flash the image: `fastboot flash system-arm64-aonly-vanilla-nosu.img` (phh v20 2018-06-07, sha256: `b4e08bedeaf6051159c3f4158320a546c866ac04f86cea8845016ac0843ff94a`) or `fastboot flash system-arm64-aonly.img` (LineageOS v4 2018-05-19, sha256: `6b05046d024902bf8ebcdbea91d6e70113438eafe4fad432901ef75a8755ec08`)
3. Boot the phone. It will boot several times then ask if a factory reset must be performed because it fails to boot
4. Perform the suggested factory reset
5. **Unplug the USB cable from your phone** (it prevents the phone from booting). It should now complete the boot

## Notes

Refer to the thread on XDA for a status of what is working and what is not.