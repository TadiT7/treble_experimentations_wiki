# [Nokia 1.3] - [Drax]

### Bootloader unlock

- Update to nokia android 11 (using updater).
- Mandatory: Insert SIM. Enable Developer Setting -> OEM unlock
- If OEM unlock is greyed out then restart phone and try again. Unless it pings Nokia server it does not allow OEM unlock.
- Power off (Important see last point)
- Hold Volume Down and then press power. You feel a vibration and then it boots into Bootloader mode
- Verify if you are connected properly with `fastboot devices`
- `fastboot flashing unlock`
- Use Volume Keys to select Unlock. Scary message!
- Allow restart
- Now device is unlocked. Again enable Developer Settings and authorise your PC.
- Notes: For unknown reasons. `adb reboot bootloader` and then `fastboot flashing unlock` does not work. You need to **power off**.

### Download 

- system-???-arm32_binder64-ab-vanilla.img.xz
- Do unxz
- I tested squeak and roar both works properly
- gzip in your PC
- `adb push system-squeak-arm64-ab-vanilla.img.gz /storage/emulated/0/`
- The next command is a single line. Note once you enter this, Nokia 1.3 becomes very slow. So wait... really wait.
- `adb shell am start-activity -n com.android.dynsystem/com.android.dynsystem.VerificationActivity -a android.os.image.action.START_INSTALL -d file:///storage/emulated/0/system-roar-arm32_binder64-ab-vanilla.img.gz --el KEY_SYSTEM_SIZE  1014649136 --el KEY_USERDATA_SIZE 2147483648`
- Look for the message: Dynamic system is ready. To start using it, restart your device.


## Hardware Support (Android 11/12)

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | √                                                         |
| Speaker / Mic             | √                                                         |
| Bluetooth                 | √                                                         |
| WiFi                      | √                                                         |
| SIM / Mobile Data / Voice | √                                                         |
| VoLTE                     | I do not know (no available from my provider)               |


### Remarks

- Roar is quicker, responsive than Squeak