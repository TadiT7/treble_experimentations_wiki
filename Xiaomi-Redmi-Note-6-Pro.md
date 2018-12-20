![Xiaomi Redmi Note 6 Pro](https://img.timesnownews.com/story/1544521578-Xiaomi_Redmi_Note_6_Pro_colours.jpg)

The Xiaomi Redmi Note 6 Pro (codenamed _"tulip"_) is a mid-range smartphone from Xiaomi announced in September 2018.

## Device specifications

|                         |                                                                       |
| ----------------------- | :-------------------------------------------------------------------- |
| Dimensions              | 157.9 x 76.4 x 8.3 mm                                                 |
| Supported networks      | GSM / HSDPA / LTE                                                     |
| SIM type                | Hybrid Dual SIM (Nano-SIM, dual stand-by)                             |
| Voice over LTE          | Yes                                                                   |
| SoC                     | Qualcomm SDM660 Snapdragon 636                                        |
| CPU                     | 8x Qualcomm® Kryo™ 260 CPU                                            |
| GPU                     | Adreno 509                                                            |
| Memory                  | (LPDDR4X) 3GB/4GB (Global); 6GB RAM (India)                           |
| Storage                 | 32/64GB eMMC 5.1 flash storage                                        |
| MicroSD                 | Up to 256 GB                                                          |
| Battery                 | Non-removable Li-Po 4000 mAh                                          |
| Display                 | 2280 x 1080 (19:9), 6.26 inch                                         |
| Rear camera 1           | 12 MP, f/1.9, 1/2.55", 1.4µm, dual pixel PDAF                         |
| Rear camera 2           | 5 MP, f/2.2, 1.12µm, depth sensor                                     |
| Front camera 1          | 20 MP, f/2.0, 0.9µm                                                   |
| Front camera 2          | 2 MP, f/2.2, 1.75µm, depth sensor                                     |
| WLAN                    | Wi-Fi 802.11 a/b/g/n/ac, dual-band, Wi-Fi Direct, hotspot             |
| Bluetooth               | 5.0; Supported protocols: A2DP, Bluetooth Low Energy                  |
| GPS                     | Supported (A-GPS, GLONASS, BDS)                                       |
| Sensors                 | Fingerprint (FPC/Goodix), IR, gyro, accelerometer, proximity, compass |
| Shipped Android version | 8.1.0 (MIUI 9)                                                        |

## What is buggy in Phh-Treble

## Hardware support

### Display
- Display cutout recognition doesn't work (third-party fixes available)
- Brightness regulation will make the screen flicker (third-party fixes available)

### RIL (SIM detection, ingoing/outgoing calls, SMS...)
- RIL works without any noticeable problem
- Dual SIM wasn't tested

### VoLTE and ViLTE
VoLTE and ViLTE will not work. This is a vendor related problem.

### Speaker and microphone
Working normally.

### Camera
- Basic point-and-shoot photo/video taking is working normally
- Camera2 API testing is needed

### Wi-Fi
- Connection to 2.4GHz/5GHz networks is working normally
- Hotspot wasn't tested.

### Bluetooth
- A2DP doesn't work
- Hands-free mode (carkit / in-call earpieces) wasn't tested
- Bluetooth Low Energy wasn't tested

### Fingerprint reader
- FPC works
- Some say Goodix doesn't work (please check)
- Tapping on the fingerprint sensor triggers an event which "clicks" on the first available action of the opened application (third-party fixes available)

### 3.5mm audio jack
Working normally.

### USB
- MTP and PTP don't work.
- ADB works.
- USB charging works.
- USB with external DAC wasn't tested.

### Other features

- Power profiles don't work (Unable to see apps' and hardware's battery stats' details)
- Widevine support wasn't tested (although DRM Info shows Widevine)
- Miracast isn't tested
- Notification LED sometimes remains active
  - When rebooting (workaround: power off, then power on)
  - When receiving notifications (this is completely random)
  - When powering on normally (this is completely random)
- Battery charging seems to prevent the notification LED from blinking in some Custom ROMs (tested on AEX 6.0)

## Additional Notes

### XDA Thread
Check: https://forum.xda-developers.com/redmi-note-6-pro/how-to/redmi-note-6-pro-project-treble-t3864694

## Tested by:
* @AryToNeX - tulip 4/64GB - December 20, 2018

Template created by @zguithues, with additions by @AryToNeX