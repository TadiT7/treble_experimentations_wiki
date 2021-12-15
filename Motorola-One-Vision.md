
Flashing procedure:

1. Boot to TWRP and go to Wipe > Dalvik, Data and System.
2. Head over to SD Card and tap on Install Image (the bottom right button on your recovery).

3.Now flash the GSI ROM.
4.Once it gets flashed (2-3mins at max), go to Reboot and tap Recovery. You will get a message that **NO OS** is installed. **IGNORE** it and proceed with the reboot. You should **NOT** reboot to the system otherwise bootloop is guaranteed from my end :)

**Reason for bootloop**: With A/B partition devices like ours, there is no separate recovery partition. It is handled by the boot partition itself (that is why we boot the recovery rather than actually flashing itself). 
Now we will have to refresh the boot partiton and for that, you will have to reboot in TWRP recovery. If you don't do so, system won't be able to recognize the boot partition (personal experience: tried many times and ended up in **bootloop** each time).

5.Once you reboot to recovery, again head over to Reboot > System. This time you won't notice the NO OS message. The first time the device might reboot once or twice, that is completely normal.

That's it. Enjoy the GSI on your kane.




