# Xiaomi Redmi 9 (lancelot)

Testing is ongoing, booting and taking photos works, the rest is untested so far.

Recovery: no official TWRP, there's a PitchBlackRecovery beta that boots (but lacks fastbootd).

## Background info

The device uses [dynamic partitioning](https://source.android.com/devices/tech/ota/dynamic_partitions), you need to enter "User Mode fastboot (fastbootd)" to be able to flash the system partition. On my device, I could not go from "Bootloader fastboot" to "User Mode fastboot" with the command `fastboot boot fastboot`. Instead, I got an error message along the lines "unknown boot target".

What worked was: booting into system, enabling abd and then using `adb reboot fastboot` to enter "User Mode fastboot (fastbootd)" or `adb reboot bootloader` to enter "Bootloader fastboot".

Because of this, the "order" of flashing vbmeta then system is reversed in the steps below.

## Steps to install


On the phone:

* Open Settings → About phone.
  Tap several times MIUI Version to enable Developer options.
* Open Settings → Additional settings → Developer options.
  Check that MI Unlock status is set to Unlocked, and
  enable USB debugging.
* Unlock the bootloader of the Redmi 9, e.g. with [XiaoMiTool V2](https://www.xiaomitool.com/V2/) on Linux. Proceed only once this is done. (I had to register the device to my account and wait 7 days to achieve this milestone).


On the PC:

* Download Stock Rom (I used [EEA V11.0.9](https://bigota.d.miui.com/V11.0.9.0.QJCEUXM/lancelot_eea_global_images_V11.0.9.0.QJCEUXM_20201201.0000.00_10.0_eea_3f4b4c4909.tgz))

* Extract vbmeta `tar -xzvf lancelot_eea_global_images_V11.0.9.0.QJCEUXM_20201201.0000.00_10.0_eea_3f4b4c4909.tgz`

* Download and extract GSI image (I used [v305-arm64-ab-vanilla](https://github.com/phhusson/treble_experimentations/releases/download/v305/system-roar-arm64-ab-vanilla.img.xz))

* Enter user mode fastboot (fastbootd) to flash system

      # enter user mode fastboot (fastbootd)
      adb reboot fastboot
      # wait until in fastbootd
      fastboot flash system system-roar-arm64-ab-vanilla.img
      # leave fastbootd
      fastboot reboot

* The device will now be in a boot loop, because it cannot verify the new system image. You will need to disable the dmverity firmware verification (see next steps)

* Enter Bootloader fastboot (Press Volume Down+Power together until reboot, then let go of power, keep holding Volume Down)

* When in Bootloader fastboot, flash vbmeta

      # flash vbmeta with verity & verification disabled
      fastboot --disable-verity --disable-verification flash lancelot_eea_global_images_V11.0.9.0.QJCEUXM_20201201.0000.00_10.0_eea_3f4b4c4909/images/vbmeta     
      # reboot
      fastboot reboot


## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             |  Not tested                                                    |
| Bluetooth                 |  Not tested                                                    |
| WiFi                      |  Not tested                                                    |
| SIM / Mobile Data / Voice |  Not tested                                                    |
| VoLTE                     | Not tested                                                |
| Fingerprint               | Not tested                                                |
| NFC                       | N/A                                                       |
| Offline Charging          | Not working                                               |

## References

* PitchBlack Recovery Redmi 9 lancelot (beta) https://github.com/PitchBlackRecoveryProject/android_device_xiaomi_lancelot-pbrp/releases/3.0.0-beta

Tested By: 2021/04/20 sebastianapel - Template created by @zguithues and @hackintosh5