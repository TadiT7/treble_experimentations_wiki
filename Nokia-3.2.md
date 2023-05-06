# [Nokia 3.2] - [deadpool/DPL] [00WW variant]

## **WARNING!!! Backup all data before you proceed!**

If you are familiar with the procedure, please skip to [Post Install Tweaks section](https://github.com/phhusson/treble_experimentations/wiki/Nokia-3.2#post-install-tweaks). If not, proceed reading.

## Preparation

1. Make sure your phone has latest vendor upgrade using system updater.

   * For Nokia 3.2 (00WW variant) it's April 2022 final guaranteed update.

2. Download [vbmeta image](https://dl.google.com/developers/android/qt/images/gsi/vbmeta.img), mandatory for disabling verified boot (AVB) and flashing GSI images via `fastboot`.

3. Enable OEM unlocking and USB debugging under Developer options.
   * Authorize ADB on phone after executing `adb devices` from PC
   * Reboot device to fastboot mode with `adb reboot bootloader`



## Unlocking bootloader and flashing GSI

For Nokia 3.2 unlocking bootloader is simple as:

`fastboot oem unlock`

Reboot bootloader with `fastboot reboot fastboot` or do it manually on device fastboot screen (visible after unlocking).

Time to flash desired GSI. Let's disable AVB (Android Verified Boot) first:

`fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`

Next, erase system with `fastboot erase system`. 
Your stock ROM is gone - R.I.P. :)

Everything's (almost) ready for your new shiny GSI.
Flash it: `fastboot flash system your-new-system-here.img`

Now, go and wipe all the data associated with the previous system. If not wiped, this can cause booting issues or other problems.

Like this: `fastboot -w`. So long [unsaved photos, passwords...](https://github.com/phhusson/treble_experimentations/wiki/Nokia-3.2#warning-backup-all-data-before-you-proceed)

Lastly, execute `fastboot reboot` and wait for your new system to load.

## Post install tweaks


I tested two [Treble GSIs](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)
built by [eremitein](https://github.com/eremitein) - [CAOS11](https://github.com/eremitein/treble-patches/wiki/CAOS11-Project) and [crDRom11](https://github.com/eremitein/treble-patches/wiki/crDRom11-Project), both **bvZ-lite variants**. 

As far as I can tell after a year of daily use, the only initial glitch is sound.

  * _Note about naming GSIs. Click "Show content" in [this post](https://forum.xda-developers.com/t/official-aosp-r-mod-caos11.4265059/post-84873461)._



**Symptoms**: Wired/bluetooth earbuds or BT speakers not working.

**Remedy**: Upon first boot open _Phh Treble Settings_ and check the following boxes:
  * _Qualcomm features-->Use alternate audio policy_. Also _Disable sound volume effect_ IF you hear sound distortion.
  * -->_Misc features-->Audio-->Use alternate way to detect headphones_ 
  * -->_Other-->Force-disable A2DP offload_.


**Everything else just works.**

Enjoy!

***

P.S. Since the device comes with (by today's standards) modest 16GB/32GB storage and 2GB/3GB RAM,
you may consider installing crDRom11, which takes only 3.5 GB and is half size CAOS11.
Both are vanilla (no Gapps) and run smoothly on my test device with lower specs, 16GB/2GB RAM.
