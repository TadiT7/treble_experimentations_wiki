THIS GUIDE IS INCOMPLETE : PLEASE DONT FOLLOW IT RIGHT NOW !

# Instructions to install GSI :

## 1. Unlock Bootloader

>Bootloader unlock tools    
For Realme UI 1 : [Get here](https://www.mediafire.com/file/4cy9u8r2yu9ve9t/DeepTest_realme_Narzo20.apk/file)  
For Realme UI 2 : [Get here](https://www.mediafire.com/file/8l33d9kxlxkdc80/DeepTesting_realme-release_20210426_newID_signed.apk/file)

>Vbmeta
For Realme UI 1 : [Get here](https://www.mediafire.com/file/0svn1vj1pn7buy7/vbmeta.img/file)  

Guide to unlock bootloader : [Get here](https://telegra.ph/How-to-unlock-bootloader-03-02)

## 2. After unlocking bootloader and rebooting device, shut it down again and enter fastboot mode by pressing vol minus and power button together

Assuming that you've already installed [Platform tools](https://developer.android.com/studio/releases/platform-tools) and is aware how to start the adb-fastboot shell , open platform tools in terminal/CMD (depending on os) and follow these steps

`adb reboot bootloader `
`fastboot reboot fastboot`
`# Your device will boot to recovery , dont touch anything in recovery, just focus on the commands below`
`fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`
`fastboot reboot fastboot`
`fastboot erase system`
`fastboot reboot fastboot`
`fastboot flash system system.img`
`fastboot -w`
`fastboot reboot bootloader`
`fastboot erase userdata`
`fastboot reboot`

