### Fix for Speakers
Audio through speakers can be fixed by running these commands as root for every boot:

    chown root:audio /dev/nxp_smartpa_dev
    chmod 0660 /dev/nxp_smartpa_dev

Or running commands using `adb shell`:

    adb root
    adb shell chown root:audio /dev/nxp_smartpa_dev
    adb shell chmod 0660 /dev/nxp_smartpa_dev

> Note: This issue has been addressed and has a fix for newer builds of Phh AOSP

### Touchscreen Issue
The touchscreen might be irresponsive on the left/right edge of the screen. Simple workaround is to stop aptouch service as root:

    stop aptouch
 
Or using `adb shell`:

    adb root
    adb shell stop aptouch