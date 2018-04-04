2018-04-04

on the Pixel 2 (walleye), the v15 system image (8.1) successfully boots over top of the OPM2.171019.029 factory image (8.1) after reflashing the vbmeta partition as follows:

```bash
$ fastboot --version
fastboot version 0.0.1-4500957
Installed as XXX
# extract vbmeta from the factory image zip and reflash:
$ fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
```

```bash
$ md5sum system-arm64-ab-vanilla-nosu.img
9aeacaa52a12feca8cb737b3fd083714  system-arm64-ab-vanilla-nosu.img
$ sha256sum system-arm64-ab-vanilla-nosu.img 
ec0e6299491dd8c6c9976e19fdfa887b470e9aaf4802632dd6295e7fb9cee38b  system-arm64-ab-vanilla-nosu.img
$ sha256sum walleye-opm2.171019.029-factory-41296266.zip 
4129626633cbab200c6c18fc52b2dd832714ef96761e1866b60d462e4dd39cac  walleye-opm2.171019.029-factory-41296266.zip
```

