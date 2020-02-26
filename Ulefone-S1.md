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
---

## Test Results 
  *  Treble ROMs require V24 stock firmware to work (any other firmware as a base doesn't seem to work)
  *  Unofficial LineageOS 15.1 V5 boots
  *  Every other ROM i've tested seems to bootloop or reset the phone at splashscreen. Needs more testing/patching
  *  USSD commands (like checking for credit status) don't work properly.


## Custom ROMs

To get custom roms working, you need V24 stock firmware. Open SP Tool, load V24 scatter file. Replace boot and recovery image with custom ones, provided below. System partition is the one containing Android. Load rom of your choosing there. Use FormatAll+Download option, otherwise you might get stuck at bootanimation.

If calling doesn't work or IMEI is lost after flashing, use this tuturial to restore IMEI
https://forum.hovatek.com/thread-25458.html
If calling still doesn't work, try RIL patch below.

## Additional Info

Very small /system partition (about ~1GB). Needs resizing (custom scatter file) to enable loading larger roms.
First few boots of Treble ROMs can be slow. Rom should settle over time and run smoothly.


## External links
https://mega.nz/#!cokRjDRL!VwhG8GF-lXu2p5GOefy9JYD8oRCfelHJ79KBzaoFr3o (boot.img)
https://mega.nz/#!og91UZxA!vhi_3CPZ3U5QKQAHS66akF3XcTADF3tv3vF67DaWhx4 (TWRP image)
https://mega.nz/#!Y4lVXDTT!Aalfgy5T1vXh-Gwpovp2wOPisX6FRD3T8Os0LX2GZXI (stock firmware)
https://mega.nz/#!Zgs30bQa!R4lYzzDq_TL4rff-JwiKEln5FnXho6M5yUA6wMqujQI (V24 firmware)
https://mega.nz/#!l99j0biJ!R2S-0ByoNm9M_vhq_OyKlXz8Xu08G_knmSc6Zud-fTU (SP flashing utility)
https://mega.nz/#!pp1jABZA!MwAyk5mUIsLySxEiK9RzIME4X0TI6KcsKOG9P7KqSQs (LineageOS rom)
https://mega.nz/#!xtsjXbBR!FExjQBxBhtax9zjjymSFyCwQ8ArqWl3skuy2i2Nibro (RIL patch)

Patched boot.img, TWRP, RIL patch provided by 4PDA.ru community, LineageOS rom provided by phhusson.
Stock images provided by Ulefone.

***

## Testing by:
* HojnikB
