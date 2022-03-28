# Moto G9 (Guamp)

<img src="https://fdn2.gsmarena.com/vv/bigpic/motorola-moto-g9.jpg" width="200" height="250" /> <img src="https://fdn.gsmarena.com/imgroot/news/20/08/motorola-moto-g9-announcement/-315/gsmarena_003.jpg" width="250" height="250" />

# Device Specification

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 4x2.0 GHz Kryo 260 Gold & 4x1.8 GHz Kryo 260 Silver
Chipset | Qualcomm SD6115 Snapdragon 662
GPU     | Adreno 610
Memory  | 2/3/4GB
Shipped Android Version | 10.0 (Q)
Internal Storage | 64/128GB
microSD | Up to 512 GB (uses shared SIM slot)
Battery | 5000 mAh
Dimensions | 165.2 x 75.7 x 9.2 mm
Display | 720 x 1600  pixels, 6.5-inch IPS LCD
Rear Camera  | 48 MP, f/1.7, (wide), 1/2.0", 0.8µm, PDAF, 2 MP, f/2.4, (macro), 2 MP, f/2.4, (depth)
Front Camera | 8 MP (f/2.2, 1.12µm, HDR)

# Installation Process

* Unlock the `bootloader` using the documentations provided by motorola.
* Factory reset the device
* Power off the device and reboot to `fastboot` using key combinations `(Vol Down + Power)`
* Connect to PC with platform tools and drivers installed
* Reboot to fastbootd using fastboot utility
     ```
     $ fastboot reboot fastboot
     ```
* Erase the system partition
     ```
     $ fastboot erase system
     ```
* Note down the slot name. eg: `a for system_a` and `b for system_b`
* Delete the logical partition of product
     ```
     $ fastboot delete-logical-partition product_a [Replace the alphabet with the previously noted one]
     ```
* Download the gsi file and flash the system image
     ```
     $ fastboot flash system system.img [Replace with the file name]
     ```
* Wipe the userdata
     ```
     $ fastboot -w
     ```
* Reboot the device
     ```
     $ fastboot reboot
     ```

# Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working                                              |
| Speaker / Mic             | Working                                              |
| Bluetooth                 | Working                                              |
| WiFi                      | Working                                              |
| SIM / Mobile Data / Voice | Working                                              |
| VoLTE                     | Working [When IMS configured via app]                |
| Fingerprint               | Working                                              |
| NFC                       | Not Working                                          |
| Offline Charging          | Working                                              |
| Boot                      | Working                                              |

Tested By: Rajin Gangadharan [telegram: @rajinTechie]

Model Tested: XT2083-3