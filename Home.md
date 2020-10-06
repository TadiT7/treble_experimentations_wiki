![android GSI](https://i.imgur.com/cJJ0zxQ.png)
### What is Project Treble, GSI, etc?
Here's [[Frequently Asked Questions (FAQ)]].

### Device List

Devices where someone has claimed to have successfully booted a version of phh's generic system image are recorded here.  The level of hardware support (e.g. Wi-Fi, NFC, Bluetooth...) may vary; please refer to the device-specific page for comments on hardware support.

**Device testers/maintainers:**  In addition to hardware support information, please record or give a pointer to at least one known-good factory-image/system-image configuration in a device-specific page (i.e. when a system image successfully boots on your device, please let others know what system image you used and what factory image you flashed over top of, and also any special flashing instructions).  There is a device-specific wiki template here:  [[New-Devices-Template-WIP]].

**ROMs:** Check available GSI ROMs here [[Generic System Image (GSI) list]].

**How to build a GSI?** : Check this guide here [[How to build a GSI?]]

**How to create a device overlay?** : Check this guide here [[How to create an overlay?]]

**Why should I use GSI for A/B devices to some A-only devices?** : On Android 9, Google changed the requirements and all devices shipped with Android 9 must use "[system-as-root](https://source.android.com/devices/bootloader/system-as-root)". Before this change, only A/B devices were system-as-root and GSI name was separated by A-only and A/B. For this historical reasons, you have to use GSI for A/B on the devices shipped with Android 9+.

|Device Name|Codename|Support from OEM|Image Type|Architecture|
|:-:|:-:|:-:|:-:|:-:|
|[[Alcatel 5V 5060D]]|n/a||A|arm64|
|[[Alldocube M5]]|n/a|✓|A|arm64|
|[[Alldocube Power M3]]|n/a|✓|A|arm64|
|[AllView V3 Viper](https://github.com/phhusson/treble_experimentations/wiki/Casper-Via-M4-(AllView-V3-Viper))|V3_Viper|✓|A|arm64|
|[[Amazon Kindle Fire HD 10 2019]]|maverick|✓|A|arm_binder64|
|[[Asus ROG Phone (ZS600KL)]]|Z01QD|✓|A/B|arm64|
|[[Asus ROG Phone II (ZS660KL)]]|I001D|✓|A/B|arm64|
|[[Asus ROG Phone III]]|I003D|✓|A/B|arm64|
|[[Asus Zenfone 4 (ZE554KL)]]|Z01KD|✓|A|arm64|
|[[Asus Zenfone 5 (ZE620KL)]]|X00QD|✓|A|arm64|
|[Asus Zenfone 5Z (ZS620KL/ZS621KL)](https://github.com/phhusson/treble_experimentations/wiki/Asus-ZenFone-5Z)|Z01R|✓|A/B|arm64|
|[[Asus Zenfone 7/Pro (ZS670KS/ZS671KS)]]|I002D|✓|A/B|arm64
|[[Asus Zenfone Go]]|Z00VD|✓ (Go)|A|arm|
|[[Asus Zenfone Max M1 (ZB555KL)]]|X00PD|✓|A/B|arm64|
|[[Asus Zenfone Max M1 (ZB556KL)]]|X00PD|✓|A/B|arm64|
|[[Asus Zenfone Max M2 (ZB632KL)]]|X01AD|✓|A/B|arm64|
|[[Asus Zenfone Max M2 (ZB633KL)]]|X01AD|✓|A/B|arm64|
|[[Asus Zenfone Max Pro M1]]|X00TD|✓|A|arm64|
|[[Asus Zenfone Max Pro M2]]|X01BD|✓|A|arm64|
|[Asus Zenfone Max Shot and Max Plus M2](https://github.com/phhusson/treble_experimentations/wiki/ASUS-ZenFone-Max-Shot-and-Max-Plus-M2)|A001D|✓|A|arm64|
|[Barnes & Noble Nook Tablet 10.1" (BNTV650)](https://github.com/phhusson/treble_experimentations/wiki/Barnes-&-Noble-Nook-Tablet-10.1%22)|st18c10bnn|✓|A|arm64|
|[[Barnes & Noble Nook Tablet 7" 2018 (BNTV460)]]|st18c7bnn|✓ (Go)|A|arm|
|[[Blackview A20]]|a20|✓ (Go)|A|arm|
|[[Blackview A60]]|a60|✓ (Go)|A|arm|
|[[Blackview A60 Pro]]|a60_pro|✓|A/B|arm64|
|[[Blackview BV9500]]|s32v63c2k_jk|✓|A|arm64|
|[[Blackview BV9500 Plus]]|s62v71c2k_jk_eea|✓|A/B|arm64|
|[[Blackview BV9500 Pro]]|s32v63c2k_jk_pro|✓|A|arm64|
|[[Blackview BV9600 Pro]]|n/a|✓|A or A/B|arm64|
|[[BLU Vivo XL4]]|V0350WW|✓|A|arm64|
|[[Bluboo D6]]|D6|✓|A|arm|
|[[BQ-mobile S-5020 Strike]]|n/a||A|arm|
|[[BQ Aquaris C]]|jeice|✓|A|arm|
|[[Brown&Proud Brown 1]]|V4701_I01||A|arm64_32
|[[Cherry Mobile Flare S8]]|X930|✓|A/B|ARM64|
|[[Cherry Mobile Flare S8 Pro]]|Flare_S8_Pro|√|A/B|ARM64|
|[[Cherry Mobile Flare S8 Plus]]|FS8Plus|√|A/B|arm64|
|[[Cherry Mobile Flare S8 Max]]|Flare_S8_Max|√|A/B|arm64|
|[[Cherry Mobile Flare S8 Prime]]|Flare_S8_Prime|√|A/B|arm64|
|[[Cherry Mobile Flare S8 Lite]]|Flare_S8_Lite|√|A/B|arm_binder64|
|[[Chuwi Hi9 Air]]|Hi9Air|✓|A|arm64|
|[[Coolpad C558]]|k39tv1|✓ (Go)|A|arm|
|[[Coolpad Cool Changer 1C]]|c107||A|arm64|
|[[Coolpad Cool Changer S1]]|c105||A|arm64|
|[[Cosmo Communicator]]|Cosmo||A|arm64|
|[[Cubot Quest]]|Cubot QUEST|✓|A|arm64|
|[[Cubot P20]]|p20|✓|A|arm64|
|[[Cubot X18 Plus]]|Cubot_X18_Plus||A|arm64|
|[[Cubot X19]]|x19|✓|A/B|arm64|
|[[DEXP A140]]|a140|✓|A|arm|
|[[DEXP A240]]|a240|✓|A|arm|
|[[DEXP B260]]|b260|✓|A|arm|
|[[DEXP BL250]]|bl250|✓|A|arm|
|[[DIGMA VOX V40 3G]]|VT4055MG|✓|A (Go)|arm|
|[[Doogee X5]]|X5|✓|A|arm|
|[[Doogee X5 Max]]|X5max|✓|A|arm|
|[[Doogee X5 Max Pro]]|X5max_PRO|✓|A|arm|
|[[Doogee X5 Pro]]|X5pro|✓|A|arm|
|[[Doogee X50]]|X50|✓|A|arm|
|[[Doogee Y8]]|Y8|✓|A/B|arm64|
|[[Duoqin Qin 2]]|sp9832e_1h10_go|✓|A/B (Go)|arm64|
|[[Duoqin Qin 2 Pro]]|s9863a1h10|✓|A/B|arm64|
|[[Elephone Soldier]]|n/a|✓|A|arm64|
|[[Elephone U Pro]]|U_Pro|✓|A/B|arm64|
|[[Essential PH-1]]|mata|✓|A/B|arm64|
|[[Fairphone 3]]|FP3|✓|A/B|arm64|
|[[F(x)tec Pro1]]|QX1000|✓|A/B|arm64|
|[[General Mobile GM 5]]|GM5_sprout||A|arm64|
|[[General Mobile GM 5 Plus]]|shamrock / GM5PlUS_sprout||A|arm64|
|[[General Mobile GM 8]]|GM8_sprout|✓|A/B|arm64|
|[[General Mobile GM 8 Go]]|GM8_go_sprout|✓ (Go)|A|arm|
|[[General Mobile GM 9 Pro]]|GM9PRO_sprout|✓|A/B|arm64|
|[[GOME U9]]|n/a|✓|A|arm64|
|[[Google Pixel and Pixel XL]]|sailfish and marlin|✓|A/B|arm64|
|[[Google Pixel 2 and Pixel 2 XL]]|walleye and taimen|✓|A/B|arm64|
|[[Google Pixel 3 and Pixel 3 XL]]|blueline and crosshatch|✓|A/B|arm64|
|[[Google Pixel 3a and Pixel 3a XL]]|sargo and bonito|✓|A/B|arm64|
|[[Google Pixel 4 and Pixel 4 XL]]|flame and coral|✓|A/B|arm64|
|[[Google Pixel 4a]]|sunfish (LTE) and bramble (5G)|✓|A/B|arm64|
|[[Google Pixel 5]]|redfin|✓|A/B|arm64|
|[[HTC U11]]|ocn||A|arm64|
|[HTC U11 Life](https://github.com/phhusson/treble_experimentations/wiki/HTC-U11-life-(Android-One))|ocl|✓|A/B|arm64|
|[[HTC U11 Plus]]|ocm|✓|A|arm64|
|[[HTC U12 Plus]]|ime|✓|A/B|arm64|
|[[Huawei Honor 6X]]|berlin / bln|✓|A|arm64|
|[[Huawei Honor 7A]]|dua|✓|A|arm64|
|[[Huawei Honor 7A Pro]]|aum|✓|A|arm64|
|[[Huawei Honor 7C]]|aum|✓|A|arm64|
|[[Huawei Honor 7C Pro]]|lnd|✓|A|arm64|
|[[Huawei Honor 7X]]|bnd|✓|A (A/B when updated to EMUI 9)|arm64|
|[[Huawei Honor 8]]|frd|✓|A|arm64|
|[[Huawei Honor 8 Lite]]|pra|✓|A|arm64|
|[[Huawei Honor 8 Pro]]|duk|✓|A|arm64|
|[[Huawei Honor 8X Max]]|ARE-AL00|✓|A (A/B when updated to EMUI 9)|arm64|
|[[Huawei Honor 9]]|stf|✓|A|arm64|
|[[Huawei Honor 9 Lite]]|lld|✓|A|arm64|
|[[Huawei Honor V8]]|knt|✓|A|arm64|
|[[Huawei Honor View 10]]|berkeley / bkl|✓|A|arm64|
|[[Huawei Mate 9]]|mha|✓|A|arm64|
|[[Huawei Mate 10]]|alp|✓|A|arm64|
|[[Huawei Mate 10 Lite]]|rne|✓|A|arm64|
|[[Huawei Mate 10 Pro]]|blanc / bla|✓|A|arm64|
|[[Huawei Mate SE]]|bnd|✓|A|arm64|
|[[Huawei MediaPad M5 Lite]]|BAH2||A|arm64|
|[[Huawei MediaPad M5 Pro]]|Cameron Pro / CMR-AL19|?|A/B|arm64|
|[[Huawei P Smart]]|fig|✓|A|arm64|
|[[Huawei P Smart (2019)]]|pot|✓|A|arm64|
|[[Huawei P Smart Z]]|stk|✓|A|arm64|
|[[Huawei P8 Lite (2017)]]|prague / pra|✓|A|arm64|
|[[Huawei P9]]|eva|✓|A|arm64|
|[[Huawei P9 Lite]]|vns|✓|A|arm64|
|[[Huawei P9 Plus]]|vienna / vie|✓|A|arm64|
|[[Huawei P10 and P10 Plus]]|vtr and vky|✓|A (A/B when updated to EMUI 9)|arm64|
|[[Huawei P10 Lite]]|was|✓|A|arm64|
|[[Huawei P20]]|eml|✓|A|arm64|
|[[Huawei P20 Lite]]|ane|✓|A (A/B when updated to EMUI 9)|arm64|
|[[Huawei P20 Pro]]|charlotte / clt|✓|A (A/B when updated to EMUI 9)|arm64|
|[[Huawei P30]]|ele|✓|A/B|arm64|
|[[Huawei P30 Lite]]|mar|✓|A/B|arm64|
|[[Huawei P30 Pro]]|vog|✓|A/B|arm64|
|[Huawei Y6 / Y6 Prime (2018)](https://github.com/phhusson/treble_experimentations/wiki/Huawei-Y6-(2018)-&-Y6-Prime-(2018))|atu|✓|A|arm64|
|[[Huawei Y9 (2018)]]|fla|✓|A|arm64|
|[[Infinix Hot 8]]|x650|✓|A/B|arm_binder64|
|[[Infinix Note 5]]|x604|✓|A/B|arm64|
|[[Infinix Note 6]]|x610|✓|A/B|arm64|
|[[Infinix Zero 6]]|x620|✓|A/B|arm64|
|[[INOI 2 Lite]]|n/a|✓|A|arm|
|[[Itel A32F]]|f8007|✓ (Go)|A|arm|
|[[Jinga Start LTE]]|ji50ag1_169hp|✓|A|arm|
|[[Koolnee Rainbow]]|rainbow|✓ (Go)|A|arm|
|[[Lava Z50]]|z50|✓ (Go)|A|arm|
|[[Leagoo M8 Pro]]|M8_Pro|✓|A|arm|
|[[Leagoo M9 Pro]]|M9_Pro|✓|A|arm (arm_binder64)|
|[[Leagoo M13]]|M13||A/B|arm64|
|[[Leagoo Power 2]]|Power_2|✓|A|arm|
|[[Leagoo Power 5]]|Power_5|✓|A|arm64|
|[[Leagoo T8s]]|T8s|✓|A|arm64|
|[[LeEco Le 2]]|s2||A|arm64|
|[[LeEco Le Max 2]]|x2||A|arm64|
|[[LeEco Le Pro 3]]|zl1||A|arm64|
|[[Lenovo K5 Note / K9 Note]]|L38012|✓|A|arm64|
|[[Lenovo K5 Play]]|L38011|✓|A|arm64|
|[[Lenovo K6 / K6 Power]]|karate||A/B|arm64|
|[[Lenovo K6 Note / K6 Plus]]|karatep||A/B|arm64|
|[[Lenovo K8 Note]]|manning||A|arm64|
|[[Lenovo P2]]|kuntao||A|arm64|
|[[Lenovo S5]]|seoul|✓|A|arm64|
|[[Lenovo Tab V7]]|PB-6505M|✓|A/B|arm64|
|[[Lenovo Vibe A Plus]]|a1010a20||A|arm|
|[[Lenovo Z5]]|jd2018|✓|A/B|arm64|
|[[Lenovo Z5 Pro GT]]|heart|✓|A/B|arm64|
|[[Lenovo Z5s]]|jd2019|✓|A/B|arm64|
|[[Lenovo Z6 Pro]]|zippo|✓|A/B|arm64|
|[[Lenovo Z6 Youth Edition]]|kunlun2|✓|A/B|arm64|
|[[LG G7 ThinQ]]|judyln|✓|A/B|arm64|
|[[LG G8 ThinQ]]|alphalm|✓|A/B|arm64|
|[[LG K7]]|m13g||A|arm|
|[[LG V30 / V30 Plus]]|joan|✓|A|arm64|
|[[LG V40 ThinQ]]|judypn|✓|A/B|arm64|
|[[LG G8s ThinQ]]|g810|✓|A/B|arm64|
|[[LG V50 ThinQ]]|v500|✓|A/B|arm64|
|[[LG V50s ThinQ]]|g850|✓|A/B|arm64|
|[[LG V60 ThinQ]]|v600|✓|A/B|arm64|
|[[Meizu 16s]]|16s||A/B|arm64|
|[[Meizu 16T]]|16T||A/B|arm64|
|[[Meizu 16th]]|16th||A|arm64|
|[[Meizu 16x]]|16x||A|arm64|
|[[Meizu M2 Mini]]|n/a||A|arm64|
|[[Meizu Note 9]]|n/a||A|arm64|
|[[Microsoft Surface Duo]]|duo|✓|A/B|arm64|
|[[Moto E5]]|nora|✓|A|arm|
|[[Moto E5 Plus]]|hannah|✓|A|arm|
|[[Moto G5]]|cedric||A|arm64|
|[[Moto G5 Plus]]|potter||A|arm64|
|[[Moto G5S]]|montana||A/B|arm64|
|[[Moto G5S Plus]]|sanders||A|arm64|
|[[Moto G6]]|ali|✓|A|arm|
|[[Moto G6 Play]]|aljeter|✓|A|arm|
|[[Moto G6 Plus]]|evert|✓|A/B|arm64|
|[[Moto G7 Play]]|channel|✓|A/B|arm (arm_binder64)|
|[[Moto G7 Plus]]|lake|✓|A/B|arm64|
|[[Moto G7 Power]]|ocean|✓|A/B|arm64|
|[[Moto G8]]|rav|✓|A/B|arm64|
|[[Moto G8 Plus]]|doha|✓|A/B|arm64|
|[[Moto X4]]|payton||A/B|arm64|
|[[Moto Z]]|griffin||A|arm64|
|[[Moto Z Play]]|addison||A|arm64|
|[[Moto Z2 Force]]|nash|✓|A/B|arm64|
|[[Moto Z2 Play]]|albus||A|arm64|
|[[Moto Z3 Play]]|beckham|✓|A/B|arm64|
|[[Moto Z3]]|messi|✓|A/B|arm64|
|[[Motorola One]]|deen|✓|A/B|arm64|
|[[Motorola One Power]]|chef|✓|A/B|arm64|
|[[Motorola One Vision]]|kane|✓|A/B|arm64|
|[[Motorola One Zoom]]|parker|✓|A/B|arm64|
|[[Motorola RAZR (2020)]]|voyager|✓|A/B|arm64|
|[[Motorola Edge and Edge+]]|racer and burton|✓|A/B|arm64|
|[[MyPhone myA11]]|myA11|✓ (Go)|A|arm|
|[[MyPhone myA12]]|myA12|✓ (Go)|A|arm|
|[[Nintendo Switch]]|icosa||A/B (when using Android 9 build)|arm64|
|[[Nokia 1]]|frt|✓ (Go)|A|arm|
|[[Nokia 1 Plus]]|ant|✓ (Go)|A|arm|
|[[Nokia 2.1 and 2 V]]|e2m and evw|✓ (Go)|A|arm|
|[[Nokia 3.1 and 5.1]]|es2 and co2|✓|A/B|arm64|
|[[Nokia 3.1 A and C]]|eag|✓|A/B|arm64|
|[[Nokia 3.1 Plus]]|roo|✓|A/B|arm64|
|[[Nokia 3.1 Plus C]]|rhd|✓|A/B|arm64|
|[[Nokia 3.2]]|deadpool / dpl|✓|A/B|arm64|
|[[Nokia 4.2]]|panther / pan|✓|A/B|arm64|
|[[Nokia 5.1 Plus (X5)]]|pda|✓|A/B|arm64|
|[[Nokia 6.1 / 6 (2018)]]|PL2|✓|A/B|arm64|
|[[Nokia 6.1 Plus (X6)]]|drg|✓|A/B|arm64|
|[[Nokia 6.2]]|starlord / sld|✓|A/B|arm64|
|[[Nokia 7]]|c1n|✓|A/B|arm64|
|[[Nokia 7 Plus]]|b2n|✓|A/B|arm64|
|[[Nokia 7.1]]|ctl|✓|A/B|arm64|
|[[Nokia 7.2]]|daredevil / ddv|✓|A/B|arm64|
|[[Nokia 8]]|nb1||A/B|arm64|
|[[Nokia 8 Sirocco]]|a1n|✓|A/B|arm64|
|[[Nokia 8.1 (X7)]]|pnx|✓|A/B|arm64|
|[[Nokia 9 PureView]]|aop|✓|A/B|arm64|
|[[Nokia C3]]|GamoraPlus / gmr|✓|A/B|arm64|
|[[Nokia X71]]|tas|✓|A/B|arm64|
|[[Nubia mini 5G]]|TP1803|✓|A/B|arm64|
|[[Nubia Red Magic]]|nx609j|✓|A|arm64|
|[[Nubia Red Magic 3]]|nx629j|✓|A/B|arm64|
|[[Nubia Z9 Max]]|nx512j||A|arm64|
|[[Nubia Z9 Mini]]|nx511j||A|arm64|
|[[Nubia Z17 and Z17s]]|nx563j and nx595j||A|arm64|
|[[Nubia Z18]]|nx606j||A|arm64|
|[[Nubia Z18 Mini]]|nx611j||A|arm64|
|[[OnePlus 3 and 3T]]|oneplus3||A (Support for A/B added since 26.08.2019)|arm64|
|[[OnePlus 5 and 5T]]|cheeseburger and dumpling|✓|A|arm64|
|[[OnePlus 6]]|enchilada|✓|A/B|arm64|
|[[OnePlus 6T]]|fajita|✓|A/B|arm64|
|[[OnePlus 7]]|guacamoleb|✓|A/B|arm64|
|[[OnePlus 7 Pro]]|guacamole|✓|A/B|arm64|
|[[OnePlus 7T]]|hotdogb|✓|A/B|arm64|
|[[OnePlus 7T Pro]]|hotdog|✓|A/B|arm64|
|[[OnePlus 8]]|instantnoodle|✓|A/B|arm64|
|[[OnePlus 8 Pro]]|instantnoodlep|✓|A/B|arm64|
|[[OnePlus Nord N10 5G]]|billie|✓|A/B|arm64|
|[[OnePlus Nord N100]]|clover|✓||arm64|
|[[Oppo R11 / R11s]]|r11|✓|A|arm64|
|[[Oukitel C10]]|C10|✓|A|arm|
|[[Oukitel C11 Pro]]|C11_pro|✓|A|arm64|
|[[Oukitel K7 Power]]|K7_power|✓|A|arm64|
|[[Oukitel K8]]|K8|✓|A|arm64|
|[[Oukitel K9]]|K9|✓|A/B|arm64|
|[[Ovvi SK3]]|V4701_I01||A|arm64|
|[[Prestigio Muze G5 LTE]]|n/a||A|arm|
|[[Razer Phone]]|cheryl|✓|A/B|arm64|
|[[Razer Phone 2]]|cheryl2|✓|A/B|arm64|
|[[Realme 1]]|cph1861|✓|A|arm64|
|[[Realme 2 Pro]]|rmx1801|✓|A|arm64|
|[[Realme 3 Pro]]|rmx1851|✓|A/B|arm64|
|[[Realme X]]|rmx1901|✓|A/B|arm64|
|[[Realme XT]]|rmx1921|✓|A/B|arm64|
|[[Realme 6]]|rmx2001|✓|A/B(Dynamic Partitions)|arm64|
|[[RED Hydrogen One]]|HydrogenONE|✓|A/B|arm64|
|[[Samsung Galaxy A6 Plus (2018)]]|a6plte|✓|A (A/B after updated to One UI 2.0)|arm_binder64|
|[[Samsung Galaxy A7 (2018)]]|a7y18lte||A|arm64|
|[[Samsung Galaxy A8 (Exynos)]]|jackpotlte||A + A/B|arm64|
|[[Samsung Galaxy A8 Plus (Exynos)]]|jackpot2lte||A + A/B|arm64|
|[[Samsung Galaxy A10]]|a10dd|✓|A/B|arm_binder64|
|[[Samsung Galaxy A20]]|a20dd|✓|A/B|arm64|
|[[Samsung Galaxy A30]]|a30dd|✓|A/B|arm64|
|[[Samsung Galaxy A40]]|a40|✓|A/B|arm64|
|[[Samsung Galaxy A50]]|a50dd|✓|A/B|arm64|
|[[Samsung Galaxy A51 5G]]|a51x|✓|A/B|arm64|
|[[Samsung Galaxy A60]]|a60q|✓|A/B|arm64|
|[[Samsung Galaxy A70]]|a70dd|✓|A/B|arm64|
|[[Samsung Galaxy Z Fold]]|winner|✓|A/B|arm64|
|[[Samsung Galaxy Z Fold 2]]|winner2|✓|A/B|arm64|
|[[Samsung Galaxy Z Flip]]|bloom|✓|A/B|arm64|
|[[Samsung Galaxy J2 Core]]|j2corelte|✓|A|arm_binder64|
|[[Samsung Galaxy J4]]|j4ltejx|✓|A|arm_binder64|
|[[Samsung Galaxy J4 Plus]]|j4primelte|✓|A|arm|
|[[Samsung Galaxy J5 (2017)]]|j5y17lte||A/b|arm64|
|[[Samsung Galaxy J6]]|j6ltexx|✓|A/b|arm64|
|[[Samsung Galaxy J7 (2016)]]|j7xelte||A|arm64|
|[[Samsung Galaxy J7 (2017)]]|j7y17lte||A/b|arm64|
|[[Samsung Galaxy J7 Neo]]|j7velte||A|arm64|
|[[Samsung Galaxy J7 Prime]]|on7xelte||A|arm64|
|[[Samsung Galaxy J8 (2018)]]|j8y18lte||A(Once You update to One ui 2.0 it becomes A/B)|arm_binder64|
|[[Samsung Galaxy M20]]|m20lte|✓|A|arm64|
|[[Samsung Galaxy M30s]]|m30slte|✓|A/B|arm64|
|[[Samsung Galaxy Note 8 (Exynos)]]|greatlte||A|arm64|
|[[Samsung Galaxy Note 8 (Snapdragon)]]|greatqlte|✓|A|arm64|
|[[Samsung Galaxy Note 9 (Exynos)]]|crownlte|✓|A (A/B after updated to One UI 2.0)|arm64|
|[[Samsung Galaxy Note 9 (Snapdragon)]]|crownqlte|✓|A (A/B after updated to One UI 2.0)|arm64|
|[[Samsung Galaxy Note 10 and 10 Plus (Exynos)]]|d1 and d2|✓|A/B|arm64|
|[[Samsung Galaxy Note 10 and 10 Plus (Snapdragon)]]|d1q and d2q|✓|A/B|arm64|
|[[Samsung Galaxy Note 20 and 20 Ultra (Exynos)]]|c1 and c2|✓|A/B|arm64|
|[[Samsung Galaxy Note 20 and 20 Ultra (Snapdragon)]]|c1q and c2q|✓|A/B|arm64|
|[[Samsung Galaxy S3 Neo]]|s3ve3g||A|arm|
|[[Samsung Galaxy S6 and S6 Edge]]|zeroflte and zerolte||A|arm64|
|[[Samsung Galaxy S7 and S7 Edge]]|herolte and hero2lte||A|arm64|
|[[Samsung Galaxy S8 and S8 Plus (Exynos)]]|dreamlte and dream2lte||A|arm64|
|[[Samsung Galaxy S9 and S9 Plus (Exynos)]]|starlte and star2lte|✓|A (A/B after updated to One UI 2.0)|arm64|
|[[Samsung Galaxy S9 and S9 Plus (Snapdragon)]]|starqlte/chn and star2qlte/chn|✓|A|arm64|
|[[Samsung Galaxy S10 and S10 Plus (Exynos)]]|beyond1lte and beyond2lte|✓|A/B|arm64|
|[[Samsung Galaxy S10 and S10 Plus (Snapdragon)]]|beyond1qlte and beyond2qlte|✓|A/B|arm64|
|[[Samsung Galaxy S10e (Exynos)]]|beyond0lte|✓|A/B|arm64|
|[[Samsung Galaxy S10e (Snapdragon)]]|beyond0qlte|✓|A/B|arm64|
|[[Samsung Galaxy S20 (Snapdragon)]]|hubblex1q|✓|A/B|arm64|
|[[Samsung Galaxy S20 Plus (Snapdragon)]]|hubbley2q|✓|A/B|arm64|
|[[Samsung Galaxy S20 Ultra (Snapdragon)]]|hubblez3q|✓|A/B|arm64|
|[[Samsung Galaxy S20 (Exynos)]]|hubblex1|✓|A/B|arm64|
|[[Samsung Galaxy S20 Plus (Exynos)]]|hubbley2|✓|A/B|arm64|
|[[Samsung Galaxy S20 Ultra (Exynos)]]|hubblez3|✓|A/B|arm64|
|[[Samsung Galaxy Tab A 10.1]]|gtaxlwifi and gtaxllte||A|arm64|
|[[Samsung Galaxy Tab A 8.0 (2019)]]|gtowifi|✓|A (A/B after updated to One UI 2.1)|arm64|
|[[Samsung Galaxy Tab A 10.1 (2019)]]|gta3xlwifi and gta3xl|✓|A/B|arm_binder64|
|[[Samsung Galaxy Tab S3 9.3]]|gts3lwifi and gts3llte||A|arm64|
|[[Samsung Galaxy Tab S4 10.5]]|gts4lwifi and gts4llte|✓|A|arm64|
|[[Samsung Galaxy Tab S5e]]|gts4lvwifi and gts4lvlte|✓|A/B|arm64|
|[[Samsung Galaxy Tab S6]]|gts6l and gts6lwifi|✓|A/B|arm64|
|[[Samsung Galaxy Tab S6 lite]]|gta4xl and gta4xlwifi|✓|A/B|arm64|
|[[Samsung Galaxy Tab S7]]|gts7l and gts7lwifi|✓|A/B|arm64|
|[[Samsung Galaxy Tab S7+]]|gts7xl and gts7xlwifi|✓|A/B|arm64|
|[[Sharp Aquos P6 / V1]]|hd1|✓|A/B|arm64|
|[[Sharp Aquos S2 / C10]]|ss2 / sat|✓|A/B|arm64|
|[[Sharp Aquos S3 / D10]]|hh1 / hh6 and sd1|✓|A/B|arm64|
|[[Sharp Aquos S3 Mini]]|sg1||A/B|arm64|
|[[Sony Xperia 1]]|kumano|✓|A/B|arm64|
|[[Sony Xperia 10 and 10 Plus]]|kirin and mermaid|✓|A/B|arm64|
|[[Sony Xperia 1 mk2]]|pdx-203|✓|A/B|arm64|
|[[Sony Xperia 10 mk2]]|seine|✓|A/B|arm64|
|[[Sony Xperia X]]|suzu||A|arm64|
|[[Sony Xperia X Performance]]|dora||A (A/B when updated to Android 10)|arm64|
|[[Sony Xperia XA1, XA1 Plus and XA1 Ultra]]|n/a|✓|A|arm64|
|[[Sony Xperia XA2, XA2 Plus and XA2 Ultra]]|pioneer, voyager and discovery|✓|A/B|arm64|
|[[Sony Xperia XZ]]|kagura||A|arm64|
|[[Sony Xperia XZ Premium]]|maple||A|arm64|
|[[Sony Xperia XZ1 and XZ1 Compact]]|poplar and lilac|✓|A|arm64|
|[[Sony Xperia XZ2 and XZ2 Compact]]|akari and apollo|✓|A/B|arm64|
|[[Sony Xperia XZ3]]|akatsuki|✓|A/B|arm64|
|[[Teclast M20 4G]]|M20_4G||A|arm64|
|[[Teclast M30]]|M30||A|arm64|
|[[Teclast P10HD]]|P10_HD||A/B|arm64|
|[[Tecno Camon X]]|tecno_ca7|✓|A|arm64|
|[[Tecno POP 1s Pro (F4 Pro)]]|tecno_f4pro||A|arm|
|[[Tecno Spark 4 Lite (Tecno BB4K)]]|tecno_BB4K||A/B|arm32_binder64|
|[[TINNO Rakuten Mini]]|C330|✓|A/B|arm64|
|[[TP-LINK Neffos C9A]]|n/a||A|arm64|
|[[Ulefone Armor 6 / 6E]]|armor_6 and armor_6e||A/B|arm64|
|[[Ulefone Armor 6S]]|armor_6S||A/B|arm64|
|[[Ulefone Armor X]]|armor_x||A|arm64|
|[[Umidigi A3]]|a3||A|arm64|
|[[Umidigi A3 Pro]]|a3_pro||A|arm64|
|[[Umidigi A5 Pro]]|a5_pro||A/B|arm64|
|[[Umidigi F1 / F1 Play]]|f1 and f1_play|✓|A/B|arm64|
|[[Umidigi One Max]]|one_max||A|arm64|
|[[Umidigi One Pro]]|one_pro||A|arm64|
|[[Umidigi Z2]]|z2||A|arm64|
|[[Vertex Impress Luck]]|impress_luck||A|arm|
|[[Wiko Lenny5]]|w_k400|✓ (Go)|A|arm|
|[[Wiko View Max]]|p200|✓|A|arm|
|[[Wileyfox Swift]]|crackling||A|arm64|
|[[Wileyfox Swift 2 / 2 Plus / 2 X]]|marmite||A|arm64|
|[[Xiaomi Black Shark]]|n/a|✓|A/B|arm64|
|[[Xiaomi Black Shark Helo]]|n/a|✓|A/B|arm64|
|[[Xiaomi Black Shark 2]]|n/a|✓|A/B|arm64|
|[[Xiaomi Mi 3 / Mi 4]]|cancro||A|arm|
|[[Xiaomi Mi 5]]|gemini||A|arm64|
|[[Xiaomi Mi 5s]]|capricorn||A|arm64|
|[[Xiaomi Mi 5s Plus]]|natrium||A|arm64|
|[[Xiaomi Mi 5X]]|tiffany||A|arm64|
|[[Xiaomi Mi 6]]|sagit||A|arm64|
|[[Xiaomi Mi 6X]]|wayne|✓|A（A/B when using MoKee)|arm64|
|[[Xiaomi Mi 8]]|dipper|✓|A|arm64|
|[[Xiaomi Mi 8 EE]]|ursa|✓|A|arm64|
|[[Xiaomi Mi 8 Lite]]|platina|✓|A|arm64|
|[[Xiaomi Mi 8 Pro (UD)]]|equuleus|✓|A|arm64|
|[[Xiaomi Mi 8 SE]]|sirius|✓|A|arm64|
|[[Xiaomi Mi 9]]|cepheus|✓|A/B|arm64|
|[[Xiaomi Mi 9 Lite / CC9]]|pyxis|✓|A/B|arm64|
|[[Xiaomi Mi 9 Pro 5G]]|сrux|✓|A/B|arm64|
|[[Xiaomi Mi 9 SE]]|grus|✓|A/B|arm64|
|[[Xiaomi Mi 10]]|umi|✓|A/B|arm64|
|[[Xiaomi Mi 10 Pro]]|cmi|✓|A/B|arm64|
|[[Xiaomi Mi 10 Ultra]]|cas|✓|A/B|arm64|
|[[Xiaomi Mi A1]]|tissot||A/B|arm64|
|[[Xiaomi Mi A2]]|jasmine|✓|A/B|arm64|
|[[Xiaomi Mi A2 Lite]]|daisy|✓|A/B|arm64|
|[[Xiaomi Mi A3]]|laurel|✓ (One)|A/B|arm64|
|[[Xiaomi Mi Max 2]]|oxygen||A|arm64|
|[[Xiaomi Mi Max 3]]|nitrogen|✓|A|arm64|
|[[Xiaomi Mi MIX]]|lithium||A|arm64|
|[[Xiaomi Mi MIX 2]]|chiron||A|arm64|
|[[Xiaomi Mi MIX 2s]]|polaris|✓|A|arm64|
|[[Xiaomi Mi MIX 3]]|perseus|✓|A/B|arm64|
|[[Xiaomi Mi MIX 3 5G]]|andromeda|✓|A/B|arm64|
|[[Xiaomi Mi Note 2]]|scorpio||A|arm64|
|[[Xiaomi Mi Note 3]]|jason||A|arm64|
|[[Xiaomi Mi Note 10 / CC9 Pro]]|tucana|✓|A/B|arm64|
|[[Xiaomi Mi Pad 4]]|clover|✓|A|arm64|
|[[Xiaomi Mi Play]]|lotus||A|arm64|
|[[Xiaomi Pocophone F1 (Poco F1)]]|beryllium|✓|A|arm64|
|[[Xiaomi Redmi 3 / 3 Pro]]|ido||A|arm64|
|[[Xiaomi Redmi 3S / Prime / 3X]]|land||A|arm64|
|[[Xiaomi Redmi 4 Pro / Prime]]|markw||A|arm64|
|[[Xiaomi Redmi 4A]]|rolex||A|arm64|
|[[Xiaomi Redmi 4X]]|santoni||A|arm64|
|[[Xiaomi Redmi 5]]|rosy||A|arm64|
|[[Xiaomi Redmi 5 Plus / Note 5 (India)]]|vince||A|arm64|
|[[Xiaomi Redmi 5A]]|riva||A|arm64|
|[[Xiaomi Redmi 6]]|cereus|✓|A (A/B when updated to Android 9)|arm (arm_binder64)|
|[[Xiaomi Redmi 6 Pro]]|sakura|✓|A|arm64|
|[[Xiaomi Redmi 7]]|onc|✓|A/B|arm64|
|[[Xiaomi Redmi 7A]]|pine|✓|A/B|arm_binder64 arm64|
|[[Xiaomi Redmi 8]]|olive|✓|A/B|arm64|
|[[Xiaomi Redmi 8A]]|olivelite|✓|A/B|arm_binder64|
|[[Xiaomi Redmi Go]]|tiare|✓ (Go)|A|arm|
|[[Xiaomi Redmi K20 / Mi 9T]]|davinci|✓|A/B|arm64|
|[[Xiaomi Redmi K20 Pro / Mi 9T Pro]]|raphael|✓|A/B|arm64|
|[[Xiaomi Redmi K20 Pro Premium]]|raphael|✓|A/B|arm64|
|[[Xiaomi Redmi K30 / Poco X2]]|phoenix|✓|A/B|arm64|
|[[Xiaomi Redmi K30 5G]]|picasso|✓|A/B|arm64|
|[[Xiaomi Redmi K30 Pro / Zoom Edition / Poco F2 Pro]]|lmi|✓|A/B|arm64|
|[[Xiaomi Redmi K30 Ultra]]|cezanne|✓|A/B|arm64|
|[[Xiaomi Redmi Note 3 (Snapdragon)]]|kenzo||A|arm64|
|[[Xiaomi Redmi Note 4 (Snapdragon)]]|mido||A|arm64|
|[[Xiaomi Redmi Note 5 / Note 5 Pro (India)]]|whyred|✓|A|arm64|
|[[Xiaomi Redmi Note 5A]]|ugg and ugglite| |A/B|arm64|
|[[Xiaomi Redmi Note 6 Pro]]|tulip|✓|A|arm64|
|[[Xiaomi Redmi Note 7]]|lavender|✓|A/B|arm64|
|[[Xiaomi Redmi Note 7 Pro]]|violet|✓|A/B|arm64|
|[[Xiaomi Redmi Note 8]]|ginkgo|✓|A/B|arm64|
|[[Xiaomi Redmi Note 8 Pro]]|begonia|✓|A/B|arm64|
|[[Xiaomi Redmi Note 8T]]|willow|✓|A/B|arm64|
|[[Xiaomi Redmi Note 9S]]|curtana|✓|A/B|arm64|
|[[Xiaomi Redmi S2 / Y2 (India)]]|ysl|✓|A|arm|
|[[Yandex Phone]]|amber|✓|A/B|arm64|
|[[ZTE A530]]|p639t10||A|arm64|
|[[ZTE Axon 7]]|axon7 / ailsa_ii||A|arm64|
|[[ZTE Axon 10 Pro]]|n/a|✓|A/B|arm64|
|[[ZTE Blade A3 (2019)]]|z3051t|✓|A/B|arm_binder64|
|[[ZTE Blade V9]]|p450f10||A|arm64|
|[[ZTE Blade V9 Vita]]|p840f03||A|arm64|
|[[ZTE Blade V10]]|n/a|✓|A/B|arm64|
|[[ZUK Z2 Plus and Z2 Pro]]|z2_plus and z2_row||A|arm64|