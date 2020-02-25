# [Ulefone S1](https://www.gsmarena.com/ulefone_s1-10036.php)
![Ulefone S1](https://fdn2.gsmarena.com/vv/pics/ulefone/ulefone-s1.jpg)
## Hardware support

| Component                 | Oreo                      | Pie                       | Q                         |
|---------------------------|---------------------------|---------------------------|---------------------------|
| Camera                    | Working , Front only      | Bootloop                  | Bootloop                  |
| Speaker / Mic             | Working                   | Bootloop                  | Bootloop                  |
| Bluetooth                 | Working                   | Bootloop                  | Bootloop                  |
| WiFi                      | Working                   | Bootloop                  | Bootloop                  |
| SIM / Mobile Data / Voice | Working                   | Bootloop                  | Bootloop                  |
| Offline Charging          | Not Working               | Bootloop                  | Bootloop                  |
| Other feature             |                           |                           |                           |
---

## Test Results 
  *  Unofficial LineageOS 15.1 V5 boots
  *  Every other ROM i've tested seems to bootloop or reset the phone at splashscreen.
  *  Requires V24 stock firmware to work (any other firmware as a base doesn't seem to work)

## Additional Info

To get custom roms working, you need V24 stock firmware. Open SP Tool, load V24 scatter file. Replace boot and recovery image with custom ones, provided below. System partition is the one containing Android. Load rom of your choosing there. Use FormatAll+Download option, otherwise you might get stuck at bootanimation.

If calling doesn't work or IMEI is lost after flashing, use this tuturial to restore IMEI
https://forum.hovatek.com/thread-25458.html

Very small /system partition (about ~1GB). Needs resizing (custom scatter file) to enable loading larger roms.


## External links
https://4pda.ru/forum/index.php?s=&showtopic=200800&view=findpost&p=80562065 (boot.img)
https://4pda.ru/forum/index.php?s=&showtopic=911631&view=findpost&p=93047996 (TWRP image)
https://drive.google.com/drive/folders/159eYdv4EVTFPpk6OmlZgbLz7Tu39D6O3 (latest stock firmware)
insert_link (V24 stock firmware)
https://androidfilehost.com/?fid=11410963190603870471 (flashing utility)

***
## Tested By:
* HojnikB
