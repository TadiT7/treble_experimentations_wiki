Here are the tests that have been done for every release:

AOSP v19 2018-06-03:
- Razer phone: system-arm64-ab-gapps-su.img: dirty flashed, boots, fde ok, bluetooth inits, wifi connects, aosp camera back preview, MGC back preview & snap
- Google Pixel 2 XL: system-arm64-ab-gapps-su.img: dirty flashed, fbe ok, bluetooth inits, wifi connects, aosp camera back preview, MGC back preview & snap
- Cubot X18 Plus: system-arm64-aonly-gapps-su.img: dirty flashed, boots, fde ok, bluetooth inits, wifi connects, aosp camera back preview & snap
- Blackview A20: system-arm-aonly-go-su.img: clean flashed, boots, bluetooth inits, wifi connects, aosp camera & front preview & snap, fde ok
- Lenovo Moto E5: system-arm-aonly-go-su.img: clean flashed, boots, gapps crash (bad Gapps/Go integration), bluetooth inits, aosp camera **no-ok**, fde ok, fingerprint ok
- Huawei Mate 9: system-arm64-aonly-gapps-su.img: dirty flashed, boots ok, 4g ok, ingoing and outgoing 3G calls ok, bluetooth inits, fp gestures ok, fp swipe for notifications ok, fp ok, fbe ok, aosp cam back preview & snap ok, MGC back previwe & snap, jack routing **blinking**
- Allview Viper V3: system-arm64-aonly-vanilla-nosu.img: clean flashed, boots, bluetooth inits, aosp cam back preview & snap, fde ok, fp ok, wifi connects
- Honor View 10: system-arm64-aonly-gapps-su.img, clean flashed, pass setup wizard (no sim, wifi, gg account, fresh start, voice match), sdcard read ok, jack detection ok, jack routing **blinking**, MGC back preview & snap ok