> ***This subpage is highly dependent on user contributions based on their experiences***

> ***This subpage gives many fixes within phh settings which can be located in settings***

> ***NOTE: provided solutions are NOT GUARANTEED to fix the issue, although they have been tested to work for most users***

## Can't listen to anything on phone calls
Try disabling A2DP offload from phh settings in Settings and reboot

## Maximum brightness is too low
Enable alternate backlight scale and linear brightness slider in phh settings

## Wired headphones not getting detected
### Solution 1
Enable alternative headphones detection in phh settings and reboot

### Solution 2
`adb shell setprop persist.sys.overlay.devinputjack true`

## Fingerprint setting is present, but crashes when opened
Open Settings > Apps > Show system apps (in the top-right 3 dot menu) > disable `com.google.android.setupwizard` (Android Setup)

## Fingerprint sensor not getting detected
`adb shell setprop persist.sys.phh.fingerprint.nocleanup true`

## High refresh rate not working
### Solution 1
Check force refresh rate option in phh settings

### Solution 2 (tested only on some oppo/realme/oneplus, **proceed with caution**)  
`adb shell -c service call SurfaceFlinger 1035 i32 0`

## Bluetooth connecting to device and then disconnecting
Try disabling A2DP offload in phh settings

## Always on display not working
Enable Force always on display in phh settings > misc, and then reboot. Go to lock screen settings in display settings, scroll down, and check if always on display can be configured

## Bluetooth crashing SystemUI
Disable media recommendations under Sound & Vibration > Media > Show media recommendations



