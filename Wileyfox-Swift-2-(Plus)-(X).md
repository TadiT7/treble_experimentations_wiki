# Wileyfox Swift 2/Plus/X - marmite

## Device Picture

![Wileyfox Swift 2](http://s.4pda.to/pP1NecmKtvq7inv7BoJt2Pld2fU1FH1pNRwu.jpg)

## Hardware Support

* Camera:
> Working on Oreo, requires patch on Pie

* Speaker / Microphone
> Working

* Bluetooth
> Working, however turning it on slows down Wi-Fi connection

* Wi-Fi
> Working

* SIM / Mobile Data / Voice
> Working (can't test VoLTE)

* GPS and Sensors
> Working

* Fingerprint Reader
> Does not work properly on Pie - either does not persist reboot or does not detect finger at all.

***
## Additional Notes
Treble for marmite is unofficial, ported by [vm03](https://4pda.ru/forum/index.php?showuser=785272), [nikith290](https://4pda.ru/forum/index.php?showuser=4331549) and [Hawkjudo](https://4pda.ru/forum/index.php?showuser=6279249) from 4PDA. It needs device repartition. Full instructions are on XDA in English (https://forum.xda-developers.com/swift-2/development/project-treble-wileyfox-swift-2-plus-x-t3848703) and on 4PDA in Russian (https://4pda.ru/forum/index.php?showtopic=894518&view=findpost&p=77365633).


***
## Tested By puuska:
  - ArrowOS Pie: Fingerprints are dumped after reboot, hotspot not working, battery stats needs to be resetted manually
  - PixelExpierience Oreo: Headphones must be routed via Audio Router app
  - OxygenOS sGSI: patches are breaking /vendor partition
  - dotOS Oreo: there are some graphic glitches in chrome on some sites, but everything else seems to work
  - OmniROM Pie: Gapps are crashing
  - Treblized 0-s: Hotspot doesn't work even without secuirty, fingerprints are dumped after reboot, Chrome Canary doesn't load pages (Firefox and Jelly works without problem)
  - MiUI 10 sGSI: bootloop

## Tested by WilhelmErasmus:
  - PixelExperience Pie: Audio works but WiFi Hotspot keeps on being disabled. Fingerprint scanner does not work and camera patch also doesn't work.
  - PixelDust Pie: Camera does not work for more than one consecutive photo using a 3rd-party app - no pre-installed camera. Fingerprints are dumped on reboot.
  - HavocOS Pie: Does not detect sim card during setup although signal is shown in statusbar. It then hangs on verification after warning about Play Certification. I dirty-flashed with PixelDust and the system UI kept crashing. Fingerprints were also dumped on reboot.