
Model BNTV650.

# Hardware Support
* Buttons: Work.
* Camera: Stock camera works, front and back.
* Speakers: Work.
* Bluetooth: Bluetooth Audio works. File transfer untested.
* WiFi: Works.
* Display: Works, though screen size is retrieved incorrectly? Reports as a 14.1" display, so the DPI is off. Can be worked around with "Easy DPI Changer" or through the "Developer options" in the device settings with the values of "752 dp".
* The battery drains quite too fast on Treble, even with the low battery power saving mode enabled, compared to the stock firmware.
* The display will be in portrait mode on a fresh start. You'll have to allow screen rotation under "display" under the device settings.

# Tablet specs
* Battery: up to 8.5 hours
* 32GB Internal eMMC chip.
* 2GB RAM.
* The storage is expandable to 256GB with an SD card.
* Dimensions in mm: 262.00 x 158.00 x 9.60
* Front camera: 2MP.
* Rear camera: 2MP.
* Shipped OS: Android 8.1 Oreo with Google Play support.
* VNDK v27.0 legacy.
* A-Only system partition.
* Release date: November 2018.
* Supported wifi modules: 802.11 a/b/g/n/ac
* Screen size in inches: 10.10
* Screen resolution: 1200x1920 pixels.
* Processor arch: arm64.
* CPU: Quad Core MediaTek A35-MT8167A.
* Claims to have "stereo speakers".
* Full HD display.
* Original brand new price from OEM: $130
* It comes with a 1GB swap file out of the box (you can use "free swapper for root" from the Google Play Store to increase the size of the current swap file).

# Stock OEM v1.0.9 Android 8.1 Oreo firmware files (excluding the userdata.img)
* Link: https://drive.google.com/file/d/1gLshzM9zYEvR0Cknl4eh6KI32nEZbL5O/view

# OEM hardware drivers
* OEM recovery drivers: https://github.com/secretwolf98/android_device_recovery_bn_bntv650_st18c10bnn
* OEM boot drivers: https://github.com/secretwolf98/android_device_kernel_bn_bntv650_st18c10bnn
* OEM vendor drivers: https://github.com/secretwolf98/android_device_vendor_bn_bntv650_st18c10bnn

## Additional Notes:
* Boot animation is missing on Phh-treble v25, unsure why.
** Can be fixed with https://github.com/phhusson/device_phh_treble/commit/92db7539d07ddb90f89fb611c6f32f3f72b3f349.
* Does not boot Phh-treble v107, seems to have errors with the GPU and KeyMaster.
* Phh Treble 9 Pie arm64 A-only with G-Apps & with SU GSI v119 boots perfectly (make sure to fastboot erase system before installing & factory reset/clear cache in the stock recovery before going into the system).
* Phh Treble v204 Android 10 Q arm64 A-only with gapps fails to flash via fastboot due to a small system partition.
* Phh Treble v121 Android 9 Pie arm64 A-only with gapps and su flashes successfully via fastboot & boots into the system without an issue.
* Phh Treble v120 Android 9 Pie arm64 A-only with gapps and su flashes successfully via fastboot & it boots into the system without an issue.
* Phh Treble v205 Android 10 Q arm64 A-only with gapps fails to flash via fastboot due to a small system partition.
* Phh Treble v205 Android 10 Q arm64 A-only vanilla flashes successfully via fastboot & boots into the system without an issue.
* Phh Treble v122 Android 9 Pie arm64 A-only with gapps and su flashes successfully via fastboot & it boots into the system without an issue.
* Phh Treble v123 Android 9 Pie arm64 A-only with gapps and su flashes successfully via fastboot & it boots into the system without an issue. (I was able to dirty flash this update from v122. First step is to clear the cache in the stock recovery. Then flash the system img in bootloader/fastboot)
* It seems like the battery was lasting fine on v122 with normal use without low battery power mode. But I will continue to test this out in v123 and report back after some testing after a few days.

## Tested By:
* izzy84075 (Phh Treble v25 on 11/30/2018, Phh Treble v107 on 11/30/2018)
* secretwolf98 (Phh Treble v119 on 10/4/2019)
* secretwolf98 (Phh Treble v121, Phh Treble v120, Phh Treble v204 on 11/30/2019)
* secretwolf98 (Phh Treble v205 on 12/3/2019)
* secretwolf98 (Phh Treble v122 on 12/9/2019)
* secretwolf98 (Phh Treble v123 on 12/12/2019)

![Nook Tablet 10.1](https://prodimage.images-bn.com/pimages/9780594827917_p0_v1_s600x595.jpg)