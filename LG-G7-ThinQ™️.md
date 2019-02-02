# Testers
- [Sellerie](https://www.github.com/sellerie98)

# Hardware
Has been tested on:
- LMG710EM (the only phone variant that is unlockable at the moment)

# GSI tested
[phh](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) works with vendor and boot image from firmware revision 10b OOTB (and with a modified kernel on 10p vendor+boot image aswell)

# Procedure
## Requirements
- The oreo firmware revision 10b installed via LGUP or LG Bridge. (Technically you just need vendor and boot image of revision 10b, even though this is possibly easier to achieve by simply flashing this version to your phone.
Regarding the boot image, I strongly recommend a TWRP-ed and Magisk-ed boot image.)

You'll need to flash a TWRP-ed boot image to the currently inactive slot, switch to it and then boot from that image by simply hitting reboot recovery in TWRP.
Back on the new TWRP you flash the GSI .img file onto the system partition. If it doesnt show up in install image/zip menu, you need to switch to image view instead of zip with the button below on the right side.
If this is done, you need to copy the plat_sepolicy.cil file to (make sure, system is mounted in the mount menu of TWRP) /system/system/etc/selinux/.

After that, the GSI should boot up successfully.


# Notes
[J0SH1X](https://www.github.com/J0SH1X) has mostly fixed the (horribly) messed up kernel sources released by LG of version 10p on his github page. Some things may be non-working yet though.
The file /system/system/etc/selinux/plat_sepolicy.cil needs to be modified: TBD

When switching to a GSI ROM, you NEED to format data. This is achieved in TWRP by tapping: Wipe -> format data -> type yes. Be careful. That not only wipes /data but also wipes your INTERNAL STORAGE (/storage/emulated/0, which is basically a symlink to /data/media)!!
