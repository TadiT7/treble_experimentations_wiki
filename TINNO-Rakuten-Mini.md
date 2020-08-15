# The world's smallest Snapdragon-powered Treble-enabled phone
<img src="https://network.mobile.rakuten.co.jp/assets/img/product/rakuten-mini/image-04.png" width="600">

## Bootloader Unlocking
1. Tap "Software version" in Settings menu a few times
2. Enter *636865625# on the dial pad
3. Open Developer options and enable OEM unlocking
4. Reboot to bootloader and run `fastboot flashing unlock` and `fastboot flashing unlock_critical`
5. (Optional) Install Magisk with [TWRP](https://drive.google.com/drive/folders/15LQok1lNR55gutIScnle6KIp6fdhwhR7?usp=sharing)

## Before installation
Rakuten Mini is released with Android 9 but vendor implementation is a bit broken. When you install Android 10 GSI, you have to install [this Magisk Module](https://github.com/AndroPlus-org/magisk-module-c330-gsi/releases) or [modded vendor image](https://drive.google.com/file/d/1_YDpV9-Wbbbvdjd2eGF1ofSGorc8xaq9/view?usp=sharing). Otherwise the phone will bootloop at home screen.

## Hardware support
| Component | Status |
|-|-|
| Audio | Working |
| Camera Main | Working|
| Camera Front | Working
| Speaker / Mic | Working |
| Bluetooth | Working |
| Wi-Fi | Working |
| RIL | Working |
| eSIM | Working (Need patch for adding eSIM) |
| Offline Charging | Working |
| VoLTE | Working (Need patch) |
| Auto-brightness | Need patch |
| NFC | Working |
| FeliCa / Osaifu Keitai | Not working |

Tested by AndroPlus_org
- Model: TINNO Rakuten Mini C330
- Vendor: [C330AE_9.0_RMN_JP_72_SS](https://drive.google.com/drive/folders/1m_IjpigWlYz35E_SJdQrfMLNpMVS_dKc?usp=sharing) (Modded)
- GSI: Android 10 arm64 A/B