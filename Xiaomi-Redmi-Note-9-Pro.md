## Hardware support:
| Component | Status |
|-|-|
| Audio | Working |
| Camera Main | Working|
| Camera Macro | Working in GCAM with Aux |
| Camera Ultrawide | Working in GCAM with Aux |
| Camera Depth Sensor | Working in GCAM as simple 2MP camera. |
| Camera Front Facing | Working
| Speaker / Mic | Working |
| Bluetooth | Working |
| WiFi | Working |
| RIL | Working |
| Double SIM | Working |
| Fingerprint | Working |
| Offline Charging | Working |
| IR blaster | Working |
| ExFat Support | Working|
| VoLTE | Working |

 Working |
| Notch and rounded corners detection | Partially |
| Auto-brightness | Working |

# NOTES

- Random touches when the fingerprint scanner is pressed. Should be fixed in the next builds. I'll make sure I'll remove this after it's fixed https://github.com/phhusson/device_phh_treble/pull/229

- Shuttering when playing media, notifications. Disable audio effects from `Phh Treble Settings > Misc features`

- Random flickering, flickering when changing the brightness / using Adaptive Brightness. Force alternate backlight scale from `Phh Treble Settings > Misc features`

- Because this is a GSI the notch isn't fully detected. While on default DPI everything looks okay, on higher DPI will cover a little bit of the notification shade

- For VoLTE to work install IMS apk from `Phh Treble Settings > IMS features` and check `Force the presence of 4G calling.

If you find any bugs/fixes feel free to edit this page.