# Barnes & Noble Nook Tablet 10.1" 2018 (BNTV650)
![Nook Tablet 10.1](https://prodimage.images-bn.com/pimages/9780594827917_p0_v1_s600x595.jpg)

## Stock Android 8.1 Oreo v1.0.9 firmware files (excluding the userdata.img):

Link: ([click here to continue to the download](https://drive.google.com/file/d/1gLshzM9zYEvR0Cknl4eh6KI32nEZbL5O/view))


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
| Battery                   | Battery life seems to be bad on Treble, compared being on the stock firmware. Low battery power mode will somewhat help with this.                                                       |
---
# Basic Flashing Guide
This is assuming your device is brand-new, with a locked bootloader. You should also have **adb** installed on your computer with the appropriate drivers. **Make sure your device has a good charge before continuing.**

## Pre-Flash
1. Boot your device and skip through the setup procedure. _A Wi-Fi connection is not required for this process._
2. Open the **Setting menu**, go to **System**, **About tablet**, and enable developer mode by tapping the **Build number** field several times. _Hint: watch for the popup at the bottom of the screen to tell you how many times you need to tap the Build number._
3. Go back to the **System** menu, and open the new **Developer options** menu.
4. Toggle OEM unlocking to unlock your bootloader.
5. Toggle USB debugging, and accept the popup.
6. Connect your tablet with a USB cable. You should see a popup asking if you want to allow USB debugging. Check the **Always allow** box, and tap **OK**.

## Ready to flash
1. Open a terminal on your computer, and type `adb devices` to verify that your tablet is available and ready to accept commands. You should see a response similar to this:

> List of devices attached

> 60901650008348  device

_If you see an error message, double-check that your tablet has been authorized with your computer. You may need to disconnect/reconnect it, or restart the adb server (`adb kill-server`)._

2. Now that adb is ready, reboot into the bootloader with `adb reboot bootloader`. The screen will go blank, and in a few moments you should see `=> FASTBOOT mode...` at the bottom of your screen.
3. Enter `fastboot flashing unlock`. You will see a warning appear on the tablet. Press the **Volume Up** button on your tablet to accept. Your bootloader is now completely unlocked, and all user data has been erased.
4. Wipe the System partition by entering `fastboot erase system`. You will see output confirming this action.
5. Enter `fastboot -u flash system name_of_system.img`, where _system name_of_system.img_ is the name of the ROM image you'd like to flash. You should see some output as the image is written to memory. This may take several minutes. Interrupting this process may require that you have to restart the flash process.
6. Finally, enter `fastboot reboot`. Your device will reboot several times, at one point showing an erasing screen. Allow the device to continue and it will eventually boot into your new system.

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
* Last edited by: tgp1994 (1/31/2020)