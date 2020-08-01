# Device Blu G90 G0310WW

Stock system dump w/ vbmeta img and stock recovery 

https://github.com/mrmazakblu/blu_g0310ww_dump

           *MUST HAVE WORKING ADB AND FASTBOOT (platform Tools) for this process. I used SDK 30

https://developer.android.com/studio/releases/platform-tools

## Steps to install

* Step 1  Unlock Bootloader
          *enable developer options on phone
             *Settings-- about phone -- click build number 7 times
             *go back one menu, select system
             *new option "developer options" is available, open
             *scroll to "enable OEM unlock" -- enable it
           *Reboot to bootloader-- 
             *long press power, select reboot
             *keep volume up pressed
             *when phone turns on, will see bootloader menu, use volume keys to select bootloader
           *Open cmd prompt(if need help with this, please use google)
           *fastboot flashing unlock
             *on phone screen will see confirmation message. Use volume keys to confirm
         
* Step 2  Flash vbmeta partions (3 total -- vbmeta, vbmeta_system, vbmets_vendor) with --disable-verity --disable-verification
           *fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
           *fastboot --disable-verity --disable-verification flash vbmeta_system vbmeta_system.img
           *fastboot --disable-verity --disable-verification flash vbmeta_vendor vbmeta_vendor.img


* Step 3  Reboot to fastboot (not bootloader) 
           *fastboot reboot fastboot

* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-quack-arm64-ab-gapps.img
    $ fastboot -w
    $ fastboot reboot
    ```
    

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Status    Working                                         |
| Speaker / Mic             | Status    Working                                         |
| Bluetooth                 | Status                                                    |
| WiFi                      | Status    Working                                         |
| SIM / Mobile Data / Voice | Status                                                    |
| VoLTE                     | Status    Unknown__ Provider / Plan Not include Volte     |
| Fingerprint               | Status    Working                                         |
| NFC                       | Status                                                    |
| Offline Charging          | Status    Turns Boot Logo ON stays on no charge animation |
| Other feature             | Status                                                    |
---

Tested By: MrmazakBlu - Model-Number(region) G0310WW, Firmware Version  - Date tested 7-31-2020 - Template created by @zguithues and @hackintosh5
