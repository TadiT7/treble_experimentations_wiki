# [Ulefone S1](https://www.gsmarena.com/ulefone_s1-10036.php)
![Ulefone S1](https://fdn2.gsmarena.com/vv/pics/ulefone/ulefone-s1.jpg)
## Hardware support

| Component                 | Oreo                      | Pie                       | Q                         |
|---------------------------|---------------------------|---------------------------|---------------------------|
| Camera                    | Working , Front only      | Bootloop                  | Bootloop                  |
| Speaker / Mic             | Working                   | Bootloop                  | Bootloop                  |
| Bluetooth                 | Working                   | Bootloop                  | Bootloop                  |
| WiFi                      | Working , Hotspot         | Bootloop                  | Bootloop                  |
| SIM / Mobile Data / Voice | Working , Data Only SIM1  | Bootloop                  | Bootloop                  |
| Offline Charging          | Not Working               | Bootloop                  | Bootloop                  |
| Other feature             |                           |                           |                           |
---

## Test Results 
  *  Unofficial LineageOS 15.1 V5 boots
  *  Every other ROM i've tested seems to bootloop or reset the phone at splashscreen.

## Additional Info

Flash the latest stock firmware with SP Tool. Replace boot and recovery partition with files below 

Boot to stock firmware, enable usb debugging and reboot to recovery. Wipe all partitions and shutdown the phone (don't boot to stock firmware at this point!).
Open SP Tool utility, load stock firmware but untick all partitions except system. Load GSI rom of your chosing and flash.
Reboot the device and if it's a compatible rom, it should boot.

HW wise, it seems to be almost identical to Oukitel C10/Blackview A20. Recovery image however does not work from these devices! 

Very small /system partition (about ~1GB). Needs resizing (custom scatter file) to enable loading larger roms.
    
## External links
https://4pda.ru/forum/index.php?s=&showtopic=200800&view=findpost&p=80562065 (patched boot.img for rooting)

https://4pda.ru/forum/index.php?s=&showtopic=911631&view=findpost&p=93047996 (TWRP image)
https://drive.google.com/drive/folders/159eYdv4EVTFPpk6OmlZgbLz7Tu39D6O3 (stock firmware)
https://androidfilehost.com/?fid=11410963190603870471 (flashing utility)
 ***
 ## Tested By:
* HojnikB
