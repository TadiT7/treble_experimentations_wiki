> ***This sub-page is highly dependant on user contributions based on their experiences***

> ***This sub page gives many fixes within phh settings which can be located in settings***

> ***NOTE: provided solutions are NOT GUARANTEED to fix the issue, although they have been tested to work for most users***

## can't listen to anything on phone calls
Try disabling a2dp overload from phh settings in settings and reboot

## Maximum brightness is too low
Enable alternate backlight scale and linear in phh settings

## Wired headphones not getting detected
### Solution 1
Enable alternative headphones detection in phh settings and reboot

### Solution 2
`adb shell setprop persist.sys.overlay.devinputjack true`

## Fingerprint setting is present, but crashes when opened
Open your settings > apps > show system apps (in the top-right 3 dot menu) > disable `com.google.android.setupwizard` (Android Setup)

## Fingerprint sensor not getting detected
`adb shell setprop persist.sys.phh.fingerprint.nocleanup true`

## High refresh rate not working
### Solution 1
Check force refresh rate option in phh settings

### Solution 2 (tested only on some oppo/realme/oneplus, **proceed with caution**)  
`adb shell -c service call SurfaceFlinger 1035 i32 0`

## Bluetooth connecting to device and then disconnecting
Try Disabling a2dp overload in PHH settings

## Always On display Not working
Enable Force always on display in phh settings misc reboot go to lock screen settings in display settings scroll down and check if always on display can be configured

## Bluetooth Crashing Systemui
disable media recommendations under Sound & Vibration > Media > Show media recommendations



