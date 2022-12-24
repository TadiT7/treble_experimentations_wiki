### **Tested images:**

* AOSP
* DerpFest
* Corvus
* CrDroid
* SparkOS
* PixelExperience 
* CherishOs

### **Not working:**

* _**FOD not working everywhere**_
* Everything works fine except for the fingerprint. Need [two ](https://mega.nz/folder/mEhWlZIS#hrI1QyOOkRk6nmKPx79rfg) overlays for normal statusbar display


### **Steps to install:**

fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img
fastboot -w  # Wipe userdata

### **Steps to update (if OTA is not working)**

fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img

Hardware Support post flashing 