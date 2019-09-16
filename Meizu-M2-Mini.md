# Meizu M2 Mini

### Incoming calls and USSD
It's broken by default on our device, but can be fixed by editing `/system/bin/rw-system.sh` script.  
Find this code:
```sh
for f in /vendor/lib/mtk-ril.so /vendor/lib64/mtk-ril.so /vendor/lib/libmtk-ril.so /vendor/lib64/libmtk-ril.so; do
    [ ! -f $f ] && continue
    # shellcheck disable=SC2010
    ctxt="$(ls -lZ "$f" | grep -oE 'u:object_r:[^:]*:s0')"
    b="$(echo "$f" | tr / _)"

    cp -a "$f" "/mnt/phh/$b"
    sed -i \
        -e 's/AT+EAIC=2/AT+EAIC=3/g' \
        "/mnt/phh/$b"
    chcon "$ctxt" "/mnt/phh/$b"
    mount -o bind "/mnt/phh/$b" "$f"

    setprop persist.sys.phh.radio.force_cognitive true
    setprop persist.sys.radio.ussd.fix true
done
```
and replace it to:
```sh
setprop persist.sys.phh.radio.force_cognitive true
setprop persist.sys.radio.ussd.fix true
```

### Camera
Stock camera app can't take photos, but can record videos.  
Then I tested with third-party camera app `Footej Camera`. It can take photos but can't record videos.

### Magisk issue
If you're flashed latest Magisk and don't getting prompt to root access, try to [do this](https://github.com/topjohnwu/Magisk/issues/844#issuecomment-503339709):
> As it turns out, it wasn't Magisk's fault. The shared library `libdirect-coredump.so` was missing from `/system/lib` / `/system/lib64`, so I copied it from `/vendor` and Magisk started working perfectly.

## Hardware support

| Component                 |      Comment                                                                                                                   |
|---------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| Camera                    | [Semi broken](#camera)                                                                                                         |
| Speaker / Mic             | Working                                                                                                                        |
| Bluetooth                 | Working                                                                                                                        |
| WiFi                      | Working with 2G and 5G networks. [Tethering broken](https://forum.xda-developers.com/showpost.php?p=80249301&postcount=1684)   |
| SIM / Mobile Data / Voice | [Semi broken](#incoming-calls-and-ussd). Mobile data and outgoing calls working. Second SIM-card slot not tested (should work) |
| VoLTE                     | Unknown                                                                                                                        |
| Offline Charging          | Working                                                                                                                        |
| 3.5mm audio jack          | Working                                                                                                                        |
---

Tested By: [EarsKilla](https://github.com/EarsKilla) - M2 mini (global), HavocOS 2.9 - 17.09.2019  
Template created by @zguithues and @hackintosh5