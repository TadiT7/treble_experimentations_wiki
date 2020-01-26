# Samsung Galaxy A50

## What works with fixes:
#### [Overlay + Build.prop](https://t.me/a50_offl/54):
- Auto Brightness
- AOD (Always on display)
- Notch + Rounded corners
- Duel SIM
- Proximity Sensor
#### [SkyKernal for GSI's](https://drive.google.com/file/d/1bhFn7FDPzV9059wJ-dP6CefiPRwp4hDO/view?usp=sharing):
- MTP (Transfering files over USB)

## Known Bugs:
- Fingerprint reader
- VoLTE
- Bluetooth Calls
- Rebooting when _**AOD** (Always On Display)_ is turned off

## Downloads:
- [ **Odin** ](https://odindownload.com/download/Odin3_v3.14.1.zip)
- [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE)
- [ **SkyKernal for GSI's** ](https://drive.google.com/file/d/1bhFn7FDPzV9059wJ-dP6CefiPRwp4hDO/view?usp=sharing)
- [ **A50.overlay+prop.zip** ](https://t.me/a50_offl/54)
- [ **G-APPs** ](https://opengapps.org/)
- [ **PHH-Magisk** ](https://t.me/a50_offl/117)

## Steps to install:

1. Go to settings and search for **_Build Number_** and repeatedly tap the **_Build Number_** until you see a message saying that you have unlocked the developer settings.
2. Next, go to the Developer settings and _**enable OEM unlock**_.
3. Power off the device and boot in download mode with _**vol up + vol down**_ buttons and plug in the USB **_(make sure the USB cable is connected to the pc)_**.
4. In download mode you see the _**long press vol up**_ option for unlock bootloader.
5. Unlock the bootloader **_(that will wipe your device so be sure you made a backup of your data)_**.
6. After bootloader unlock boot up the phone and _make sure it's connected to the internet_, or this will trigger an rmm pre normal error.
7. Set up the phone _without google account_ etc.
8. Reboot into download mode and flash the [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE) recovery **_.tar_** file for your device with [ _**Odin**_ ](https://odindownload.com/download/Odin3_v3.14.1.zip) in the _**AP field**_.
9. Next, Hold _**vol up + power button**_ while [ _**Odin**_ ](https://odindownload.com/download/Odin3_v3.14.1.zip) is flashing until you are in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE).
10. Format _**cache, data and system**_ in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE).
11. Flash the [ _**SkyKernal for GSI's**_ ](https://drive.google.com/file/d/1bhFn7FDPzV9059wJ-dP6CefiPRwp4hDO/view?usp=sharing) zip in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE).
12. Flash your chosen GSI .img in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE) as system.
13. Flash the latest available - [ **PHH-Magisk** ](https://t.me/a50_offl/117) in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE).
14. Flash the [ _**A50.overlay+prop.zip**_ ](https://t.me/a50_offl/54) file in [ **TWRP** ](http://gofile.me/4xNLJ/Plj8vFfFE).
15. _If needed_, flash your chosen [_**G-APPs**_](https://opengapps.org/) file now.
16. Boot into the OS using reboot to recovery. (First Boot may take a while)

## Hardware support:

| Component                 |      Comment                                                        |
|---------------------------|---------------------------------------------------------------------|
| Camera                    | Works mostly (No Wide angle support, front and rear)                |
| Speaker / Mic             | Works                                                               |
| Bluetooth media           | Works                                                               |
| Bluetooth calls           | No                                                                  |
| WiFi                      | Works, both 5GHz & 2.4GHz                                           |
| SIM / Mobile Data / Voice | Works, both SIM1 & SIM2                                             |
| Dual SIM                  | Yes                                                                 |
| VoLTE                     | No                                                                  |
| Fingerprint               | No                                                                  |
| NFC                       | Yes                                                                 |
---