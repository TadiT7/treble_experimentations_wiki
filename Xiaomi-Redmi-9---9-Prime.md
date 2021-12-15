# Xiaomi Redmi 9 (lancelot)
![](https://lh3.googleusercontent.com/cFqtZPdP-3L5XGrCR1_0cjOAGM1R2PwOAZ8vv5nVSaIiAXyd8mJ7vs5fA9ICXbm3EKqoBw5lGEzma1jK1Sw-jVt2fM4vGrl2VI3cC8CUo0c7i9NsAHxXvLmaPHUt6iKoB6rMMxqQ6H_HmWD0c3Qv5b0XMEJf7ET7TjzULh-_KqNhYpbQh44TVhit2zj74RrbNyiGu6_0dfB_fa_iRq8K4Kr_ewwvgcGpw2Ai-Q_pliNwWL5YBmcONwUlHHcNdH1uKvBT-5aLJBz65Hi1SENzH8Dj8gyvfGkf9Y250AgA0kC5ME8QlKgu2bVvc1fmjN8wM3AkJxLMBgxhf9_T5aOs2O0pX7VB9GjuxPRFoW9GML67Ta4K6uiDT5lpacHDyQR8ICRQ9m6VayeOzAjiQf3y7PyXHAinC7ywu_DjoPhevxdktZhsgu-0oczfTgVEkv8RUG6c_W0DNrTkc4uPdGlLd0wne7iL1n3VKoLRNpvznJUn85DNrHuNlFYDLnNwdP2xoXc0GCD1VxGaq_ZdRi9I7TKQ3jLuKJGchoK1JXJGg5gN3A-1wVr81UePyw5G8bsVKSEVLMK98yztLTIgtAlnxgm1f-gb8_a-3DhkKODTrY8iedS6E8Vxvn---6WfgS8hjFdtH71cZe1DEMdfjRHAWc874DaRjvO3pmJ4vhLT7zY00PRGrnTAXpXWGkVma93Q_C5nsqxgRzSivtbc6_y-2SI=w1280-h600-no?authuser=0)

Recovery ROM: there is no official TWRP, there's a PitchBlackRecovery beta that boots (but lacks fastbootd). As of writing (May 26th 2021, the best option is an official version of Skyhawk Recovery SHRP that can be built from source and has working decryption and fastbootd (see references for links to binaries).

## Background info

The device uses [dynamic partitioning](https://source.android.com/devices/tech/ota/dynamic_partitions), you need to enter "User Mode fastboot (fastbootd)" to be able to flash the system partition. On my device, I could not go from "Bootloader fastboot" to "User Mode fastboot" with the command `fastboot boot fastboot`. Instead, I got an error message along the lines "unknown boot target".

What worked was: booting into system, enabling ADB and then using `adb reboot fastboot` to enter "User Mode fastboot (fastbootd)" or `adb reboot bootloader` to enter "Bootloader fastboot".

Because of this, the "normal" order of first flashing vbmeta and then flashing system is reversed in the steps below.

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

You only disable verified boot for one time only! So when you want to flash GSI, you don't have to disable it again

## Hardware support

- I had a problems with headphones, but this [workaround](https://github.com/phhusson/treble_experimentations/issues/118#issuecomment-449163865) fixed it.
- Brightness had a problem, that could be fixed by "setprop persist.sys.qcom-brightness 2047" in adb (as root)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             |  Working                                                 |
| Headphones                | Workaround required                                            |
| Bluetooth                 |  Working                                                    |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| VoLTE                     | Not tested                                                |
| Fingerprint               | Not tested                                                |
| NFC                       | N/A                                                       |
| Offline Charging          |  Not tested                                                 |

## References

* Seahawk Recovery https://sourceforge.net/projects/shrp/files/lancelot/SHRP_v3.1_stable-Official_lancelot-1619460079.zip/download
* PitchBlack Recovery Redmi 9 lancelot (beta) https://github.com/PitchBlackRecoveryProject/android_device_xiaomi_lancelot-pbrp/releases/3.0.0-beta

Tested By: 2021/04/20 sebastianapel - Template created by @zguithues and @hackintosh5