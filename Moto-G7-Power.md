# Motorola Moto G7 Power (XT-1955) (ocean)

Tested with Phh Treble v200 - beta D

VERY IMPORTANT
- To boot the Android 10 GSI, you must first change `ro.control_privapp_permissions=enforcing` to `ro.control_privapp_permissions=log` in `/vendor/build.prop`. Vendor enforcements denies permissions from the GSI and considers them violations. If this property is not changed, the vendor will prevent the device from booting.
- To use Magisk on this GSI or any other, you must also remove `init.mmi.hab.sh` from `/vendor/bin/`. This file conflicts with Magisk's rooting permissions, preventing the device from booting when applied.

## Wireless

### Wi-Fi

works - only if [this patch](https://t.me/G7Power/27482) is flashed in TWRP, modifying the vendor partition, otherwise Wifi connections will only be successful on Static connections and not DHCP (default) connections

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

not working

### FM Radio

not working - FM radio receiver could not be picked up by [the new NextRadio app](https://play.google.com/store/apps/details?id=com.nextradioapp.nextradio)

### GPS

works

## USB Connection

### USB On-The-Go Cable Connection

works

# Other Issues

- The GSI's "Display Cutout" option in Developer Settings "device default, hide, etc" does not effectively hide the notch, like it does on the device's stock firmware

- The System UI of the GSI currently conflicts with the Magisk module Pix3lify when the enabling of the Pixel framework is selected

- The navigation bar (the 2 button or 3 button scheme) can no longer be modified with [the Custom Navigation Bar app](https://play.google.com/store/apps/details?id=xyz.paphonb.systemuituner), therefore receiving an incompatibility error when installing from the Google Play Store

- Once decrypting the device, 1) the fingerprint API for the GSI is erased and 2) when setting a screen lock, it refuses to accept the correct passcode to unlock the device; in other words, any password is the "incorrect password"

- (Beta D) This may be a kernel problem but in certain button presses or certain actions, the GSI freezes and forcefully restarts the device, such as opening the camera, or changing certain states of quick settings such as Airplane mode

- (Beta D) After leaving the phone for a while, increasing the up time, apps refuse to open, and if so, gets stuck on their splash screen, having the user to restart the device each time

- (Beta D) The two issues above may correspond with the system itself significantly lagging or straight up freezing when performing certain actions or playing powerful games, such as Asphalt 9: Legends

- (Beta D) The swipe up for recent apps function when the 2-button navigation is selected does not work correctly in landscape mode, neither does the swipe right for previous app function, if in the development settings, the "Smallest width" display value is set to at least 597

- (Beta D) When forcefully enabling full-gesture navigation on launchers other than the default, (using the adb command `adb shell cmd overlay enable com.android.internal.systemui.navbar.gestural`) the swipe up and hold for recent apps function does not work, neither does the swipe right for previous app function. (Tested with Lawnchair Launcher v2) This is proven not to work when the "Smallest width" value was set to either more or less than 597

https://github.com/phhusson/treble_experimentations/issues/791