# Motorola Moto G7 Power (XT-1955) (ocean)

Tested with Phh Treble v222 with Gapps
*some of these notes are no longer necessary as of the Motorola Android 10 update

VERY IMPORTANT
- To boot the Android 10 GSI, you must first change `ro.control_privapp_permissions=enforcing` to `ro.control_privapp_permissions=log` in `/vendor/build.prop`. Vendor enforcements denies permissions from the GSI and considers them violations. If this property is not changed, the vendor will prevent the device from booting (This is seemingly no longer necessary as of v215).
- To use Magisk on this GSI or any other, you must also remove `init.mmi.hab.sh` from `/vendor/bin/`. This file conflicts with Magisk's rooting permissions, preventing the device from booting when applied.
- Passing CTS/SafetyNet for certain apps like Pokémon GO will be rendered impossible unless you "Securize" the system by going to Settings --> Treble Settings --> Miscellaneous --> Securize
- To successfully receive an SMS message over the LTE network:
  - 1: [`android.hardware.telephony.ims.xml`](http://treble.phh.me/android.hardware.telephony.ims.xml) must be applied to `vendor/etc/permissions` with the permission 0644*.
  - 2: download and install [the latest ims apk](http://treble.phh.me/stable/ims-q.64.apk) as a user image and restart the system
  - 3: after restarting, do so again after approximately 6 minutes, and repeat the process 3-5 times
  - 4: as the VoLTE feature is still a work in progress, disable it in Settings --> Mobile network --> VoLTE. You will now receive 3G-only calls (until January 2021 for the T-Mobile network and shared MVNOs such as Metro), but SMS messaging over LTE will now function properly

## Wireless

### Wi-Fi

partially - Wifi connections will only be successful on Static connections 

### Mobile Data

works

### Bluetooth

works

### Mobile Hotspot

works

## RIL

### Calling

- Outgoing call

partially - only on 3G, as the VoLTE feature is still a work in progress; microphone works in calls only if Dial pad tones is enabled in Settings --> Sound*

- Incoming call

partially - only on 3G, as the VoLTE feature is still a work in progress; microphone works in calls only if Dial pad tones is enabled in Settings --> Sound*

### VoLTE (calls on the LTE network)

currently not working; calls cannot be made, and after such attempt, the phone cannot be hung up unless a system restart is prompted

### Messaging

- Sending (SMS and MMS)

works

- Receiving (SMS and MMS)


partially - only if the ims APK is installed, but its VoLTE feature is disabled, as instructed above.


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

works

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

- Once decrypting the device, the fingerprint API for the GSI is erased and when setting a screen lock, it refuses to accept the correct passcode to unlock the device; in other words, any password is the "incorrect password"
