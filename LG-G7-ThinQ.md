# Testers
- [Sellerie](https://www.github.com/sellerie98)

# Hardware
Has been tested on:
- LMG710EM (the only phone variant that is unlockable at the moment)

# GSI tested
[phh](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/experimental-phh-treble-t3709659) works with vendor and boot image from firmware/vendor revision 20c OOTB. vbmeta needs to be disabled and the boot image may have to be configured to boot GSIs.

# Procedure
## Requirements
- The Pie 20c image needs to be installed using LGUP or LG Bridge (the firmware is yet only availiable for the korean region.)

You'll need to flash a TWRP-ed boot image to the currently inactive slot, switch to it and then boot from that image by simply hitting reboot recovery in TWRP.
Back on the new TWRP you flash the GSI .img file onto the system partition. If it doesnt show up in install image/zip menu, you need to switch to image view instead of zip with the button below on the right side.
If this is done, you need to copy the plat_sepolicy.cil file to (make sure, system is mounted in the mount menu of TWRP) /system/system/etc/selinux/.

After that, the GSI should boot up successfully.


# Notes

When switching to a GSI ROM, you NEED to format data. This is achieved in TWRP by tapping: Wipe -> format data -> type yes. Be careful. That not only wipes /data but also wipes your INTERNAL STORAGE (/storage/emulated/0, which is basically a symlink to /data/media)!!
