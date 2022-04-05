# [Nokia 1.3] - [Drax]

### Bootloader unlock

- Update to nokia android 11 (using updater).
- Mandatory: Insert SIM. Enable Developer Setting -> OEM unlock
- If OEM unlock is greyed out then restart phone and try again. Unless it pings Nokia server it does not allow OEM unlock.
- Power off (Important see last point)
- Hold Volume Down and then press power. You feel a vibration and then it boots into fastboot mode
- Or use `fastboot reboot fastboot`
- Verify if you are connected properly with `fastboot devices`
- `fastboot flashing unlock`
- Use Volume Keys to select Unlock. Scary message!
- Allow restart
- Now device is unlocked. Again enable Developer Settings and authorise your PC.

### Download and install GSI

- Charge your phone to 100 %
- system-???-arm32_binder64-ab-vanilla.img.xz
- Do `unxz`
- `adb reboot bootloader`
- Get vbmeta from "Nokia 1.3 Flash File – Stock ROM" (just google it) and unzip

`user@ubuntu: ~/ $ fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`

`Rewriting vbmeta struct at offset: 0`

`Sending 'vbmeta' (4 KB)                            OKAY [  0.003s]`

`Writing 'vbmeta'                                   OKAY [  0.002s]`

`Finished. Total time: 0.030s`

`user@ubuntu: ~/ $ fastboot reboot fastboot`

`Rebooting into fastboot                            OKAY [  0.001s]`

`< waiting for any device >`

`Finished. Total time: 20.381s`

`user@ubuntu: ~/ $ fastboot flash system system-roar-arm32_binder64-ab-vanilla.img `

`Resizing 'system'                                  OKAY [  0.005s]`

`Sending sparse 'system' 1/4 (262140 KB)            OKAY [ 13.330s]`

`Writing 'system'                                   OKAY [  5.165s]`

`Sending sparse 'system' 2/4 (262140 KB)            OKAY [ 12.603s]`

`Writing 'system'                                   OKAY [  5.177s]`

`Sending sparse 'system' 3/4 (262140 KB)            OKAY [ 13.173s]`

`Writing 'system'                                   OKAY [  5.174s]`

`Sending sparse 'system' 4/4 (204448 KB)            OKAY [  9.632s]`

`Writing 'system'                                   OKAY [  4.101s]`

`Finished. Total time: 68.370s`


- Select **recovery** in the menu. Do **wipe data/factory reset**


### Results

- I tested squeak and roar both works properly

### Dynamic System Updates (DSU) 


- gzip in your PC
- `adb push system-squeak-arm64-ab-vanilla.img.gz /storage/emulated/0/`
- `adb shell setprop persist.sys.fflag.override.settings_dynamic_system true`
- The next command is a single line. Note once you enter this, Nokia 1.3 becomes very slow. So wait... really wait.
- `adb shell am start-activity -n com.android.dynsystem/com.android.dynsystem.VerificationActivity -a android.os.image.action.START_INSTALL -d file:///storage/emulated/0/system-roar-arm32_binder64-ab-vanilla.img.gz --el KEY_SYSTEM_SIZE  1014649136 --el KEY_USERDATA_SIZE 2147483648`
- Look for the message: Dynamic system is ready. To start using it, restart your device.
- Notes: Inside developer options there is DSU loader but it is empty (as Nokia does not provide it). 


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