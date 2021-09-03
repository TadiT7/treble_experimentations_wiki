# Summary.
WiFi, Mobile Data, Bluetooth, Fingerprint, Adaptive Brightness, Sound, Microphone work perfectly.

# Before you begin.
You must NOT have magisk installed in your stock ROM, otherwise you'll get a beautiful bootloop, I don't know why... If your phone is rooted, flash the original boot.img before doing anything.

# Steps to Install.
1. Reboot to fastboot.
2. Once you're there, enter fastbootd `fastboot reboot fastboot`
3. Flash vbmeta `fastboot flash --disable-verification vbmeta vbmeta.img`
4. Erase your system partition `fastboot erase system`
5. You may need to delete the product partition as well `fastboot delete-logical-partition product`
6. Flash the GSI `fastboot flash system <image-name.img>`
7. While being on fastbootd, use the volume and power keys to enter recovery mode.
8. Erase all user data (Factory reset.) From recovery... `fastboot -w` Didn't work for me.
9. Use the volume and power keys to reboot the phone and you're good to go.

Support?

* Camera - Yup.
* Mobile Data - Yup.
* Adaptive Brightness - Yup.
* Fingerprint - It triggers the volume control when you use it but it works... So, yup.
* WiFi - Yup.
* Bluetooth - Yup (You need to use the Stock Android 11 firmware, the Android 10 firmware will get you Bluetooth errors.

Tested By: dpkg-i-foo-deb - XT2073-2 RETLA - RPL31.Q2-63-10-2 - 02/09/2021.