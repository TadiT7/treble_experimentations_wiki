# Motorola Moto G7 Power (XT-1955) (ocean)


## Wireless

### Wi-Fi

partially - DHCP method successfully connects on only few access points; most access points require the Static method for a reliable connection

### Mobile Data

works - confirmed to work on at least Metro by T-Mobile on AOSP Pie v115 and up

### Bluetooth

partially - Media audio is confirmed to be a bit choppy. Call audio, on the other hand, works fine

### Mobile Hotspot

works

## RIL

### Calling

- Start call

works

- Receive call

works

### VoLTE

currently not working - [the apk](https://t.me/R3SPX_UPDATES/459) and [the patch](https://t.me/R3SPX_UPDATES/458) provided via [the #phh-volte Telegram group](https://t.me/phhvolte) works, but prevents calls from hanging up successfully

### Messaging

- Sending (SMS and MMS)

works

- Receiving (SMS and MMS)


partially - messages can only be received on a 3G/HSPA/UMTS network, not on a 4G LTE network


## Hardware

### Fingerprint Reader

works

### Proximity/Ambient/Gyro Sensor

works

### Camera

- Taking pictures (front and rear)

works

- Recording (front and rear)

partially - front camera lagged during recording; the sound from the recordings of the front and rear camera is also choppy

- Flashlight

works

### Speaker

partially - resulting sound is choppy as well

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

# Additional Notes

- The GSI does not yet feature a developer option "Display Cutout" in order to hide the notch, like it does on the device's stock firmware

- Unlike the stock firmware, which aims to keep the device's battery life lasting up to 72 hours, multiple users report that battery life with the GSI does not last near to 72 hours on a full charge such as the international/unlocked models

- Although Magisk works on the stock firmware, flashing Magisk on the GSI conflicts with the system somehow, causing the device to bootloop (similar situation with the Moto G7 (river) (https://github.com/topjohnwu/Magisk/issues/844#issuecomment-485201012))

- Once decrypting the device, the fingerprint API for the GSI is erased

https://github.com/phhusson/treble_experimentations/issues/611