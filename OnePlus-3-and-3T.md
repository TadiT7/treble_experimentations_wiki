## The step-by-step guide on how to treblize your device:

Treble needs a partition called "Vendor", but our device does not have this device. What we need to do is to create a vendor partition by our selves.
I made a custom TWRP Treble build to do this process, here is what you should do in TWRP.
1. Flash this TWRP in the download link below.
2. Boot it up and go to "Advanced" -> "Terminal", Type treblize and run.
Treblize is a shell that we could modify our partition. It basically does the same thing as the commands below.
Code:
  ```
  /sbin/sgdisk --typecode=5:8300 /dev/block/sdf
  /sbin/sgdisk --change-name=5:vendor /dev/block/sdf
  ```
3. Reboot your phone to your current system to check if there is storage failure.
It's very important. Some of the users report it may cause storage broken. You'd better check it first before flashing LOS Treble.
4. Reboot your phone to TWRP.
5. Flash LOS Treble in the download link below.
After these processes, you have got a treblized Oneplus3. Boot it up to check if everything works, or just trying other GSIs anyway.

## The step-by-step guide on how to flash GSIs:
1. Choose and flash LOS Treble solution first for the vendor partition.
Because of the supporting of system-as-root for our device, you can now use every GSIs if possible. I personally recommend the system-as-root solution for future android standards, although they are basically the same some old recovery install scripts may be broken like opengapps will not working anymore according to the report.
2. Flash A-only or A/B GSI image according to the flag in the download section.
3. Wipe data.

## Downloads:
* [New][A/B] LineageOS 16.0 Treble system-as-root: https://mega.nz/#F!UgdQRYSD!8s-_u2HJQZDEqNnFOnejxQ
* [Old][A-only] LineageOS 16.0 Treble: https://mega.nz/#F!A0VmQAaC!Mc3HYZgAkxeoQwGkZyJvwg
---
## Hardware support
| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (with [linker fix](https://github.com/OP3Treble/linkerfix) to load shims)|
| Speaker / Microphone      | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Device supports VoLTE, but can't test at this moment      |
| Fingerprint Reader        | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | N/A                                                       |

## Things not working:
* [A-only & A/B] SELinux is set to permissive for most GSIs.
Unnecessary and won't fix for now.
* [A/B] Reboot and stuck at boot animation while GSI installation.
Solution: Use adb for a reboot, don't just hold the power button. After this the system will boot, at least we could get console-ramoops correctly for debugging.
---

## Additional Notes
Works using this [Treble ROM](https://forum.xda-developers.com/oneplus-3/oneplus-3--3t-cross-device-development/treble-lineageos-15-1-treble-oneplus-3-t3830455)
***


## Tested By:
* [simonsmh](https://github.com/simonsmh) - Device Specifics - 19 July 2018
* Tested with the following builds:
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [EvolutionX 3.3](https://sourceforge.net/projects/developerluke-roms/files/GSIs/Evolution-X_3.3_20191111_ARM64-AB.img.xz/download)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [ResurrectionRemix P v7.0.3](https://sourceforge.net/projects/developerluke-roms/files/GSIs/RR-P-v7.0.3-20191112-ARM64-AB.img.xz/download)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [Dirty Unicorns v14.0](https://sourceforge.net/projects/developerluke-roms/files/GSIs/DirtyUnicorns-14.0_111119-ARM64-AB.img.xz/download)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [OxygenOS 9](https://mirrors.lolinet.com/firmware/gsi/OxygenOS/OxygenOS-AB-9-20191031-ErfanGSI.img-2108.7z)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [ResurrectionRemix Q v8.0.0](https://github.com/EnesSastim/GSI/releases/download/ErfanGSI/RR-Q-AB-10-20190911-ErfanGSI.img.7z)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [Pixel Experience 10.0](https://sourceforge.net/projects/developerluke-roms/files/GSIs/PixelExperienceQ-28102019-ARM64-AB.img.xz/download)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [AOSP 10.0](https://github.com/phhusson/treble_experimentations/releases/tag/v203) (system-quack-arm64-ab-gapps)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [OxygenOS 10](https://github.com/EnesSastim/GSI/releases/download/ErfanGSI/OxygenOS-AB-10-20190922-ErfanGSI.img.7z) with  [Permissiver_v5](https://androidfilehost.com/?fid=6006931924117940902) [Partly works]
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [AOSiP 9.0](https://sourceforge.net/projects/illusionproject/files/GSI/AOSiP-9.0-GSI-arm64_ab-20190819.img/download)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [ResurrectionRemix P v7.0.x](https://get.resurrectionremix.com/gsi/ARM64_AB_20191205.img)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [Descendant 4.0.1](https://github.com/Descendant/InOps/releases/download/4.0.1/Descendant_4.0.1_arm64_ab.zip)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [crDroidAndroid v4.4](https://androidfilehost.com/?fid=5862345805528041177)
    * [M6R1ARTY](https://github.com/M6R1ARTY) - A3010 - [LineageOS 15.1](https://github.com/phhusson/treble_experimentations/releases/tag/lineage-v21) (system-arm64-ab-gapps-su)

Template created by [zguithues](https://github.com/zguithues) and [simonsmh](https://github.com/simonsmh)