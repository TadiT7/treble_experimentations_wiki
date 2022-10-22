# Huawei P50 (ABR-AL00)

Summary of what works and doesn't

## Steps to install

You need to do an unofficial Bootloader Unlock.  
(EDL test points and flash engineer firmware or replace unfused SoC.)  
Due to the specifications of HarmonyOS 2, you should unpack and repack vendor image(vendor image uses hmdfs filesystem) and convert the GSI image to EROFS, or you will not boot.
Enter fastbootd mode, and flash image normally.