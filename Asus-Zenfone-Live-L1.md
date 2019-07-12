 # Asus Zenfone Live L1 (ZA550KL)
![Asus Zenfone Live L1](https://cdn2.gsmarena.com/vv/pics/asus/asus-zenfone-live-l1-za550kl-1.jpg)

Asus Zenfone Live L1 (codenamed "X00RD") is a smartphone from Asus released in May 2018.

## Device specifications

|         Feature         |                            Information                                |
|-------------------------|-----------------------------------------------------------------------|
| Dimensions              | 147.3 x 71.8 x 8.2 mm (5.80 x 2.83 x 0.32 in)                         |
| Supported networks      | GSM / HSPA / LTE                                                      |
| SIM type                | Dual SIM (Nano-SIM, dual stand-by)                                    |
| Voice over LTE          | Yes                                                                   |
| SoC                     | Qualcomm MSM8917 Snapdragon 425 (28 nm)                               |
| CPU                     | Quad-core 1.4 GHz Cortex-A53                                          |
| GPU                     | Adreno 308                                                            |
| Memory                  | (LPDDR3) 2GB/3GB RAM                                                  |
| Storage                 | 16/32 GB Internal                                                     |
| MicroSD                 | microSD, up to 2 TB (dedicated slot)                                  |
| Battery                 | Non-removable Li-Ion 3000 mAh battery                                 |
| Display                 | 720 x 1440 pixels, 18:9 ratio (~293 ppi density), 5.5 inch            |
| Rear Camera             | 13 MP, f/2.0, PDAF                                                    |
| Front Camera            | 5 MP, f/2.4                                                           |
| WLAN                    | Wi-Fi 802.11 b/g/n, Wi-Fi Direct, hotspot                             |
| Bluetooth               | 4.0, A2DP, LE                                                         |
| GPS                     | Yes, with A-GPS, GLONASS, BDS                                         |
| Sensors                 | Accelerometer, gyro, proximity, compass                               |
| Shipped Android version | Android 8.0 Oreo (ZenUI 5)                                            |

Front and back camera both working but with few bugs. Flash on stock camera if set to on or auto the camera will launch to force close. Also the camera have a dark problem on some GSI. If we using the front camera, we will see our face rendered very weird. Also video calling cannot use front camera.

## Steps to install

* Extract the image file (if it compressed, like .zip or .xz format).
* Boot into Fastboot Mode.
* Flash the image file into the System Image partition with Fastboot command :
`fastboot flash system [name of GSI file].img`

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | Working (with bugs)                                       |
| Speaker / Mic             | Working                                                   |
| Bluetooth                 | Working                                                   |
| WiFi                      | Working                                                   |
| SIM / Mobile Data / Voice | Working                                                   |
| VoLTE                     | Working (using a patch)                                   |
| Hotspot                   | Working                                                   |
| Flashlight                | Working                                                   |
| Offline Charging          | Working                                                   |
| Other feature             | Not tested at all                                         |
---

Tested By: AcAciA, Maulana Kurniawan, Satu Prasetyo Gilang Mahameru - ASUS_X00RD, WW-15.01.1902.121 - April 10, 2019 - Template created by @maulaaana, @zguithues and @hackintosh5