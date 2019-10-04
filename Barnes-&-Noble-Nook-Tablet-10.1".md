Model BNTV650.
# Hardware Support
* Buttons: Work.
* Camera: Stock camera works, front and back.
* Speakers: Work.
* Bluetooth: Bluetooth Audio works. File transfer untested.
* WiFi: Works.
* Display: Works, though screen size is retrieved incorrectly? Reports as a 14.1" display, so the DPI is off. Can be worked around with "Easy DPI Changer" or through the "Developer options" in the device settings with the values of "752 dp".

## Additional Notes:
* Boot animation is missing on Phh-treble v25, unsure why.
** Can be fixed with https://github.com/phhusson/device_phh_treble/commit/92db7539d07ddb90f89fb611c6f32f3f72b3f349 .
* Does not boot Phh-treble v107, seems to have errors with the GPU and KeyMaster.
* Phh Treble 9 Pie a-only with G-Apps & with SU GSI v119 boots perfectly (make sure to fastboot erase system before installing & factory reset/clear cache in the stock recovery before going into the system).

## Tested By:
* izzy84075 (Phh Treble v25 on 11/30/2018, Phh Treble v107 on 11/30/2018)
* secretwolf98 (Phh Treble v119 on 10/4/2019)