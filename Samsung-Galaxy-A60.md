What can be used and what can't :

## Android 10

| Starting_Up | Daily_Use | Wifi | SIM  | VoLTE | Bluetooth | GPS  | Brightness | Torch | Hotpot | NFC  | Fingerprint | Camera | MTP       | Note |
| ----------- | --------- | ---- | ---- | ----- | --------- | ---- | ---------- | ----- | ------ | ---- | ----------- | ------ | --------- | ---- |
| ✔           | ✔         | ✔    | ✔    | ❌     | ✔         | ✔    | ✔          | ✔     | ✔      | ✔    | ✔           | ✔      | ⭕ADB_ONLY |      |

## Android 11

| Starting_Up | Daily_Use | Wifi | SIM  | VoLTE | Bluetooth | GPS  | Brightness | Torch | Hotpot | NFC  | Fingerprint | Camera | MTP       | Note |
| ----------- | --------- | ---- | ---- | ----- | --------- | ---- | ---------- | ----- | ------ | ---- | ----------- | ------ | --------- | ---- |
| ⭕           | ❓         | ✔    | ✔    | ❌     | ✔         | ✔    | ✔          | ✔     | ✔      | ✔    | ✔           | ✔      | ⭕ADB_ONLY |      |

It should be noted that most GSI based on Android 11 can't start up on verder with Android 11, but can on verder 10 where there are many problems.

## Steps to install
* Step 1 Download GSI, unzip it and get a `*.img` file
* Step 2 Rename the file to `system.img.ext4` and compress it in `.tar` format
* Step 3 Load the compressed file into Odin's AP slot and flash
* Step 4 Press and hold the volume up button and power button during reboot to enter recovery
* Step 5 Select wipe data, then reboot now. Then you will have a new experience.

---
It's was tested on CHC version SM-A6060. Read it in [Chinese](https://github.com/Jason-summer/shuajizhenkuaile/wiki/Samsung-Galaxy-A60).