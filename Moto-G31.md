This device is kinda tricky to get working because of the super.img dynamic partition layout... Took me like 2 weeks of research to get everything working AFAIK

# Quick guide:

Toggle OEM Unlock in dev settings.
Do everything thats explained here until you get the unlock code [Unlocking Bootloader Motorola](https://motorola-global-portal.custhelp.com/app/standalone/bootloader/unlock-your-device-a/)

Get the vbmeta image from your stock ROM (I had to use the [Motorola Rescue Tool](https://www.motorola.com/us/rescue-and-smart-assistant/) because I couldn't find it anywhere else...)

Also this tool will be needed if we f*ck up the process to reflash everything...

It stores the ROM at C:\ProgramData\RSA\Download\RomFiles\

Reboot to fastboot with power+volume down.

**WARNING: If you wanna keep encryption support, DONT LET THE DEVICE BOOT AFTER UNLOCKING IT WITH OEM UNLOCK, ALL THE COMMANDS MUST BE DONE WITHOUT EXITING FASTBOOT AND WITHOUT FACTORY RESET OTHERWISE YOU WILL FORGET THE ABILITY TO SET ENCRYPTION AND LOCKSCREEN**

Unlock your device with `fastboot oem unlock UNLOCKCODE`

Flash vbmeta.img with `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img` (We don't have TWRP right now so everything will get messy now)

Reboot to fastbootd from fastboot with `fastboot reboot fastboot`

Now we need to delete the 2 system partitions, and resize them, otherwise fastbootd will complain that we dont have enough space, even if we delete the product partitions.

* `fastboot delete-logical-partition system_a`
* `fastboot delete-logical-partition system_b`
* `fastboot create-logical-partition system_a 100000`
* `fastboot create-logical-partition system_b 100000`

Flash the wanted GSI, in my case it was `system-squeak-arm64-ab-vndklite-vanilla-secure.img.xz`

Extract it and flash with `fastboot flash system_a system-squeak-arm64-ab-vndklite-vanilla-secure.img`
Same for system_b just in case.

Now type `fastboot reboot`, it should boot straight into the GSI, keeping encryption and with the storage wiped. 

After booting, set fingerprint, lockscreen and go to phh treble settings. 
On misc enable:
* Use alternate way to detect headsets. (This fixes the headphone jack)
* Disable HW overlays, (my device felt a bit choppy with the latest release without it).
* Expose Aux cameras
* Force Enable Camera2API HAL3

After that reboot and you should be ready to go.

Problems: Dynamic partition layouts. Even if you use vndklite, you cant modify /vendor or /system files to add an overlay... Had to create one, extract vendor_a  from the stock super.img, resize it, mount it, add the overlay apk to /vendor/overlays, umount and resize again on my Linux desktop.

I'll just upload my vendor here and create a PR with my changes.

[vendor_a.img with overlay](https://drive.google.com/file/d/12OCER4GLDf6OUMJA1B88LIVywKwFSZ4y/view?usp=sharing)

It fixes powersaving and the choppy display as far as I have seen.

To flash it, go to fastbootd and use `fastboot flash vendor_a vendor_a.img` and same for vendor_b






