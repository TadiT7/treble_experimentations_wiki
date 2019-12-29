# Barnes & Noble Nook Tablet 10.1" 2018 (BNTV650)
![Nook Tablet 10.1](https://prodimage.images-bn.com/pimages/9780594827917_p0_v1_s600x595.jpg)

# Working & non-working Phh-Treble versions (with added notes):

* Phh-Treble v25 (The boot animation seems not to show up on this build. That can be fixed with this commit: ([click here to continue to the commit](https://github.com/phhusson/device_phh_treble/commit/92db7539d07ddb90f89fb611c6f32f3f72b3f349))
* Phh-Treble v107 (This build seems to have errors with the GPU & the KeyMaster)
* Phh-Treble v119 (This build seems to boot into the system without an issue. Everything works as expected)
* Phh-Treble v204 (This build seems to boot into the system without an issue. To use Android 10 on this tablet, you must use the no gapps version. The system partition is too small to be able to handle Android 10 with gapps)
* Phh-Treble v120 (This build seems to boot into the system without an issue. Everything works as expected)
* Phh-Treble v121 (This build seems to boot into the system without an issue. Everything works as expected)
* Phh-Treble v205 (This build seems to boot into the system without an issue. To use Android 10 on this tablet, you must use the no gapps version. The system partition is too small to be able to handle Android 10 with gapps)
* Phh-Treble v122 (This build seems to boot into the system without an issue. Everything works as expected)
* Phh-Treble v123 (This build seems to boot into the system without an issue. Everything works as expected)
* Phh-Treble v208 (This build seems to boot into the system without an issue. To use Android 10 on this tablet, you must use the no gapps version. The system partition is too small to be able to handle Android 10 with gapps)

# Hardware support:

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working. (Front & back cameras tested)                                                   |
| Speaker/Mic               | Working.                                                   |
| Bluetooth                 | Bluetooth audio works. Bluetooth file transfer is untested.                                                  |
| WiFi                      | Working.                                                   |
| Buttons                   | Working.                                            |
| Display size              | You will have to set the screen size to 752dp in the developer opitions in the device settings.                                                   |
| Display mode              | On first boot, the display shows in portrait mode. You'll have to fix this by allowing screen rotation in the display section of the device settings.                                                      |
| Battery                   | Battery life seems to be bad on Treble, compared being on the stock firmware. Low battery power mode will somewhat help this.                                                       |
---

## Tested By:

* izzy84075 (Phh-Treble v25 on 11/30/2018, Phh-Treble v107 on 11/30/2018)
* secretwolf98 (Phh-Treble v119 on 10/4/2019)
* secretwolf98 (Phh-Treble v121, Phh-Treble v120, Phh-Treble v204 on 11/30/2019)
* secretwolf98 (Phh-Treble v205 on 12/3/2019)
* secretwolf98 (Phh-Treble v122 on 12/9/2019)
* secretwolf98 (Phh-Treble v123 on 12/12/2019)
* secretwolf98 (Phh-Treble v208 on 12/26/2019)

## Device wiki notes:

* Created by: izzy84075 (12/3/2018)
* Last edited by: secretwolf98 (12/29/2019)