# Tested images

Mostly working fine (see Hardware support bellow)

- [PixelExperience_Plus_arm64-ab-13.0-20230104-UNOFFICIAL.img.xz](https://github.com/ponces/treble_build_pe/releases/download/v2023.01.04-plus/PixelExperience_Plus_arm64-ab-13.0-20230104-UNOFFICIAL.img.xz)

# Steps to install

```
1. Unlock bootloader first
2. Use miflash to flash latest fastboot package from xiaomi
3. boot into MIUI first
4. reboot to fastboot, and type "fastboot reboot fastboot"
5. fastboot flash system your_gsi_rom_of_choice.img
```

# Steps to update (if OTA is not working)

```
fastboot reboot fastboot
fastboot flash system your_gsi_rom_of_choice.img
```

# Hardware Support post flashing

| Component | Comment |
| --- | --- |
| Camera | [Works](#notes) |
| Speaker/Mic | Works |
| Bluetooth | [Works with tweak](#notes) |
| Wi-Fi | Works |
| SIM/Mobile Data/Voice | Works (Without 5G) |
| VoLTE | Not working |
| Fingerprint | Works |
| Display Refresh rate | 60Hz (90Hz/30Hz in phh settings) |
| Screen Brightness | Works |
| Volume scale | Works |
| 5G | [Works](#notes) |
| SafetyNet post root | Not Tested |

# Notes

- For bluetooth, enable "Use System Wide BT HAL", also see [here](https://github.com/phhusson/treble_experimentations/issues/2501)
- When you using 5G, calls and sms aren't working
- Camera works badly