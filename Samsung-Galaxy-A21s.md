# Device

Summary of what works and doesn't

## Steps to install

* flash gsi image with `fastboot`:
* (Optional But Recommended) ADB sideload the custom kernel `KawaKernel` [A217F](https://drive.google.com/file/d/12F-1mDKqio9j6NTCdddL1YDs6WQ2eCJa/view?usp=sharing)  [A217M](https://drive.google.com/file/d/1yFBIeErICu1BAjr7LE-jsRhsUvF-31OC/view?usp=sharing)
## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| Dual SIM                  | Working                                                   |    
| VoLTE                     | Not working                                               |
| Fingerprint               | Working*                                               |
| NFC                       | N/A                                                   |
| Hotspot / Usb tethering   | Working                                                   |
| MTP                       | Working                                                   |
---

[\*] To Enable Fingerprint, 1. `DO NOT SETUP A PASSCODE DURING SETUP` 2. Disable "com.google.android.setupwizard" (App Name: Android Setup)

### Test Log
Tested By: @yafia - SM-A217F , Firmware Version - arm64_ab_gapps v413 and Corvus OS vS1.0 , Date tested - 2022-05-05

Created By @yafia