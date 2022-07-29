# Device

Tested with [crDroid-8.7-arm64_bvN-Unofficial.img.xz](https://sourceforge.net/projects/gsi-projects/files/v415/crDroid-8.7/crDroid-8.7-arm64_bvN-Unofficial.img.xz/download) gsi and [Panda-v12.3-eas.zip](https://github.com/Pzqqt/android_kernel_xiaomi_whyred/releases/download/v12.3/Panda-v12.3-eas.zip) kernels.

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Works (use Phh Settings > Misc features > **Force enable Camera2API HAL3**)                                                    |
| Speaker / Mic             | Works (use Phh Settings > Qualcomm features > **Use alternate audio policy** to fix audio in telegram calls) |
| DT2W                      | Works (use Phh Settings > Xiaomi features > **Enable DT2W**) |
| Bluetooth                 | Works                                                     |
| WiFi                      | Works                                                     |
| SIM / Mobile Data / Voice | Works                                                     |
| VoLTE                     | Can't test                                                |
| Fingerprint               | Works                                                     |
| NFC                       | N/A                                                       |
| Offline Charging          | Works                                            |
| Other feature             | Screen sometimes can't wake up (reboot and leave screen on for a ~2-3 mins to fix this), charging indication in notification led is not working|
---