## Infinix Hot 7(X624B)

## Installation
- Remove dm-verity with magisk or any other sutable way
- Make sure you have formatted the phone
- Unlock your bootloader on the developer option then power off then phone.
- Boot to fastboot by holding `power` and `volume down` buttons.
- Download the infinix hot 7 fastbootdriver then connect through adb either from pc or android with otg app like [Bugjaeger](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=en&gl=US)
  and run `fastboot flashing unlock` hit volume up to confirm.
- Run `fastboot flash system system-quack-arm-aonly-gapps.img`
- Boom thats it. Simple right.

**Supported GSI : A only**

**Tested GSI : [AOSP 10.0 v222](https://github.com/phhusson/treble_experimentations/releases/tag/v222) - [system-quack-arm-aonly-gapps.img.xz](https://github.com/phhusson/treble_experimentations/releases/download/v222/system-quack-arm-aonly-gapps.img.xz)**

## Issues
 Random device restart not frequently maybe cause am rooted using magisk and superuser was already available.

## Hardware Support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Troublesome|
| Speaker / Mic / Calls     | Working  |
| Bluetooth / BT Audio                | Troublesome |
| WiFi                      | Working                                                    |
| SIM / Mobile Data / Voice | Working                                                    |
| VoLTE                     | Device Not Support                                              |
| Fingerprint               | Not working                                                   |
| Bluetooth calls           | Not Tested                                               |
| Brightness                | Working |
| Sensors | Not tested |
---
Template created by [brostosjoined](https://github.com/brostosjoined)