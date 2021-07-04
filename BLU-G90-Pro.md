# Blu G90 Pro

Main rear camera only supports 12MP instead of 48MP.  Additional rear cameras don't work at all.  FM radio does not work.

## Steps to install

* Step 1: Enable developer mode.  Turn on OEM unlocking in developer options.
* Step 2: Reboot into fastboot mode (hold volume up button when booting) and run `fastboot flashing unlock`
* Step 3: Optional: Install TWRP from https://github.com/lopestom/device_TWRP-PBRP_BLU_G0370WW
* Step 4: Reboot into fastbootd (enter fastboot from recovery mode)
* Step 5: You will need to delete the product partition by running `fastboot delete-logical-partition product`
* flash this image with the `fastboot` utility:
    ```
    $ fastboot flash system system-arm64-ab-gapps-su.img
    ```
* Wipe user data partition by running `fastboot -w`
* Flash any additional packages (i.e. gapps) and reboot.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Front Camera              | Working                                                   |
| Rear Camera (Main)        | Working, but only at 12MP instead of 48MP                 |
| Wide Angle Camera         | Not working                                               |
| Macro Camera              | Not working                                               |
| Depth Camera              | Not working                                               |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Untested                                                  |
| Fingerprint               | Working                                                   |
| Offline Charging          | Working*                                                  |
| Headphone Jack            | Working*                                                  |

## Notes

* Offline charging works correctly on AndyYan's LineageOS 18.1 image.  On AOSP 11.0 v309, the device just sits at the boot screen when plugged in.
* Headphone jack works correctly after running `setprop persist.sys.overlay.devinputjack true`
* Additional back cameras do not show up when running `dumpsys media.camera` on GSI, but do appear when running the same command under stock firmware.  Even under stock firmware, the main back camera is limited to 12MP when not using the stock camera app, so I suspect they are probably using some non-standard APIs.
* The stock FM radio app runs after copying it over along with the required library, and fixing permissions.  It can tune to stations and display RDS info, but no sound is output over either the speaker or the headphones.
---

Tested By: ArrestedLightning - G0370WW, Firmware Version 10.0.04.03 - Tested 2021-07-04