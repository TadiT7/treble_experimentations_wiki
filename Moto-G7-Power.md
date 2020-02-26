# Motorola Moto G7 Power (XT-1955) (ocean)

Tested with Phh Treble v212

VERY IMPORTANT
- To boot the Android 10 GSI, you must first change `ro.control_privapp_permissions=enforcing` to `ro.control_privapp_permissions=log` in `/vendor/build.prop`. Vendor enforcements denies permissions from the GSI and considers them violations. If this property is not changed, the vendor will prevent the device from booting.
- To use Magisk on this GSI or any other, you must also remove `init.mmi.hab.sh` from `/vendor/bin/`. This file conflicts with Magisk's rooting permissions, preventing the device from booting when applied.
- To successfully receive an SMS message over the LTE network, [`android.hardware.telephony.ims.xml`](http://treble.phh.me/android.hardware.telephony.ims.xml) must be applied to `system/etc/permissions` with the permission 0644. Optionally, the file can also be applied to `vendor/etc/permissions` given the 0644 permission. This solution may be easily break, so installing a Magisk module such as Pix3lify, is strongly ill-advised.

## Wireless

### Wi-Fi

partially - only if [this patch](https://t.me/G7Power/29274) is flashed in TWRP, modifying the vendor partition, will DHCP (default) connections work, otherwise Wifi connections will only be successful on Static connections 

### Mobile Data

works

### Bluetooth

works - only when the Wifi patch above is not flashed

### Mobile Hotspot

works

## RIL

### Calling

- Send call

partially - (https://github.com/phhusson/treble_experimentations/issues/1138)

- Receive call

partially - (https://github.com/phhusson/treble_experimentations/issues/1138)

### VoLTE (calls on the LTE network)

currently not working

### Messaging

- Sending (SMS and MMS)

works

- Receiving (SMS and MMS)


partially - only if android.hardware.telephony.ims.xml is applied to the system as instructed above


## Hardware

### Fingerprint Reader

works

### Proximity/Ambient/Gyro Sensor

works

### Camera

- Taking pictures (front and rear)

works

- Recording (front and rear)

works

- Flashlight

works

### Speaker

works

### Microphone

works - fully functioning only [outside of phone calls](https://github.com/phhusson/treble_experimentations/issues/1138)

### Headphone Audio

works

### FM Radio

not working - FM radio receiver could not be picked up by [the new NextRadio app](https://play.google.com/store/apps/details?id=com.nextradioapp.nextradio)

### GPS

works

## USB Connection

### USB On-The-Go Cable Connection

works

# Other Issues

- The GSI's "Display Cutout" option in Developer Settings "device default, hide, etc" does not effectively hide the notch, like it does on the device's stock firmware, although executing `adb shell wm size 720x1280` (a 16:9 screen ratio) is a good temporary solution. (The `1280` value (screen width) can be changed to the user's preferences)

- The System UI of the GSI currently conflicts with the Magisk module Pix3lify when the enabling of the Pixel framework is selected

- The navigation bar (the 2 button or 3 button scheme) can no longer be modified with [the Custom Navigation Bar app](https://play.google.com/store/apps/details?id=xyz.paphonb.systemuituner), therefore receiving an incompatibility error when installing from the Google Play Store

- Once decrypting the device, 1) the fingerprint API for the GSI is erased and 2) when setting a screen lock, it refuses to accept the correct passcode to unlock the device; in other words, any password is the "incorrect password"

- The swipe up for recent apps function when the 2-button navigation is selected does not work correctly in landscape mode, neither does the swipe right for previous app function, if in the development settings, the "Smallest width" display value is set to at least 597

https://github.com/phhusson/treble_experimentations/issues/791