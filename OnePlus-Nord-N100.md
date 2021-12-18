Works very well! WiFi, camera, calls, speakers, bluetooth work out of the box. Headphone jack requires configuration.

# Install GSI on Oneplus Nord N100

Enable USB debugging and connect phone to computer with adb installed. Then:

```
# unlock bootloader, device will wipe and restart
adb reboot bootloader
fastboot oem unlock

# re-enable usb debugging and again connect through USB with computer
adb reboot fastboot
fastboot erase system

# it will print either Erasing system_a or system_b. In the following I assume system_a was erased; if it was b, change commands accordingly.

# with phhusson GSI, system partition needs to be larger than stock. so delete the product_a partition to make space (see https://developer.android.com/codelabs/using-android-q-gsi#3)
fastboot delete-logical-partition product_a

# when flashing the system, disable integrity checks on startup to allow image to boot
fastboot --disable-verity --disable-verification flash system_a system-roar-arm64-ab-gapps.img

# wipe again, then reboot
fastboot -w reboot
```

# Fixes

- To get the headphone jack (3.5mm) to work, go to Settings > Phh Treble Settings > Qualcomm features and select "Use alternate audio policy".