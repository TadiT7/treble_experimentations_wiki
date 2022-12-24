Tested images:
AOSP
DerpFest
Corvus
CrDroid
SparkOS
PixelExperience 
CherishOs

Not working:
FOD not working everywhere
Everything works fine except for the fingerprint. 


Steps to install
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img
fastboot -w  # Wipe userdata
Steps to update (if OTA is not working)
fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img
Hardware Support post flashing 