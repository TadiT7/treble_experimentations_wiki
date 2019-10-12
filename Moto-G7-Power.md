# Motorola Moto G7 Power (XT-1955) (ocean)

Tested with Phh Treble v200 - beta D

VERY IMPORTANT
- To boot the Android 10 GSI, you must first change `ro.control_privapp_permissions=enforcing` to `ro.control_privapp_permissions=log` in `/vendor/build.prop`. Vendor enforcements denies permissions from the GSI and considers them violations. If this property is not changed, the vendor will prevent the device from booting.
- To use Magisk on this GSI or any other, you must also remove `init.mmi.hab.sh` from `/vendor/bin/`. This file conflicts with Magisk's rooting permissions, preventing the device from booting when applied.

## Wireless

### Wi-Fi

partially - DHCP method successfully connects on only few access points; most access points require the Static method for a reliable connection

### Mobile Data

(not yet tested)

### Bluetooth

(not yet tested)

### Mobile Hotspot

(not yet tested)

## RIL

### Calling

- Start call

(not yet tested)

- Receive call

(not yet tested)

### VoLTE

currently not working - [the apk](https://t.me/R3SPX_UPDATES/459) and [the patch](https://t.me/R3SPX_UPDATES/458) provided via [the #phh-volte Telegram group](https://t.me/phhvolte) has no effect on the system, therefore the function is still unavailable

### Messaging

- Sending (SMS and MMS)

(not yet tested)

- Receiving (SMS and MMS)


partially - messages can only be received on a 3G/HSPA/UMTS network, not on a 4G LTE network


## Hardware

### Fingerprint Reader

not working

### Proximity/Ambient/Gyro Sensor

works

### Camera

- Taking pictures (front and rear)

(not yet tested)

- Recording (front and rear)

(not yet tested)

- Flashlight

works

### Speaker

works

### Microphone

(not yet tested)

### Headphone Audio

not working

### FM Radio

not working - FM radio receiver could not be picked up by [the new NextRadio app](https://play.google.com/store/apps/details?id=com.nextradioapp.nextradio)

### GPS

(not yet tested)

## USB Connection

### USB On-The-Go Cable Connection

works

# Additional Notes

- The GSI's "Display Cutout" option in Developer Settings "device default, hide, etc" does not effectively hide the notch, like it does on the device's stock firmware

- Once decrypting the device, 1) the fingerprint API for the GSI is erased and 2) when setting a screen lock, it refuses to accept the correct passcode to unlock the device; in other words, any password is the "incorrect password"

- (Beta D) This may be a kernel problem but in certain button presses or certain actions, the GSI freezes and forcefully restarts the device, such as opening the camera, or disabling Airplane mode by enabling Wi-Fi

- (Beta D) After leaving the phone for a while, increasing the up time, apps refuse to open, and if so, gets stuck on their splash screen, having the user to restart the device each time