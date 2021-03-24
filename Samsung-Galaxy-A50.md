## What works with fixes:
#### [Overlay + Build.prop](https://github.com/RandomAJL/A50-GSI-BugFixes/releases/tag/1.0):
- Auto Brightness
- AOD (Always on display) availability
- Notch + Rounded corners + Status bar height
- Dual SIM
- Proximity Sensor in some apps
#### [Quantum Kernel for GSI's](https://github.com/prashantpaddune/android_kernel_samsung_a50dd/releases/download/v1.1/Quantum_A505F_GSI_V1.1-Magisk-Patched.zip):
- MTP (Transferring files over USB)

## Known Bugs:
- VoLTE
- Bluetooth calls
- In some unlucky devices none of the cameras work. I haven't worked out a solution yet.

## Downloads:
- [ **Odin** ](https://odindownload.com/download/Odin3_v3.14.1.zip)
- [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE)
- [ **Ovarlay + Build.prop** ](https://github.com/RandomAJL/A50-GSI-BugFixes/releases/tag/1.0)
- [ **Quantum Kernal for GSI's** ](https://github.com/prashantpaddune/android_kernel_samsung_a50dd/releases/download/v1.1/Quantum_A505F_GSI_V1.1-Magisk-Patched.zip)
- [ **G-APPs** ](https://opengapps.org/)
- [ **PHH-Magisk** ](https://t.me/a50_offl/117)

## A50 Forums:
- [ **XDA** ](https://forum.xda-developers.com/galaxy-a50)
- [ **Telegram** ](https://t.me/SamsungGalaxyA50)

## Steps to install:

1. Go to settings and search for **_Build Number_** and repeatedly tap the **_Build Number_** until you see a message saying that you have unlocked the developer settings.
2. Next, go to the Developer settings and _**enable OEM unlock**_.
3. Power off the device and boot in download mode with _**vol up + vol down**_ buttons and plug in the USB **_(make sure the USB cable is connected to the pc)_**.
4. In download mode you see the _**long press vol up**_ option for unlock bootloader.
5. Unlock the bootloader **_(that will wipe your device so be sure you made a backup of your data)_**.
6. After bootloader unlock boot up the phone and _make sure it's connected to the internet_, or this will trigger an rmm pre normal error.
7. Set up the phone _without google account_ etc.
8. Reboot into download mode and flash the [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE) recovery **_.tar_** file for your device with [ _**Odin**_ ](https://odindownload.com/download/Odin3_v3.14.1.zip) in the _**AP field**_.
9. Next, Hold _**vol up + power button**_ while [ _**Odin**_ ](https://odindownload.com/download/Odin3_v3.14.1.zip) is flashing until you are in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
10. Format _**cache, data and system**_ in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
11. Flash the [ _**MultiDisabler-Samsung**_ ](https://github.com/ianmacd/multidisabler-samsung/releases) zip in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
11. Flash the [ _**Quantum Kernel for GSI's**_ ](https://github.com/prashantpaddune/android_kernel_samsung_a50dd/releases/download/v1.1/Quantum_A505F_GSI_V1.1-Magisk-Patched.zip) zip in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
12. Flash your chosen GSI .img in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE) as system.
13. Flash the latest available - [ **PHH-Magisk** ](https://t.me/a50_offl/117) in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
14. Flash the [ _**Overlay + Build.prop**_ ](https://github.com/RandomAJL/A50-GSI-BugFixes/releases/tag/1.0) file in [ **TWRP** ](https://drive.google.com/drive/folders/1Kn3_2Kjt-lc3553VF230qY5Wwlhs-crE).
15. _If needed_, flash your chosen [_**G-APPs**_](https://opengapps.org/) file now.
16. Boot into the OS using reboot to recovery. (First Boot may take a while)

## Hardware support:

| Component                 |      Comment                                                        |
|---------------------------|---------------------------------------------------------------------|
| Camera                    | Works mostly (No Wide angle support, front and rear)                |
| Speaker / Mic             | Works                                                               |
| Bluetooth media           | Works                                                               |
| Bluetooth calls           | No                                                                  |
| Wi-Fi                     | Works, both 5GHz & 2.4GHz                                           |
| SIM / Mobile Data / Voice | Works, both SIM1 & SIM2                                             |
| Dual SIM                  | Yes (Some models do not include this feature)                       |
| VoLTE                     | No                                                                  |
| Fingerprint               | Yes                                                                 |
| NFC                       | Yes (Some models do not include this feature)                       |
---	

Created By: [ **RandomAJL** ](https://github.com/RandomAJL) - 26.01.2020

Edited By:  [ **aaronleetw** ](https://github.com/aaronleetw) - Mar 24, 2021

Overlay + Build.prop by [ **RandomAJL** ](https://github.com/RandomAJL)	

#### Many thanks too:	
- [ **prashantp01** ](https://github.com/prashantpaddune) for Quantum Kernel for GSI's	
- [ **redymedan (XDA)** ](https://forum.xda-developers.com/m/redymedan.7915760) for TWRP and Multidisabler	
- PHH-Magisk patched by [ **ExpressLuke** ](https://github.com/ExpressLuke)	
- The main man himself [ **Pierre-Hugues HUSSON** ](https://github.com/phhusson)

#### Changelog:
```
03.24.2021 | aaronleetw | Change TWRP file (pervious one bricks device), added multidisabler, and added new known bug.
```