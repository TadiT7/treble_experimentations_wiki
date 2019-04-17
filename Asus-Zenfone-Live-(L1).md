# Asus Zenfone Live (L1) ZA550KL
##  Hardware support
* Camera
> Front and back both working. Stock gsi ROM camera is working fine, but flash on stock camera if set to on/auto will make camera force close, other 3rd party camera apps working fine with flash on/auto. Add this line to build.prop on system folder to make the camera photo result normal and no dark anymore, thanks to Maulana Kurniawan (myself), accidentally discover this & solving the problem : 
`ro.build.user=zhuyujing ro.build.host=SOFT30-28 ro.build.tags=test-keys ro.build.flavor=A306-user ro.product.model=ASUS_X00RD ro.product.brand=Android ro.product.name=ZA550KL ro.product.device=asus`
* Speaker / Microphone
> Loud-speak (bottom) works, earpiece (top-front) works, microphone works
* Bluetooth
> Bluetooth with Mi Band 2 worked
* WiFi
> Works
* SIM / Mobile Data / Voice
> Works
## Additional Notes
This model pre-installed by Asus with Android 8.0 ZenUI and support project Treble.
## Tested By:
* AcAciA - Asus Zenfone Live (L1) ZA550KL 2GB RAM on AOSP 8.1 v23 by phhusson, and Pixel Experience 2018-09-11 by jhenrique09. On 2018-9-13.
* AOSP 9.0 v111 by bramaudi 2019-03-21
* Maulana Kurniawan & Tyo Mahameru - Asus Zenfone Live L1 ZA550KL 2GB RAM on AOSP 8.1 v30 & AOSP 9.1 v112 by phhusson, AOSP Extended v6.0 & v6.1 by EnesSastim, AICP-mordiford v13.1 by AndroPlus, LineageOS v15.1 gsi by phhusson, dotOS v2.3.1 by dotOS Team, POSP by NFound etc. On 2019-04-15