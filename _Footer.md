--------- beginning of main
05-16 08:26:45.359   345   345 W auditd  : type=2000 audit(0.0:1): initialized
05-16 08:26:47.619   345   345 I auditd  : type=1403 audit(0.0:2): policy loaded auid=4294967295 ses=4294967295
05-16 08:26:47.639   335   335 W fsck.f2fs: type=1400 audit(0.0:3): avc: denied { open } for path="/dev/urandom" dev="tmpfs" ino=2184 scontext=u:r:fsck:s0 tcontext=u:object_r:tmpfs:s0 tclass=chr_file permissive=0
05-16 08:26:47.659     1     1 W init    : type=1400 audit(0.0:4): avc: denied { relabelfrom } for name="uevent" dev="sysfs" ino=33163 scontext=u:r:init:s0 tcontext=u:object_r:sysfs_zram_uevent:s0 tclass=file permissive=0
05-16 08:26:47.859     1     1 W init    : type=1400 audit(0.0:5): avc: denied { relabelto } for name="cust" dev="tmpfs" ino=12800 scontext=u:r:init:s0 tcontext=u:object_r:cust_block_device:s0 tclass=lnk_file permissive=0
05-16 08:26:48.319   342   342 W charger : type=1400 audit(0.0:6): avc: denied { read } for name="/" dev="tmpfs" ino=2179 scontext=u:r:charger:s0 tcontext=u:object_r:device:s0 tclass=dir permissive=0
05-16 08:26:48.319   209   209 W kworker/u16:2: type=1400 audit(0.0:7): avc: denied { write } for name="hwlog_dubai" dev="tmpfs" ino=2304 scontext=u:r:kernel:s0 tcontext=u:object_r:device:s0 tclass=chr_file permissive=0
05-16 08:26:48.399   348   348 W init    : type=1400 audit(0.0:8): avc: granted { open } for path="/dev/pmsg0" dev="tmpfs" ino=2340 scontext=u:r:init:s0 tcontext=u:object_r:pmsg_device:s0 tclass=chr_file
05-16 08:26:48.404   348   348 E logwrapper: Cannot log to file /dev/fscklogs/log
05-16 08:26:48.443   347   347 E hwservicemanager: BINDER_SET_INHERIT_FIFO_PRIO failed with error -1
05-16 08:26:48.804   348   348 E logwrapper: Cannot log to file /dev/fscklogs/log
05-16 08:26:49.272   348   348 I chatty  : uid=0(root) /init identical 4 lines
05-16 08:26:49.357   348   348 E logwrapper: Cannot log to file /dev/fscklogs/log
05-16 08:26:49.449   387   387 W e2fsck  : type=1400 audit(0.0:9): avc: denied { read } for name="mmcblk0p11" dev="tmpfs" ino=2452 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-16 08:26:49.449   387   387 W e2fsck  : type=1400 audit(0.0:10): avc: denied { read write } for name="mmcblk0p11" dev="tmpfs" ino=2452 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-16 08:26:49.499   390   390 W e2fsck  : type=1400 audit(0.0:11): avc: denied { read } for name="mmcblk0p18" dev="tmpfs" ino=2487 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-16 08:26:49.499   390   390 W e2fsck  : type=1400 audit(0.0:12): avc: denied { read write } for name="mmcblk0p18" dev="tmpfs" ino=2487 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
--------- beginning of crash
05-16 08:26:49.502   386   386 F libc    : CANNOT LINK EXECUTABLE "/vendor/bin/atcmdserver": library "android.hidl.base@1.0.so" not found
05-16 08:26:49.502   386   386 F libc    : Fatal signal 6 (SIGABRT), code -6 in tid 386 (atcmdserver), pid 386 (atcmdserver)
05-16 08:26:49.509   241   241 W modem_sysboot_s: type=1400 audit(0.0:13): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.512   385   385 I aptouch_daemon: log_init_is_factory, 0
05-16 08:26:49.512   385   385 I aptouch_daemon: log_init_is_enabled, 0
05-16 08:26:49.512   385   385 I aptouch_daemon: main, first_log_in_aptouch_daemon_main
05-16 08:26:49.517   385   385 I aptouch_daemon: set thp.dae_alive as: false
05-16 08:26:49.523   343   343 E         : pid 1, opration oeminfo_read OK
05-16 08:26:49.523   343   343 E         : 
--------- beginning of system
05-16 08:26:49.526   379   379 I vold    : Vold 3.0 (the awakening) firing up
05-16 08:26:49.526   379   379 V vold    : Detected support for: ext4 f2fs vfat
05-16 08:26:49.529   241   241 W modem_sysboot_s: type=1400 audit(0.0:14): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.529   241   241 W modem_sysboot_s: type=1400 audit(0.0:15): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.529     1     1 W init    : type=1400 audit(0.0:16): avc: granted { open } for path="/dev/pmsg0" dev="tmpfs" ino=2340 scontext=u:r:init:s0 tcontext=u:object_r:pmsg_device:s0 tclass=chr_file
05-16 08:26:49.529   343   343 E         : pid 1, opration oeminfo_read OK
05-16 08:26:49.529   343   343 E         : 
05-16 08:26:49.537   343   343 E         : oeminfo_read:oeminfo data not find !!!!
05-16 08:26:49.537   343   343 E         : 
05-16 08:26:49.537   343   343 E         : oeminfo_read_data, fail to read oeminfo
05-16 08:26:49.537   343   343 E         : 
05-16 08:26:49.537   343   343 E         : pid 1, opration oeminfo_read FAIL
05-16 08:26:49.537   343   343 E         : 
05-16 08:26:49.538     1     1 E         : rmt_oeminfo_read, get data from server fail
05-16 08:26:49.539   392   392 E cutils-trace: Error opening trace file: No such file or directory (2)
05-16 08:26:49.542   343   343 E         : oeminfo_read:oeminfo data not find !!!!
05-16 08:26:49.542   343   343 E         : 
05-16 08:26:49.542   343   343 E         : oeminfo_read_data, fail to read oeminfo
05-16 08:26:49.542   343   343 E         : 
05-16 08:26:49.542   343   343 E         : pid 1, opration oeminfo_read FAIL
05-16 08:26:49.542   343   343 E         : 
05-16 08:26:49.542     1     1 E         : rmt_oeminfo_read, get data from server fail
05-16 08:26:49.546   396   396 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-16 08:26:49.546   396   396 E libc    : failed to connect to tombstoned: No such file or directory
05-16 08:26:49.548   343   343 E         : oeminfo_read:oeminfo data not find !!!!
05-16 08:26:49.548   343   343 E         : 
05-16 08:26:49.549   343   343 E         : oeminfo_read_data, fail to read oeminfo
05-16 08:26:49.549   343   343 E         : 
05-16 08:26:49.549   343   343 E         : pid 1, opration oeminfo_read FAIL
05-16 08:26:49.549   343   343 E         : 
05-16 08:26:49.549     1     1 E         : rmt_oeminfo_read, get data from server fail
05-16 08:26:49.550   396   396 I crash_dump64: performing dump of process 386 (target tid = 386)
05-16 08:26:49.550   396   396 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-16 08:26:49.550   396   396 F DEBUG   : Build fingerprint: 'Android/treble_arm64_agS/phhgsi_arm64_a:8.1.0/OPM4.171019.016/180514:userdebug/test-keys'
05-16 08:26:49.550   396   396 F DEBUG   : Revision: '0'
05-16 08:26:49.550   396   396 F DEBUG   : ABI: 'arm64'
05-16 08:26:49.551   396   396 F DEBUG   : pid: 386, tid: 386, name: atcmdserver  >>> /vendor/bin/atcmdserver <<<
05-16 08:26:49.551   396   396 F DEBUG   : signal 6 (SIGABRT), code -6 (SI_TKILL), fault addr --------
05-16 08:26:49.553   396   396 F DEBUG   : Abort message: 'CANNOT LINK EXECUTABLE "/vendor/bin/atcmdserver": library "android.hidl.base@1.0.so" not found'
05-16 08:26:49.553   396   396 F DEBUG   :     x0   0000000000000000  x1   0000000000000182  x2   0000000000000006  x3   0000000000000008
05-16 08:26:49.553   396   396 F DEBUG   :     x4   0000000000000000  x5   0000000000000000  x6   0000000000000000  x7   0000000000000038
05-16 08:26:49.553   396   396 F DEBUG   :     x8   0000000000000083  x9   c364a42c2478df62  x10  0000000000000000  x11  0000000000000001
05-16 08:26:49.553   396   396 F DEBUG   :     x12  ffffffffffffffff  x13  000000005afbeb49  x14  000773593fe2b400  x15  000008f153b54f79
05-16 08:26:49.553   396   396 F DEBUG   :     x16  0000000000000000  x17  04ed9fe422d08f77  x18  00000078c3e6e450  x19  0000000000000182
05-16 08:26:49.553   396   396 F DEBUG   :     x20  0000000000000182  x21  0000005d1b9cd4eb  x22  0000007fdfe30d58  x23  0000005d1ba61500
05-16 08:26:49.553   396   396 F DEBUG   :     x24  00000078c3e6d488  x25  00000078c3f773d0  x26  00000078c3f777b0  x27  00000078c3f77000
05-16 08:26:49.554   396   396 F DEBUG   :     x28  0000007fdfe30d50  x29  0000007fdfe2fa30  x30  00000078c3f1b000
05-16 08:26:49.554   396   396 F DEBUG   :     sp   0000007fdfe2f9f0  pc   00000078c3f1b01c  pstate 0000000060000000
05-16 08:26:49.562   396   396 F DEBUG   : 
05-16 08:26:49.562   396   396 F DEBUG   : backtrace:
05-16 08:26:49.562   396   396 F DEBUG   :     #00 pc 000000000009e01c  /system/bin/linker64 (__dl_abort+104)
05-16 08:26:49.562   396   396 F DEBUG   :     #01 pc 000000000001cb50  /system/bin/linker64 (__dl___linker_init+3624)
05-16 08:26:49.562   396   396 F DEBUG   :     #02 pc 0000000000023000  /system/bin/linker64 (_start+4)
05-16 08:26:49.573   343   343 E         : pid 1, opration oeminfo_read OK
05-16 08:26:49.573   343   343 E         : 
05-16 08:26:49.576   343   343 E         : oeminfo_read:oeminfo data not find !!!!
05-16 08:26:49.576   343   343 E         : 
05-16 08:26:49.576   343   343 E         : oeminfo_read_data, fail to read oeminfo
05-16 08:26:49.576   343   343 E         : 
05-16 08:26:49.576   343   343 E         : pid 1, opration oeminfo_read FAIL
05-16 08:26:49.576   343   343 E         : 
05-16 08:26:49.576     1     1 E         : rmt_oeminfo_read, get data from server fail
05-16 08:26:49.576     1     1 E factory_interface: get_preload_app_batch: Read preload app batch error! 
05-16 08:26:49.581   343   343 E         : pid 1, opration oeminfo_read OK
05-16 08:26:49.581   343   343 E         : 
05-16 08:26:49.589   396   396 W crash_dump64: type=1400 audit(0.0:17): avc: denied { search } for name="/" dev="tmpfs" ino=2733 scontext=u:r:crash_dump:s0 tcontext=u:object_r:tmpfs:s0 tclass=dir permissive=0
05-16 08:26:49.594   396   396 E crash_dump64: unable to connect to activity manager: Permission denied
05-16 08:26:49.644   343   343 E         : pid 1, opration nvm_read OK
05-16 08:26:49.644   343   343 E         : 
05-16 08:26:49.662   385   385 I aptouch_daemon: daemon_prop_version, daemon current version: normal/2.5.365, old version: null.
05-16 08:26:49.666   385   385 I aptouch_daemon: open libray libaftouch.so sucessfully
05-16 08:26:49.666   385   385 I aptouch_daemon: main, this panel do not support hostprocessing and not support aft.
05-16 08:26:49.667   385   385 I aptouch_daemon: self_exit
05-16 08:26:49.707   379   399 D VoldCryptCmdListener: cryptfs mountdefaultencrypted
05-16 08:26:49.709   379   405 I Cryptfs : cryptfs_check_passwd
05-16 08:26:49.710   379   405 D Cryptfs : crypt_ftr->fs_size = 113680352
05-16 08:26:49.710   379   405 I Cryptfs : Using scrypt with keymaster for cryptfs KDF
05-16 08:26:49.730   343   343 E         : pid 1, opration nvm_read OK
05-16 08:26:49.730   343   343 E         : 
05-16 08:26:49.731   343   343 I chatty  : uid=0(root) oeminfo_nvm_ser identical 1 line
05-16 08:26:49.742   343   343 E         : pid 1, opration nvm_read OK
05-16 08:26:49.742   343   343 E         : 
05-16 08:26:49.757   408   409 W libc    : Set property "sys.usb.ffs_hdb.ready" to "1"
05-16 08:26:49.762   408   410 E cutils-trace: atrace_findTraceFiles, can't find trace_path
05-16 08:26:49.762   408   410 E cutils-trace: atrace_init_once, Error find trace file
05-16 08:26:49.780   407   412 W libc    : Set property "sys.usb.ffs.ready" to "1"
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:18): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:19): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:20): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:21): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:22): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:23): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:24): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.799   241   241 I chatty  : uid=0(root) identical 1 line
05-16 08:26:49.799   241   241 W modem_sysboot_s: type=1400 audit(0.0:26): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.807   406   406 E cutils-trace: Error opening trace file: No such file or directory (2)
05-16 08:26:49.810   347   347 E cutils-trace: Error opening trace file: No such file or directory (2)
05-16 08:26:49.819   241   241 W modem_sysboot_s: type=1400 audit(0.0:27): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.822   406   406 D vndksupport: Loading /vendor/lib64/hw/android.hardware.keymaster@3.0-impl.so from current namespace instead of sphal namespace.
05-16 08:26:49.829   241   241 I chatty  : uid=0(root) expire 14 lines
05-16 08:26:49.829   241   241 W modem_sysboot_s: type=1400 audit(0.0:42): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.839   422   422 W ACPU_NFEXT: type=1400 audit(0.0:43): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-16 08:26:49.840   414   414 F libc    : CANNOT LINK EXECUTABLE "/vendor/bin/atcmdserver": library "android.hidl.base@1.0.so" not found
05-16 08:26:49.840   414   414 F libc    : Fatal signal 6 (SIGABRT), code -6 in tid 414 (atcmdserver), pid 414 (atcmdserver)
05-16 08:26:49.842   406   406 E /vendor/bin/hw/android.hardware.keymaster@3.0-service: Failed to dlopen android.hardware.keymaster@3.0-impl.so: dlopen failed: library "libkeymaster1.so" not found
05-16 08:26:49.844   406   406 E android.hardware.keymaster@3.0-service: Could not get passthrough implementation for android.hardware.keymaster@3.0::IKeymasterDevice/default.
05-16 08:26:49.872   436   436 E cutils-trace: Error opening trace file: No such file or directory (2)
05-16 08:26:49.878   437   437 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-16 08:26:49.879   437   437 E libc    : failed to connect to tombstoned: No such file or directory
05-16 08:26:49.879   437   437 I crash_dump64: performing dump of process 414 (target tid = 414)
05-16 08:26:49.879   437   437 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-16 08:26:49.879   437   437 F DEBUG   : Build fingerprint: 'Android/treble_arm64_agS/phhgsi_arm64_a:8.1.0/OPM4.171019.016/180514:userdebug/test-keys'
05-16 08:26:49.879   437   437 F DEBUG   : Revision: '0'
05-16 08:26:49.879   437   437 F DEBUG   : ABI: 'arm64'
05-16 08:26:49.880   437   437 F DEBUG   : pid: 414, tid: 414, name: atcmdserver  >>> /vendor/bin/atcmdserver <<<
05-16 08:26:49.880   437   437 F DEBUG   : signal 6 (SIGABRT), code -6 (SI_TKILL), fault addr --------
05-16 08:26:49.882   437   437 F DEBUG   : Abort message: 'CANNOT LINK EXECUTABLE "/vendor/bin/atcmdserver": library "android.hidl.base@1.0.so" not found'
05-16 08:26:49.882   437   437 F DEBUG   :     x0   0000000000000000  x1   000000000000019e  x2   0000000000000006  x3   0000000000000008
05-16 08:26:49.883   437   437 F DEBUG   :     x4   0000000000000000  x5   0000000000000000  x6   0000000000000000  x7   0000000000000038
05-16 08:26:49.883   437   437 F DEBUG   :     x8   0000000000000083  x9   8ca59567bbe3af5b  x10  0000000000000000  x11  0000000000000001
05-16 08:26:49.883   437   437 F DEBUG   :     x12  ffffffffffffffff  x13  000000005afbeb49  x14  000c84587fdf6200  x15  0000019d012aa99c
05-16 08:26:49.883   437   437 F DEBUG   :     x16  0000000000000000  x17  0046a2f13069d7e8  x18  00000078af263230  x19  000000000000019e
05-16 08:26:49.883   437   437 F DEBUG   :     x20  000000000000019e  x21  000000583fb364eb  x22  0000007fcb514338  x23  000000583fbca500
05-16 08:26:49.883   437   437 F DEBUG   :     x24  00000078af262488  x25  00000078af36c3d0  x26  00000078af36c7b0  x27  00000078af36c000
05-16 08:26:49.883   437   437 F DEBUG   :     x28  0000007fcb514330  x29  0000007fcb513010  x30  00000078af310000
05-16 08:26:49.883   437   437 F DEBUG   :     sp   0000007fcb512fd0  pc   00000078af31001c  pstate 0000000060000000
05-16 08:26:49.887   437   437 F DEBUG   : 
05-16 08:26:49.887   437   437 F DEBUG   : backtrace:
05-16 08:26:49.887   437   437 F DEBUG   :     #00 pc 000000000009e01c  /system/bin/linker64 (__dl_abort+104)
05-16 08:26:49.887   437   437 F DEBUG   :     #01 pc 000000000001cb50  /system/bin/linker64 (__dl___linker_init+3624)
05-16 08:26:49.887   437   437 F DEBUG   :     #02 pc 0000000000023000  /system/bin/linker64 (_start+4)
05-16 08:26:49.909   437   437 W crash_dump64: type=1400 audit(0.0:44): avc: denied { search } for name="/" dev="tmpfs" ino=2733 scontext=u:r:crash_dump:s0 tcontext=u:object_r:tmpfs:s0 tclass=dir permissive=0
05-16 08:26:49.916   437   437 E crash_dump64: unable to connect to activity manager: Permission denied
05-16 08:26:49.984   407   443 E cutils-trace: atrace_findTraceFiles, can't find trace_path
05-16 08:26:49.985   407   443 E cutils-trace: atrace_init_once, Error find trace file
