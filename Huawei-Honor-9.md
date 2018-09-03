### Flash instructions:

1. Backup data with [TWRP](https://forum.xda-developers.com/honor-9/development/oreo-t3754483) or other backup tool:
`adb reboot recovery`
_(reboots into your recovery and stock recovery if you haven't installed a custom recovery)_

2. Reboot to eRecovery

3. Wipe (factory reset including data) with stock eRecovery (TWRP wipe doesn't currently work)

5. Reboot to fastbootmode

5. Flash ROM .img to system partition using fastboot
`fastboot flash system GSINAME.img`
_(replace GSINAME.img with the name and location of your GSI image)_

4. Reboot device `fastboot reboot`


### Hardware commands - done with device turned off

#### Need to connect the computer:

- `Fastboot mode`: long press the volume down key + power button.

- `eRecovery mode`: long press the volume up key + power button.

#### Do not need to connect the computer:

- `Recovery mode`: long press the volume up key + power button.

- `Upgrade mode`: long press the volume up key + volume down key + power button.


### Additional infos:

- [Ported stock Camera exists](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/huawei-stock-camera-app-treble-roms-t3735169) and mostly work, keeping original quality.

- Brightness stuck at 40%, both in settings and real life.