# Xiaomi Redmi 7 (Codename "onc")

Works with selinux=permissive, VoLTE untested, all other hardware works.

## Steps to install

#### 1. Unlock bootloader
Using the Xiami tool or [Penn5's tool](https://github.com/penn5/miunlock)

#### 2. Flash stock rom [V11.0.2.0.PFLMIXM_20191022](https://bigota.d.miui.com/V11.0.2.0.PFLMIXM/onclite_global_images_V11.0.2.0.PFLMIXM_20191022.0000.00_9.0_global_b0cd3cab92.tgz)
([_index of ROMs_](https://mirom.ezbox.idv.tw/en/phone/onclite/))

Not sure if you need this, but this is what worked for me.

Note: I've made sure the device is not rebooting after this step by uncommenting "fastboot reboot"
in the second last line of "flash_all.sh" below. This enables the GSI ROM to run the device encryption.

```
$ wget https://bigota.d.miui.com/V11.0.2.0.PFLMIXM/onclite_global_images_V11.0.2.0.PFLMIXM_20191022.0000.00_9.0_global_b0cd3cab92.tgz
$ tar -xzvf onclite_global_images_V11.0.2.0.PFLMIXM_20191022.0000.00_9.0_global_b0cd3cab92.tgz
$ cd onclite_global_images_V11.0.2.0.PFLMIXM_20191022.0000.00_9.0_global
$ cat ./flash_all.sh | sed "s/fastboot reboot/#fastboot reboot/g" > flash_all_no_reboot.sh
$ chmod u+x ./flash_all_no_reboot.sh
$ ./flash_all_no_reboot.sh
```

#### 3. Flash vbmeta with disable verity

This was necessary because otherwise the boot img halted with a dm-verity exception and the
device was stuck in a boot loop.

Note: Flashing with --disable-verity AND --disable-verification did NOT enable
the device to boot (stuck in bootloader). Flashing with --disable-verity ONLY worked for me.

```
$ fastboot flash --disable-verity vbmeta images/vbmeta.img
```

#### 4. Modify stock boot.img to make "androidboot.selinux=permissive"

This was necessary because the the GSI ROM I used got stuck while booting with
selinux exceptions in adb logcat.

The following commands basically add "androidboot.selinux=permissive" to the
end of the kernel cmdline in boot img.

```
$ cp images/boot.img stock-boot-with-bootarg-permissive.img
$ echo "6d6dd34f63ab42785186e01ca036a751  stock-boot-with-bootarg-permissive.img" | md5sum -c
$ if [ $? -ne 0 ] ; then echo "MD5 checksum of input boot.img not as expected"; fi
$ printf " androidboot.selinux=permissive" | dd if=/dev/stdin of=stock-boot-with-bootarg-permissive.img obs=1 seek=388 conv=notrunc
$ echo "be80a5217ebe846c1e547c14092c4efe  stock-boot-with-bootarg-permissive.img" | md5sum -c
$ if [ $? -eq 0 ] ; then echo "MD5 checksum of patched boot.img is OK - patching successful"; fi
```

If the above patching is successful (you should see the "patching successful message"), you need to flash the result:
```
$ fastboot flash boot stock-boot-with-bootarg-permissive.img
```

#### 5. Flash the GSI system image (I've used the current [Ressurection Remix GSI](https://get.resurrectionremix.com/gsi/ARM64_AB_20191205.img))
```
$ fastboot flash system ARM64_AB_20191205.img
```

#### 6. Reboot the device
```
$ fastboot reboot
```

#### 7. Resize filesystem
In Recovery, resize the Data and System filesystems.

#### GApps
Flashing OpenGApps with official TWRP [`twrp-3.3.1-1-onclite`](https://eu.dl.twrp.me/onclite/twrp-3.3.1-1-onclite.img) doesn't work, it fails with [error 64](https://github.com/TeamWin/Team-Win-Recovery-Project/issues/1070).
Unofficial version [`TWRP-Redmi7-LRTeam`](https://miui.blog/redmi-7/twrp-flasher-tool-redmi-7/) works. 

Enjoy!

## Hardware support

| Component                 |      Comment                                              |
|---------------------------|-----------------------------------------------------------|
| Camera                    | works                                                    |
| Speaker / Mic             | works                                                    |
| Bluetooth                 | works                                                    |
| WiFi                      | works                                                    |
| SIM / Mobile Data / Voice | works                                                    |
| VoLTE                     | untested                                                    |
| Fingerprint               | works                                                    |
| NFC                       | not present                                                    |
| Offline Charging          | works                                                    |
---

Tested By: @SebastianApel - xiaomi/onc_eea/onc:9/PKQ1.181021.001/V10.2.8.0.PFLEUXM - 2019-07-24

Template created by @zguithues and @hackintosh5