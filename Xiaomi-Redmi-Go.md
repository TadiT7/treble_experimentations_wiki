**Follow this link **:https://forum.xda-developers.com/android/software/redmi-aosp-9-t3922192
Preliminary information and warnings
Your warranty is now void, though it's pretty easy to re-flash stock firmware & re-lock the bootloader.

Hardware Support
Camera: Works out of the box (Both back and front)

Speaker / Microphone : Needs further testing but looks good

Bluetooth : Works out of the box

Wi-Fi : Works out of the box

SIM / Mobile Data / Voice : Works out of the box

VoLTE : Device supports VoLTE, but can't test at this moment

Performace : NEED IMPROVEMENT (ihave to modify the build.prop to make the aosp 9 playable)

Google apps : not certified fix by this :https://www.xda-developers.com/how-to-fix-device-not-certified-by-google-error/
***
### Flashing 

***
* Flashing procedure for Redmi Go Global feb 1 2019
* Enable USB debugging and OEM unlock in developer options
* adb reboot bootloader
* fastboot oem unlock / fastboot flashing unlock (Both work and give same result)
* fastboot flash system _your_gsi_path_
* fastboot format userdata
* fastboot reboot

***

working gsi builds 👍 

***

Lineageos 15 go : not good for daily use
Aosp 9 go: still buggy ui bugs slow performance
Aosp 8 go : good for daily use
RR oreo go build : still buggy like lineage os 15
