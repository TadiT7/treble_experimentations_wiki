# Samsung Galaxy S7/S7 edge (Exynos)

General bugs:
- No signal bars shown (signal itself is working fine) **Fixed in GSI ROMS with v118+ patches**
- Offline Charging Working only in MoroKernel 7.1.1 - [Download](https://www.androidfilehost.com/?fid=6006931924117940846) 
- Fingerprint Gestures
- Wi-Fi Direct
- On each boot the first call is muted

## Steps to install

1. Flash heroxlte_createVendor from [here](https://mega.nz/#F!opVUCKCY!jy4WjnNZ2hw4bnQh35T6jQ)
2. Reboot to recovery
3. Flash any downloaded GSI as image-system image (ARM64_AONLY)
4. Flash heroxlte_vendor also from [here](https://mega.nz/#F!opVUCKCY!jy4WjnNZ2hw4bnQh35T6jQ)
5. Optional flash Magisk root

## Steps to revert
1. Reboot to recovery
2. Flash heroxlte_revertVendor from [here](https://mega.nz/#F!opVUCKCY!jy4WjnNZ2hw4bnQh35T6jQ)
3. Reboot to recovery
4. Wipe System,Data,Cache in TWRP wipe menu


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
| Offline Charging          | Working only in MoroKernel 7.1.1 - [Download](https://www.androidfilehost.com/?fid=6006931924117940846)                                              |
| Other feature             | N/A                                                       |
---

Tested By: Project Pizza Testing Group