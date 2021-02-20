# Poco X3 NFC

Tested by [sadyqowl1560](https://github.com/sadyqowl1560).

# - Arm64,AB (**stock vendor**) :

**Steps :**

1- Install last orangefox [here](https://t.me/PocoX3OfficialUpdates/557).

 better to extract recovery.img from zip and install it by fastboot.

2- Boot to recovery , backup super on usb. | for emergency

3- Boot to fastbootd.

4- Install system.img : fastboot flash system system.img.

5- Format data.

6- Reboot system.

**Bugs :**
- Some audio issues. (Fixed) | In phh settings , enable (disable audio effects & use alternate audio policy) 
- Ghost Touch. (Fixed) | push [uinput-goodix.kl](https://del.dog/uinput-goodix.txt) to /system_root/system/usr/keylayout in recovery.
- Sometimes Screen color looks yellow.
- Screen flickering in some gsi.
 