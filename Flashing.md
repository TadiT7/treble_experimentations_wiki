
Flashing procedure for Redmi Go Global version feb 1 2019
Enable USB debugging and OEM unlock in developer options
adb reboot bootloader
fastboot oem unlock / fastboot flashing unlock (Both work and give same result)
fastboot flash system _your_gsi_path_
fastboot format userdata
fastboot reboot