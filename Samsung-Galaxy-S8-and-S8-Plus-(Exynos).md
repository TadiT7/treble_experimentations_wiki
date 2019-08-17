# Samsung Galaxy S8 and S8 Plus (Exynos)

General bugs:
- No signal bars shown (signal itself is working fine)
- offline charging
- fingerprint gestures
- touchscreen dies after a while with AOD/Ambient display always on (fixable with spamming power button 2-3 times)
- wifi direct

## Steps to install
1. Download a PIE GSI from [[here|Generic-System-Image-(GSI)-list]], use ARM64, A only
2. Put GSI in internal storage
3. Flash treble-convert zip from [here](https://mega.nz/#!LowzWQaL!1FPz7HgKGCvZjNHkaTVaAUiKQ0Sj5JmcBCFGwEIikbc)
4. Reboot to recovery
5. Flash any downloaded GSI as image-system image
6. Flash treble-pie-vendor zip from [here](https://mega.nz/#!T1plkYSZ!7XXrsIxArEc83uHrczJSePRqeIj7gt2k_3YzhN9bcyc)
7. Optional flash Magisk > 19.3

## Steps to revert

1) Reboot to recovery
2) Flash treble-revert zip from [here](https://mega.nz/#!L1hjnCIb!QnCkXV2z3Jdwl-15yi9xd7U-NMRyMvZOsRRmW0bew-8)
3) Reboot recovery
4) Wipe CACHE in twrp wipe menu
5) Flash any non treble rom or restore your previous twrp backup


## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                                   |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Not working                                               |
| Fingerprint               | Working                                                   |
| NFC                       | Working                                                   |
| Offline Charging          | Not working                                               |
| Other feature             | N/A                                                       |
---