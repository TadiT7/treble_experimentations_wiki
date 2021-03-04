# Xiaomi Redmi 8 (olive)

Everything tested except for offline charging works

## Steps to install

Unlock the bootloader of the Redmi 8, e.g. with [XiaoMiTool V2](https://www.xiaomitool.com/V2/) on Linux.
Proceed only once this is done.

On the phone:

* Open Settings → About phone.
  Tap several times MIUI Version to enable Developer options.
* Open Settings → Additional settings → Developer options.
  Check that MI Unlock status is set to Unlocked, and
  enable USB debugging.

On the PC:

* Download [TWRP 3.4.0-1](https://dl.twrp.me/olive/twrp-3.4.0-1-olive.img) from <https://twrp.me/xiaomi/xiaomiredmi8.html> and rename to `twrp.img`.
* Download [`vbmeta.img`](https://forum.xda-developers.com/attachments/vbmeta-img.5031479/) from <https://forum.xda-developers.com/t/guide-how-to-instal-gsi-rom-havoc-os-v3-x-official-arm64-a-b-on-redmi-8.4108735>.
* Flash TWRP and vbmeta:

      adb reboot bootloader
      fastboot devices # check if device is connected correctly
      fastboot flash recovery twrp.img
      fastboot flash vbmeta vbmeta.img

On the phone:

* Press “Power” and “Volume Up” buttons for about 20 seconds until you see the TWRP screen.
* Select Wipe → Format Data.
* Select Wipe → Advanced Wipe and wipe System, Data, Cache, and Dalvik.

On the PC:

* Download phhusson's [AOSP 11.0 v300.n](https://github.com/phhusson/treble_experimentations/releases/download/v301/system-roar-arm64-ab-gapps.img.xz) from <https://github.com/phhusson/treble_experimentations/releases>.
  Note that the Redmi 8 is an ARM64 A/B device.
* Decompress the compressed image:

      xz --decompress system-roar-arm64-ab-gapps.img.xz
* Copy the uncompressed image to the Redmi 8.

On the phone (still in TWRP):

* Select Install → Install Image
* Select the uncompressed image file.
* Flash to System Image.


## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not tested                                                |
| Fingerprint               | Not tested                                                |
| NFC                       | N/A                                                       |
| Offline Charging          | Not working                                               |

## References

* Instructions for Redmi 7 (predecessor):
  <https://github.com/phhusson/treble_experimentations/wiki/Xiaomi-Redmi-7>
* Overview of guides for Redmi 8:
  <https://forum.xda-developers.com/t/index-all-custom-rom-kernel-recovery-for-redmi-8.4109481/>
* Generic instructions for GSI image flashing:
  <https://www.xda-developers.com/flash-generic-system-image-project-treble-device/>

Tested By: @01mf02 - 2021/03/04 - Template created by @zguithues and @hackintosh5