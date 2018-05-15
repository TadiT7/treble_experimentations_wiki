--------- beginning of main
05-15 01:33:03.431   383   383 W auditd  : type=2000 audit(0.0:1): initialized
05-15 01:33:05.639   383   383 I auditd  : type=1403 audit(0.0:2): policy loaded auid=4294967295 ses=4294967295
05-15 01:33:05.659   338   338 W fsck.f2fs: type=1400 audit(0.0:3): avc: denied { open } for path="/dev/urandom" dev="tmpfs" ino=9612 scontext=u:r:fsck:s0 tcontext=u:object_r:tmpfs:s0 tclass=chr_file permissive=0
05-15 01:33:05.679     1     1 W init    : type=1400 audit(0.0:4): avc: denied { relabelfrom } for name="uevent" dev="sysfs" ino=33163 scontext=u:r:init:s0 tcontext=u:object_r:sysfs_zram_uevent:s0 tclass=file permissive=0
05-15 01:33:05.879     1     1 W init    : type=1400 audit(0.0:5): avc: denied { relabelto } for name="cust" dev="tmpfs" ino=3437 scontext=u:r:init:s0 tcontext=u:object_r:cust_block_device:s0 tclass=lnk_file permissive=0
05-15 01:33:07.559   376   376 W e2fsck  : type=1400 audit(0.0:6): avc: denied { read } for name="mmcblk0p11" dev="tmpfs" ino=3588 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-15 01:33:07.559   376   376 W e2fsck  : type=1400 audit(0.0:7): avc: denied { read write } for name="mmcblk0p11" dev="tmpfs" ino=3588 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-15 01:33:07.579   379   379 W e2fsck  : type=1400 audit(0.0:8): avc: denied { read } for name="mmcblk0p18" dev="tmpfs" ino=9745 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-15 01:33:07.579   379   379 W e2fsck  : type=1400 audit(0.0:9): avc: denied { read write } for name="mmcblk0p18" dev="tmpfs" ino=9745 scontext=u:r:fsck:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=0
05-15 01:33:07.589   240   240 W modem_sysboot_s: type=1400 audit(0.0:10): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-15 01:33:07.693   384   384 I SELinux : SELinux: Loaded service_contexts from:
05-15 01:33:07.696   384   384 I SELinux :     /system/etc/selinux/plat_service_contexts
05-15 01:33:07.719   386   386 W vndservicemanag: type=1400 audit(0.0:14): avc: denied { write } for name="hwlog_dubai" dev="tmpfs" ino=4441 scontext=u:r:vndservicemanager:s0 tcontext=u:object_r:device:s0 tclass=chr_file permissive=0
05-15 01:33:07.724   386   386 I SELinux : SELinux: Loaded service_contexts from:
05-15 01:33:07.726   386   386 I SELinux :     /vendor/etc/selinux/vndservice_contexts
05-15 01:33:07.740   385   385 E hwservicemanager: BINDER_SET_INHERIT_FIFO_PRIO failed with error -1
05-15 01:33:07.749   411   411 I rw-system.sh: type=1400 audit(0.0:15): avc: denied { getattr } for path="/system/bin/sh" dev="mmcblk0p52" ino=1764 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:shell_exec:s0 tclass=file permissive=1
05-15 01:33:07.759   411   411 I rw-system.sh: type=1400 audit(0.0:16): avc: denied { read } for path="/system/bin/sh" dev="mmcblk0p52" ino=1764 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:shell_exec:s0 tclass=file permissive=1
05-15 01:33:07.759   411   411 I rw-system.sh: type=1400 audit(0.0:17): avc: denied { getattr } for path="/system/bin/toybox" dev="mmcblk0p52" ino=1802 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:toolbox_exec:s0 tclass=file permissive=1
05-15 01:33:07.759   411   411 I rw-system.sh: type=1400 audit(0.0:18): avc: denied { execute } for name="toybox" dev="mmcblk0p52" ino=1802 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:toolbox_exec:s0 tclass=file permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:19): avc: denied { getattr } for path="/sec_storage" dev="mmcblk0p13" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:teecd_data_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:20): avc: denied { getattr } for name="/" dev="mmcblk0p13" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:teecd_data_file:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:21): avc: denied { getattr } for path="/splash2" dev="mmcblk0p19" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:splash2_data_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:22): avc: denied { getattr } for name="/" dev="mmcblk0p19" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:splash2_data_file:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:23): avc: denied { getattr } for path="/cache" dev="mmcblk0p44" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:cache_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:24): avc: denied { getattr } for path="/3rdmodem" dev="mmcblk0p43" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:unlabeled:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:25): avc: denied { getattr } for path="/3rdmodemnvm" dev="mmcblk0p14" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:radio_data_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:26): avc: denied { getattr } for name="/" dev="mmcblk0p14" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:27): avc: denied { getattr } for path="/mnvm2:0" dev="mmcblk0p11" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:modem_nv_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:28): avc: denied { getattr } for name="/" dev="mmcblk0p11" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:modem_nv_file:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:29): avc: denied { getattr } for path="/modem_log" dev="mmcblk0p18" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:modem_log_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:30): avc: denied { getattr } for name="/" dev="mmcblk0p18" ino=2 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:modem_log_file:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:31): avc: denied { getattr } for path="/storage" dev="tmpfs" ino=3652 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:storage_file:s0 tclass=dir permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:32): avc: denied { getattr } for path="/sbin/adbd" dev="mmcblk0p52" ino=1699 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:adbd_exec:s0 tclass=file permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:33): avc: denied { remount } for scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:labeledfs:s0 tclass=filesystem permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:34): avc: denied { read } for name="mmcblk0p52" dev="tmpfs" ino=3430 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:35): avc: denied { open } for path="/dev/block/mmcblk0p52" dev="tmpfs" ino=3430 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:36): avc: denied { ioctl } for path="/dev/block/mmcblk0p52" dev="tmpfs" ino=3430 ioctlcmd=125d scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=1
05-15 01:33:07.769   412   412 I mount   : type=1400 audit(0.0:37): avc: denied { setsched } for scontext=u:r:phhsu_daemon:s0 tcontext=u:r:kernel:s0 tclass=process permissive=1
05-15 01:33:07.769   414   414 I rw-system.sh: type=1400 audit(0.0:38): avc: denied { execute_no_trans } for path="/system/bin/grep" dev="mmcblk0p52" ino=1920 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:system_file:s0 tclass=file permissive=1
05-15 01:33:07.779   416   416 I resize2fs: type=1400 audit(0.0:39): avc: denied { getattr } for path="/dev/block/mmcblk0p52" dev="tmpfs" ino=3430 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=1
05-15 01:33:07.779   416   416 I resize2fs: type=1400 audit(0.0:40): avc: denied { read } for name="swaps" dev="proc" ino=4026532213 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:proc:s0 tclass=file permissive=1
05-15 01:33:07.779   416   416 I resize2fs: type=1400 audit(0.0:41): avc: denied { open } for path="/proc/swaps" dev="proc" ino=4026532213 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:proc:s0 tclass=file permissive=1
05-15 01:33:07.779   416   416 I resize2fs: type=1400 audit(0.0:42): avc: denied { getattr } for path="/proc/swaps" dev="proc" ino=4026532213 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:proc:s0 tclass=file permissive=1
05-15 01:33:07.779   416   416 I resize2fs: type=1400 audit(0.0:43): avc: denied { write } for name="mmcblk0p52" dev="tmpfs" ino=3430 scontext=u:r:phhsu_daemon:s0 tcontext=u:object_r:block_device:s0 tclass=blk_file permissive=1
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:44): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:45): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:46): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:47): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:48): avc: denied { dac_override } for capability=1 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:49): avc: denied { dac_read_search } for capability=2 scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=capability permissive=0
05-15 01:33:07.789   240   240 W modem_sysboot_s: type=1400 audit(0.0:50): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-15 01:33:07.789   240   240 I chatty  : uid=0(root) identical 2 lines
05-15 01:33:07.989   464   464 D vndksupport: Loading /vendor/lib64/hw/android.hardware.keymaster@3.0-impl.so from current namespace instead of sphal namespace.
05-15 01:33:07.996   464   464 E /vendor/bin/hw/android.hardware.keymaster@3.0-service: Failed to dlopen android.hardware.keymaster@3.0-impl.so: dlopen failed: library "libkeymaster1.so" not found
05-15 01:33:07.999   464   464 E android.hardware.keymaster@3.0-service: Could not get passthrough implementation for android.hardware.keymaster@3.0::IKeymasterDevice/default.
--------- beginning of system
05-15 01:33:08.919   477   477 I vold    : Vold 3.0 (the awakening) firing up
05-15 01:33:08.920   477   477 V vold    : Detected support for: exfat ext4 f2fs ntfs vfat
05-15 01:33:08.927   476   476 I android.hardware.keymaster@3.0-impl: Fetching keymaster device name default
05-15 01:33:08.927   476   476 D vndksupport: Loading /vendor/lib64/hw/keystore.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:08.929     1     1 I chatty  : uid=0(root) /init expire 12 lines
05-15 01:33:08.931   477   481 D vold    : e4crypt_init_user0
05-15 01:33:08.931   477   481 D vold    : e4crypt_prepare_user_storage for volume null, user 0, serial 0, flags 1
05-15 01:33:08.931   477   481 D vold    : Preparing: /data/system/users/0
05-15 01:33:08.932   477   481 D vold    : Preparing: /data/misc/profiles/cur/0
05-15 01:33:08.932   477   481 D vold    : Preparing: /data/system_de/0
05-15 01:33:08.932   477   481 D vold    : Preparing: /data/misc_de/0
05-15 01:33:08.932   477   481 D vold    : Preparing: /data/user_de/0
05-15 01:33:08.932   477   481 D vold    : e4crypt_unlock_user_key 0 serial=0 token_present=0
05-15 01:33:08.932   477   481 E vold    : Failed to chmod /data/system_ce/0: No such file or directory
05-15 01:33:08.932   477   481 E vold    : Failed to chmod /data/misc_ce/0: No such file or directory
05-15 01:33:08.932   477   481 E vold    : Failed to chmod /data/media/0: No such file or directory
05-15 01:33:08.935   476   476 I android.hardware.keymaster@3.0-impl: Found keymaster2 module Keymaster2 Hisi HAL, version 200
05-15 01:33:08.935   476   476 I HisiKeyMaster: hisi_km_open start
05-15 01:33:08.936   476   476 E libteec : connect() failed, errno=111, type is 1
05-15 01:33:08.945   482   482 I /system/bin/tzdatacheck: timezone distro dir /data/misc/zoneinfo/current does not exist. No action required.
05-15 01:33:08.945   477   479 V vold    : /system/bin/sgdisk
05-15 01:33:08.945   477   479 V vold    :     --android-dump
05-15 01:33:08.945   477   479 V vold    :     /dev/block/vold/disk:179_192
05-15 01:33:08.947   484   484 I chatty  : uid=0(root) /sbin/cust_init expire 5 lines
05-15 01:33:08.956   346   346 I chatty  : uid=0(root) oeminfo_nvm_ser expire 33 lines
05-15 01:33:08.959   477   479 V vold    : DISK mbr
05-15 01:33:08.959   477   479 V vold    : 
05-15 01:33:08.959   477   479 V vold    : PART 1 c
05-15 01:33:08.959   477   479 V vold    : 
05-15 01:33:08.969   487   487 I chatty  : uid=0(root) expire 1 line
05-15 01:33:08.982   489   489 I chatty  : uid=0(root) expire 1 line
05-15 01:33:08.990   491   491 I chatty  : uid=0(root) expire 1 line
05-15 01:33:08.995   492   492 I chatty  : uid=0(root) expire 1 line
05-15 01:33:08.998   493   493 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.006   494   494 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.014   501   501 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.023   512   512 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.034   498   498 I ServiceManagement: Removing namespace from process name android.hardware.configstore@1.0-service to configstore@1.0.
05-15 01:33:09.047   540   540 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.050   495   495 I ServiceManagement: Removing namespace from process name android.hidl.allocator@1.0-service to allocator@1.0-s.
05-15 01:33:09.059   542   542 I chatty  : uid=0(root) expire 1 line
05-15 01:33:09.073   497   497 I ServiceManagement: Removing namespace from process name android.hardware.bluetooth@1.0-service to bluetooth@1.0-s.
05-15 01:33:09.079   497   497 I android.hardware.bluetooth@1.0-service: Registration complete for android.hardware.bluetooth@1.0::IBluetoothHci/default.
05-15 01:33:09.089   509   509 D vndksupport: Loading /vendor/lib64/hw/vr.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.090   508   508 I chatty  : uid=0(root) /vendor/bin/hw/android.hardware.usb@1.0-service expire 2 lines
05-15 01:33:09.092   521   521 I chatty  : uid=0(root) hwfs@1.0-servic expire 3 lines
05-15 01:33:09.092   502   502 D vndksupport: Loading /vendor/lib64/hw/gatekeeper.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.093   505   505 I ServiceManagement: Removing namespace from process name android.hardware.health@1.0-service to health@1.0-serv.
05-15 01:33:09.101   514   514 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.105   385   385 W /system/bin/hwservicemanager: getTransport: Cannot find entry vendor.huawei.hardware.hwfs@1.0::IHwfs/default in either framework or device manifest.
05-15 01:33:09.107   505   505 I android.hardware.health@1.0-service: Registration complete for android.hardware.health@1.0::IHealth/default.
05-15 01:33:09.108   519   519 D vndksupport: Loading /vendor/lib64/hw/libhwdisplay.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.108   518   518 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:09.109   509   509 I ServiceManagement: Removing namespace from process name android.hardware.vr@1.0-service to vr@1.0-service.
05-15 01:33:09.110   385   385 E SELinux : avc:  denied  { find } for interface=vendor.huawei.hardware.hwdisplay.displayengine::IDisplayEngineWrapper pid=518 scontext=u:r:hal_displayengine_default:s0 tcontext=u:object_r:displayengine_hwservice:s0 tclass=hwservice_manager permissive=0
05-15 01:33:09.117   543   543 I chatty  : uid=0(root) /vendor/bin/irqbalance expire 1 line
05-15 01:33:09.120   509   509 I android.hardware.vr@1.0-service: Registration complete for android.hardware.vr@1.0::IVr/default.
05-15 01:33:09.123   517   517 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.huaweisigntool@1.0-service to huaweisigntool@.
05-15 01:33:09.124   513   513 D vndksupport: Loading /vendor/lib64/hw/mediacomm.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.124   515   515 D HiVRARHal: HIDL_FETCH_IHiVRAR:276: +.
05-15 01:33:09.124   503   503 D vndksupport: Loading /vendor/lib64/hw/gralloc.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.124   515   515 D vndksupport: Loading /vendor/lib64/hw/hivr.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.125   507   507 D vndksupport: Loading /vendor/lib64/hw/thermal.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.127   536   536 I chatty  : uid=0(root) /system/bin/lmkd expire 1 line
05-15 01:33:09.127   496   496 D vndksupport: Loading /vendor/lib64/hw/activity_recognition.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.127   517   517 I vendor.huawei.hardware.huaweisigntool@1.0-service: Registration complete for vendor.huawei.hardware.huaweisigntool@1.0::ISignTool/huaweisigntool.
05-15 01:33:09.128   506   506 D vndksupport: Loading /vendor/lib64/hw/memtrack.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.136   520   520 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwfactoryinterface@1.1-service to hwfactoryinterf.
05-15 01:33:09.138   541   541 I chatty  : uid=0(root) /system/vendor/bin/aptouch_daemon expire 8 lines
05-15 01:33:09.141   532   532 I TS_Service: HIDL_FETCH_ITouchscreen:will get hw_module hw_touchscreen 
05-15 01:33:09.141   532   532 D vndksupport: Loading /vendor/lib64/hw/hw_touchscreen.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.142   506   506 I ServiceManagement: Removing namespace from process name android.hardware.memtrack@1.0-service to memtrack@1.0-se.
05-15 01:33:09.143   506   506 I android.hardware.memtrack@1.0-service: Registration complete for android.hardware.memtrack@1.0::IMemtrack/default.
05-15 01:33:09.146   515   515 D libhivr : HIVRSession:36: HIVRSession is starting
05-15 01:33:09.146   515   515 E libhivr : check_int:47: failed to read /sys/class/graphics/fb0/amoled_vr_mode, or read too long[-1]!
05-15 01:33:09.146   515   515 D libhivr : DSSDevice:51: mAutoRefreshEn=0, mLowPersistenceEn=0, mScene=0, mLcdMode=-1
05-15 01:33:09.146   515   515 D libhivr : PowerPerfDevice:46: mPowerSustainedModeEn=0, mPowerVrModeEn=0
05-15 01:33:09.146   515   515 D HiVRARHal: HIDL_FETCH_IHiVRAR:297: -.
05-15 01:33:09.146   513   513 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.graphics.mediacomm@2.0-service to mediacomm@2.0-s.
05-15 01:33:09.147   548   548 D vndksupport: Loading /vendor/lib64/hw/consumerir.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.147   513   513 I         : Registration complete for vendor.huawei.hardware.graphics.mediacomm@2.0::IMediaComm/default.
05-15 01:33:09.149   507   507 I ServiceManagement: Removing namespace from process name android.hardware.thermal@1.0-service to thermal@1.0-ser.
05-15 01:33:09.150   507   507 I android.hardware.thermal@1.0-service: Registration complete for android.hardware.thermal@1.0::IThermal/default.
05-15 01:33:09.155   516   516 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.huaweiantitheft@1.0-service to huaweiantitheft.
05-15 01:33:09.157   510   510 I DisplayEffectService: Display effect start ......
05-15 01:33:09.157   516   516 I         : Registration complete for vendor.huawei.hardware.huaweiantitheft@1.0::IHuaweiAntiTheft/huaweiantitheft.
05-15 01:33:09.158   510   510 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.graphics.displayeffect@1.0-service to displayeffect@1.
05-15 01:33:09.159   510   510 I vendor.huawei.hardware.graphics.displayeffect@1.0-service: Registration complete for vendor.huawei.hardware.graphics.displayeffect@1.0::IEffect/default.
05-15 01:33:09.161   549   549 E vendor.huawei.hardware.irsl@1.0-impl: HIDL_FETCH_IIrselflearning
05-15 01:33:09.162   549   549 D vndksupport: Loading /vendor/lib64/hw/irselflearning.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.162   514   514 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:09.162   514   514 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:09.163   514   514 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:09.168   526   526 D vndksupport: Loading /vendor/lib64/hw/lights.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.170   527   527 E vendor.huawei.hardware.nfc@1.0-impl: HIDL_FETCH_IHWNfc: ret = 0
05-15 01:33:09.170   527   527 E vendor.huawei.hardware.nfc@1.0-impl: HIDL_FETCH_IHWNfc: load hw lib:/vendor/lib64/hw/nfc_nci.pn54x_45_66t.default.so
05-15 01:33:09.170   527   527 D vndksupport: Loading /vendor/lib64/hw/nfc_nci.pn54x_45_66t.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.172   515   515 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hivrar@1.0-service to hivrar@1.0-serv.
05-15 01:33:09.172   385   385 W /system/bin/hwservicemanager: getTransport: Cannot find entry android.hardware.thermal@1.1::IThermal/default in either framework or device manifest.
05-15 01:33:09.173   538   538 I chatty  : uid=0(root) /system/bin/thermalserviced expire 1 line
05-15 01:33:09.174   515   515 I vendor.huawei.hardware.hivrar@1.0-service: Registration complete for vendor.huawei.hardware.hivrar@1.0::IHiVRAR/default.
05-15 01:33:09.175   385   385 E SELinux : avc:  denied  { find } for interface=vendor.huawei.hardware.hwdisplay.displayengine::IDisplayEngineWrapper pid=518 scontext=u:r:hal_displayengine_default:s0 tcontext=u:object_r:displayengine_hwservice:s0 tclass=hwservice_manager permissive=0
05-15 01:33:09.175   518   518 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:09.175   525   525 D vndksupport: Loading /vendor/lib64/hw/jpeg.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.176   385   385 E SELinux : avc:  denied  { add } for interface=vendor.huawei.hardware.hwdisplay.displayengine::IDisplayEngineWrapper pid=518 scontext=u:r:hal_displayengine_default:s0 tcontext=u:object_r:displayengine_hwservice:s0 tclass=hwservice_manager permissive=0
05-15 01:33:09.176   518   518 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:09.177   549   549 E irda_hal_init: file not exit, use default
05-15 01:33:09.177   549   549 E irda_hal_init: chiptype default as Maxim
05-15 01:33:09.177   532   532 I TS_HAL  : touchscreen_open:Module name: Huawei touchscreen Comm Module
05-15 01:33:09.177   548   548 D ConsumerIrHal: check file
05-15 01:33:09.178   532   532 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.tp@1.0-service to tp@1.0-service.
05-15 01:33:09.179   532   532 I vendor.huawei.hardware.tp@1.0-service: Registration complete for vendor.huawei.hardware.tp@1.0::ITouchscreen/default.
05-15 01:33:09.179   522   522 D vndksupport: Loading /vendor/lib64/hw/vibrator.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.181   531   531 D vndksupport: Loading /vendor/lib64/hw/sensors.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.182   477   481 D VoldCryptCmdListener: cryptfs mountdefaultencrypted
05-15 01:33:09.182   526   526 D vndksupport: Loading /vendor/lib64/hw/lights.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.184   526   526 I chatty  : uid=1000(system) light@2.0-servi identical 11 lines
05-15 01:33:09.184   526   526 D vndksupport: Loading /vendor/lib64/hw/lights.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.185   526   526 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.light@2.0-service to light@2.0-servi.
05-15 01:33:09.186   526   526 I vendor.huawei.hardware.light@2.0-service: Registration complete for vendor.huawei.hardware.light@2.0::ILight/default.
05-15 01:33:09.187   522   522 D         : Vibrator using timed_output
05-15 01:33:09.187   522   522 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwvibrator@1.0-service to hwvibrator@1.0-.
05-15 01:33:09.187   529   529 I PF_PG   : Construct perfgenius
05-15 01:33:09.188   529   529 D PF_PH   : open path [/sys/devices/system/cpu/cpufreq/boost] failed
05-15 01:33:09.188   522   522 I vendor.huawei.hardware.hwvibrator@1.0-service: Registration complete for vendor.huawei.hardware.hwvibrator@1.0::IHWVibrator/default.
05-15 01:33:09.189   572   575 W libc    : Set property "sys.usb.ffs_hdb.ready" to "1"
05-15 01:33:09.191   572   576 I cutils-trace: atrace_init_once, trace_marker_path = /sys/kernel/debug/tracing/trace_marker
05-15 01:33:09.192   527   527 E HAL     : load: id=nfc_nci.pn54x_45_66t != hmi->id=nfc_nci.pn54x
05-15 01:33:09.192   477   570 I Cryptfs : cryptfs_check_passwd
05-15 01:33:09.192   527   527 E vendor.huawei.hardware.nfc@1.0-impl: HIDL_FETCH_IHWNfc: load hw lib:/vendor/lib64/hw/nfc_nci.pn54x.default.so
05-15 01:33:09.193   527   527 D vndksupport: Loading /vendor/lib64/hw/nfc_nci.pn54x.default.so from current namespace instead of sphal namespace.
05-15 01:33:09.193   525   525 E jpeg_dec: jpeg_device_open:1189: /dev/hisi_jpu open failed
05-15 01:33:09.193   525   525 E JpegDecode: failed to open jpeg decode device: Operation not permitted
05-15 01:33:09.193   549   549 E irda_hal_init: init maxim driver success
05-15 01:33:09.193   548   548 I ConsumerIrHal: find permission file /product/etc/permissions/android.hardware.consumerir.xml
05-15 01:33:09.194   548   548 E irda_hal_init: file not exit, use default
05-15 01:33:09.194   548   548 E irda_hal_init: chiptype default as Maxim
05-15 01:33:09.194   525   525 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.jpegdec@1.0-service to jpegdec@1.0-ser.
05-15 01:33:09.194   548   548 E irda_hal_init: init maxim driver success
05-15 01:33:09.194   548   548 D ConsumerIrHal: Open Consumer IR HAL
05-15 01:33:09.194   549   549 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.irsl@1.0-service to irsl@1.0-servic.
05-15 01:33:09.194   525   525 I vendor.huawei.hardware.jpegdec@1.0-service: Registration complete for vendor.huawei.hardware.jpegdec@1.0::IJpegDecode/default.
05-15 01:33:09.195   549   549 I vendor.huawei.hardware.irsl@1.0-service: Registration complete for vendor.huawei.hardware.irsl@1.0::IIrselflearning/irselflearning.
05-15 01:33:09.195   548   548 I ServiceManagement: Removing namespace from process name android.hardware.ir@1.0-service to ir@1.0-service.
05-15 01:33:09.196   548   548 I android.hardware.ir@1.0-service: Registration complete for android.hardware.ir@1.0::IConsumerIr/default.
05-15 01:33:09.196   529   529 D         : [xmlFilesLoad:69] Load XML File [/vendor/etc/perfgenius_boost_policy.xml] Succeed
05-15 01:33:09.197   529   529 D         : [xmlFilesLoad:69] Load XML File [/vendor/etc/perfgenius_config.xml] Succeed
05-15 01:33:09.197   529   529 E PF_CM   : [createGovernorHandleObject:331] no valid scene.
05-15 01:33:09.199   477   570 D Cryptfs : crypt_ftr->fs_size = 52608992
05-15 01:33:09.199   477   570 I Cryptfs : Using scrypt with keymaster for cryptfs KDF
05-15 01:33:09.199   529   529 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.perfgenius@1.0-service to perfgenius@1.0-.
05-15 01:33:09.200   530   530 D vndksupport: Loading /vendor/lib64/hw/power.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.200   504   504 D vndksupport: Loading /vendor/lib64/hw/hwcomposer.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.201   529   529 I vendor.huawei.hardware.perfgenius@1.0-service: Registration complete for vendor.huawei.hardware.perfgenius@1.0::IPerfGenius/perfgenius.
05-15 01:33:09.202   476   476 I HisiKeyMaster: hisi_km_open success
05-15 01:33:09.202   476   476 I HisiKeyMaster: hisi_km_configure start
05-15 01:33:09.202   476   476 I HisiKeyMaster: Disable the enhanced crypto!
05-15 01:33:09.203   531   531 I chatty  : uid=1000(system) /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service expire 63 lines
05-15 01:33:09.208   502   502 I ServiceManagement: Removing namespace from process name android.hardware.gatekeeper@1.0-service to gatekeeper@1.0-.
05-15 01:33:09.209   530   530 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.power@1.0-service to power@1.0-servi.
05-15 01:33:09.209   502   502 I android.hardware.gatekeeper@1.0-service: Registration complete for android.hardware.gatekeeper@1.0::IGatekeeper/default.
05-15 01:33:09.210   530   530 I vendor.huawei.hardware.power@1.0-service: Registration complete for vendor.huawei.hardware.power@1.0::IHWPower/default.
05-15 01:33:09.212   519   519 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay@1.0-service to hwdisplay@1.0-s.
05-15 01:33:09.212   527   527 D NxpNfcNciHal: nfc_open: enter; name=nci
05-15 01:33:09.212   527   527 D NxpNfcNciHal: nfc_open: exit 0
05-15 01:33:09.213   519   519 I vendor.huawei.hardware.hwdisplay@1.0-service: Registration complete for vendor.huawei.hardware.hwdisplay@1.0::IDisplay/default.
05-15 01:33:09.213   527   527 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.nfc@1.0-service to nfc@1.0-service.
05-15 01:33:09.214   527   527 I vendor.huawei.hardware.nfc@1.0-service: Registration complete for vendor.huawei.hardware.nfc@1.0::IHWNfc/default.
05-15 01:33:09.215   476   476 I HisiKeyMaster: open first km session
05-15 01:33:09.216   476   476 I HisiKeyMaster: hisi_km_configure success
05-15 01:33:09.217   476   476 I ServiceManagement: Removing namespace from process name android.hardware.keymaster@3.0-service to keymaster@3.0-s.
05-15 01:33:09.218   476   476 I android.hardware.keymaster@3.0-service: Registration complete for android.hardware.keymaster@3.0::IKeymasterDevice/default.
05-15 01:33:09.221   528   528 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.otherdevices@1.0-service to otherdevices@1..
05-15 01:33:09.222   528   528 I         : Registration complete for vendor.huawei.hardware.otherdevices@1.0::IOtherdevices/default.
05-15 01:33:09.235   524   524 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.iawareperf@1.0-service to iawareperf@1.0-.
05-15 01:33:09.236   524   524 I vendor.huawei.hardware.iawareperf@1.0-service: Registration complete for vendor.huawei.hardware.iawareperf@1.0::IUniPerf/uniperf.
05-15 01:33:09.267   571   607 I adbd    : initializing functionfs
05-15 01:33:09.267   571   607 I adbd    : opening control endpoint /dev/usb-ffs/adb/ep0
05-15 01:33:09.278   496   496 I ArHal   : (ar_device_open:132):open module [activity_recognition_hidl].
05-15 01:33:09.278   496   496 I ArComm  : (comm_dev_init:684):enter.
05-15 01:33:09.278   496   496 I ARLog   : (ar_log_init:204):no [/etc/activity_recognition.conf].
05-15 01:33:09.278   496   496 I ArComm  : (comm_netlink_init:350):enter.
05-15 01:33:09.278   496   496 I ArComm  : (comm_netlink_socket_setup:323):enter. fd[7]
05-15 01:33:09.278   496   496 I ArComm  : (comm_thread_create:235):success, tid[0x78e86904f0]
05-15 01:33:09.278   496   496 I ArData  : (ar_data_setup:1001):id[2].
05-15 01:33:09.278   496   496 I ArComm  : (comm_thread_create:235):success, tid[0x78e85934f0]
05-15 01:33:09.278   496   496 I AR_ENV  : (ar_env_setup:566):<<<<ar env running>>>>
05-15 01:33:09.278   496   496 I AR_ENV  : (ar_env_get_dev:465):can't find dev
05-15 01:33:09.278   496   496 I AR_ENV  : (ar_env_feature_switch_config:685):env feature off.
05-15 01:33:09.278   496   496 E AR_ENV  : (ar_env_setup:574):not support env
05-15 01:33:09.278   496   496 I ArHal   : (ar_device_open:181):open module [activity_recognition_hidl] v1.2 successfully.
05-15 01:33:09.278   496   611 I ArComm  : (comm_netlink_thread:429):thread start.
05-15 01:33:09.279   496   611 I ArComm  : (comm_netlink_thread:440):wakelock[COMMNL_201F0].
05-15 01:33:09.280   496   496 I vendor.hisi.hardware.activity_recognition@1.0-service: Registration complete for vendor.huawei.hardware.activity_recognition@1.0::IActivityRecognition/default.
05-15 01:33:09.285   503   503 I ServiceManagement: Removing namespace from process name android.hardware.graphics.allocator@2.0-service to allocator@2.0-s.
05-15 01:33:09.286   503   503 I android.hardware.graphics.allocator@2.0-service: Registration complete for android.hardware.graphics.allocator@2.0::IAllocator/default.
05-15 01:33:09.289    87    87 I chatty  : uid=0(root) kworker/u16:1 expire 1 line
05-15 01:33:09.302   504   504 W hwcomposer: Connect:280: Disp0 resolution(1080 x 1920), fps: 60 Hz.
05-15 01:33:09.302   504   504 D vndksupport: Loading /vendor/lib64/hw/gralloc.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.306   504   504 I GRALLOC : 	 shrFd=25,fmt=0x1,intFmt=0x200000001,btStrd=4352,size=8486912,pid=504 
05-15 01:33:09.306   504   504 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:09.306   504   504 I GRALLOC : 	 iova_size=8486912,conUsg=0x0,proUsg=0x900,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 1 
05-15 01:33:09.306   504   504 I GRALLOC : 	 shrFd=27,fmt=0x1,intFmt=0x200000001,btStrd=4352,size=8486912,pid=504 
05-15 01:33:09.306   504   504 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:09.306   504   504 I GRALLOC : 	 iova_size=8486912,conUsg=0x0,proUsg=0x900,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 2 
05-15 01:33:09.306   504   504 I GRALLOC : 	 shrFd=29,fmt=0x1,intFmt=0x200000001,btStrd=4352,size=8486912,pid=504 
05-15 01:33:09.306   504   504 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:09.306   504   504 I GRALLOC : 	 iova_size=8486912,conUsg=0x0,proUsg=0x900,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 3 
05-15 01:33:09.308   504   504 I ServiceManagement: Removing namespace from process name android.hardware.graphics.composer@2.1-service to composer@2.1-se.
05-15 01:33:09.309   504   504 I android.hardware.graphics.composer@2.1-service: Registration complete for android.hardware.graphics.composer@2.1::IComposer/default.
05-15 01:33:09.315   533   533 I vendor.huawei.hardware.hwwifiext@1.1-service: WIFI VENDOR HAL STARTING.
05-15 01:33:09.315   533   533 I vendor.huawei.hardware.wifi@1.1-service: Wifi Hal 1.1 is starting up...
05-15 01:33:09.333   533   533 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.wifi@1.1-service to wifi@1.1-servic.
05-15 01:33:09.333   533   533 I vendor.huawei.hardware.hwwifiext@1.1-service: Registration complete for vendor.huawei.hardware.wifi@1.1::IHwWifiExt/default.
05-15 01:33:09.344   511   511 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 29 lines
05-15 01:33:09.360   610   610 I chatty  : uid=0(root) /vendor/bin/atcmdserver expire 8 lines
05-15 01:33:09.384   499   499 I chatty  : uid=1013(media) /vendor/bin/hw/android.hardware.drm@1.0-service expire 5 lines
05-15 01:33:09.392   500   500 I chatty  : uid=1013(media) drm@1.0-service expire 3 lines
05-15 01:33:09.394   385   385 I chatty  : uid=1000(system) hwservicemanage expire 11 lines
05-15 01:33:09.429   537   537 I chatty  : uid=1000(system) /system/bin/surfaceflinger expire 31 lines
05-15 01:33:09.468   571   607 I adbd    : functionfs successfully initialized
05-15 01:33:09.468   571   607 I adbd    : registering usb transport
05-15 01:33:09.583   537   537 I SurfaceFlinger: GL_MAX_TEXTURE_SIZE = 8192
05-15 01:33:09.583   537   537 I SurfaceFlinger: GL_MAX_VIEWPORT_DIMS = 8192
05-15 01:33:09.590   504   504 D vndksupport: Loading /vendor/lib64/hw/gralloc.hi3650.so from current namespace instead of sphal namespace.
05-15 01:33:09.594   537   537 D mali_winsys: EGLint new_window_surface(egl_winsys_display *, void *, EGLSurface, EGLConfig, egl_winsys_surface **, egl_color_buffer_format *, EGLBoolean) returns 0x3000
05-15 01:33:09.606   503   503 I GRALLOC : 	 shrFd=10,fmt=0x1,intFmt=0x200000001,btStrd=4352,size=8486912,pid=503 
05-15 01:33:09.606   503   503 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:09.606   503   503 I GRALLOC : 	 iova_size=8486912,conUsg=0x1a00,proUsg=0x1a00,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 1 
05-15 01:33:09.606   503   503 I chatty  : uid=1000(system) allocator@2.0-s identical 1 line
05-15 01:33:09.607   503   503 I GRALLOC : 	 shrFd=10,fmt=0x1,intFmt=0x200000001,btStrd=4352,size=8486912,pid=503 
05-15 01:33:09.607   503   503 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:09.607   503   503 I GRALLOC : 	 iova_size=8486912,conUsg=0x1a00,proUsg=0x1a00,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 1 
05-15 01:33:09.713   477   570 I Cryptfs : Signing safely-padded object
05-15 01:33:09.716   476   476 I HisiKeyMaster: hisi_km_begin start
05-15 01:33:09.716   476   476 I HisiKeyMaster: Disable the enhanced crypto!
05-15 01:33:09.724   476   476 I HisiKeyMaster: out_params_buffer_len = 4096
05-15 01:33:09.724   476   476 I HisiKeyMaster: hisi_km_begin success
05-15 01:33:09.724   476   476 I HisiKeyMaster: Disable the enhanced crypto!
05-15 01:33:09.729   476   476 I HisiKeyMaster: hisi_km_finish start
05-15 01:33:09.729   476   476 I HisiKeyMaster: Disable the enhanced crypto!
05-15 01:33:09.762   537   537 D SurfaceFlinger: shader cache generated - 24 shaders in 154.702606 ms
05-15 01:33:09.764   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:09.774   476   476 I HisiKeyMaster: output data size=256
05-15 01:33:09.774   476   476 I HisiKeyMaster: hisi_km_finish success
05-15 01:33:10.160   660   663 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:10.179   660   663 I /system/bin/bootanimation: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasWideColorDisplay retrieved: 0
05-15 01:33:10.180   660   663 D mali_winsys: EGLint new_window_surface(egl_winsys_display *, void *, EGLSurface, EGLConfig, egl_winsys_surface **, egl_color_buffer_format *, EGLBoolean) returns 0x3000
05-15 01:33:10.181   660   663 D BootAnimation: BootAnimationShownTiming start time: 7439ms
05-15 01:33:10.213   503   503 I GRALLOC : 	 shrFd=10,fmt=0x2,intFmt=0x200000002,btStrd=4352,size=8486912,pid=503 
05-15 01:33:10.213   503   503 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:10.213   503   503 I GRALLOC : 	 iova_size=8486912,conUsg=0xb00,proUsg=0xb00,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 1 
05-15 01:33:10.220   503   503 I GRALLOC : 	 shrFd=10,fmt=0x2,intFmt=0x200000002,btStrd=4352,size=8486912,pid=503 
05-15 01:33:10.220   503   503 I GRALLOC : 	 yuv=2,w=1080,h=1920,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:10.220   503   503 I GRALLOC : 	 iova_size=8486912,conUsg=0xb00,proUsg=0xb00,	 strd=1088,[afbc]HdrStrd=1088 PyldStrd=69632 Scrmbl=0,ionhnd = 1 
05-15 01:33:10.285   477   570 I Cryptfs : Enabling support for allow_discards in dmcrypt.
05-15 01:33:10.287   477   479 D vold    : Disk at 253:0 changed
05-15 01:33:10.809   477   570 I Cryptfs : Password matches
05-15 01:33:10.809   477   570 D Cryptfs : test_mount_encrypted_fs(): Master key saved
05-15 01:33:10.810   477   570 D Cryptfs : Password is default - restarting filesystem
05-15 01:33:10.842   477   570 D Cryptfs : unmounting /data succeeded
05-15 01:33:10.842   477   570 I vold    : [libfs_mgr]Running /system/bin/fsck.f2fs -a /dev/block/dm-0
05-15 01:33:10.920   477   570 I vold    : [libfs_mgr]__mount(source=/dev/block/dm-0,target=/data,type=f2fs)=0: Success
05-15 01:33:10.920   477   570 D Cryptfs : Just triggered post_fs_data
05-15 01:33:10.955   477   481 D vold    : e4crypt_init_user0
05-15 01:33:10.955   477   481 D vold    : e4crypt_prepare_user_storage for volume null, user 0, serial 0, flags 1
05-15 01:33:10.955   477   481 D vold    : Preparing: /data/system/users/0
05-15 01:33:10.956   477   481 D vold    : Preparing: /data/misc/profiles/cur/0
05-15 01:33:10.957   477   481 D vold    : Preparing: /data/system_de/0
05-15 01:33:10.957   477   481 D vold    : Preparing: /data/misc_de/0
05-15 01:33:10.958   477   481 D vold    : Preparing: /data/user_de/0
05-15 01:33:10.958   477   481 D vold    : e4crypt_unlock_user_key 0 serial=0 token_present=0
05-15 01:33:10.958   477   481 E vold    : Failed to chmod /data/system_ce/0: No such file or directory
05-15 01:33:10.958   477   481 E vold    : Failed to chmod /data/misc_ce/0: No such file or directory
05-15 01:33:10.958   477   481 E vold    : Failed to chmod /data/media/0: No such file or directory
05-15 01:33:10.972   705   705 I /system/bin/tzdatacheck: timezone distro dir /data/misc/zoneinfo/current does not exist. No action required.
05-15 01:33:10.977   706   706 I chatty  : uid=0(root) /sbin/cust_init expire 5 lines
05-15 01:33:11.020   711   711 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.032   713   713 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.040   714   714 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.047   715   715 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.056   477   570 D Cryptfs : post_fs_data done
05-15 01:33:11.056   716   716 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.058   477   570 D Cryptfs : Just triggered restart_framework
05-15 01:33:11.063   717   717 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.064   718   718 I bootstat: Service started: /system/bin/bootstat -r post_decrypt_time_elapsed 
05-15 01:33:11.071   719   719 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.092   722   722 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.099   723   723 I chatty  : uid=0(root) expire 1 line
05-15 01:33:11.132   733   733 I installd: installd firing up
05-15 01:33:11.145   756   756 I chatty  : uid=0(root) /sbin/logctl_service expire 2 lines
05-15 01:33:11.146   744   744 I chatty  : uid=0(root) /vendor/bin/check_root expire 4 lines
05-15 01:33:11.156   753   753 I chatty  : uid=0(root) /vendor/bin/mac_addr_normalization expire 1 line
05-15 01:33:11.167   346   346 E         : oeminfo_read:oeminfo data not find !!!!
05-15 01:33:11.167   346   346 E         : 
05-15 01:33:11.167   346   346 E         : oeminfo_read_data, fail to read oeminfo
05-15 01:33:11.167   346   346 E         : 
05-15 01:33:11.167   346   346 E         : pid 757, opration oeminfo_read FAIL
05-15 01:33:11.167   346   346 E         : 
05-15 01:33:11.168   346   346 E         : pid 753, opration nvm_read OK
05-15 01:33:11.168   346   346 E         : 
05-15 01:33:11.168   753   753 I         : macaddr[1] = 52
05-15 01:33:11.168   757   757 E         : rmt_oeminfo_read, get data from server fail
05-15 01:33:11.170   750   750 I perfprofd: starting Android Wide Profiling daemon
05-15 01:33:11.183   346   346 E         : pid 744, opration oeminfo_read OK
05-15 01:33:11.183   346   346 E         : 
05-15 01:33:11.186   750   750 E perfprofd: unable to open configuration file /data/data/com.google.android.gms/files/perfprofd.conf
05-15 01:33:11.187   750   750 I perfprofd: random seed set to 593879668
05-15 01:33:11.196   754   754 E         : [gpsdaemon] is Commercial User  
05-15 01:33:11.196   754   754 E         : [gpsdaemon]  pid = 754, ppid = 1
05-15 01:33:11.196   754   754 E         : 
05-15 01:33:11.196   754   754 E         : [gpsdaemon] will delete path is rm /data/gps/crash.cont 
05-15 01:33:11.198   346   346 E         : oeminfo_read:oeminfo data not find !!!!
05-15 01:33:11.198   346   346 E         : 
05-15 01:33:11.199   346   346 E         : oeminfo_read_data, fail to read oeminfo
05-15 01:33:11.199   346   346 E         : 
05-15 01:33:11.199   346   346 E         : pid 1, opration oeminfo_read FAIL
05-15 01:33:11.199   346   346 E         : 
05-15 01:33:11.199   346   346 E         : pid 753, opration nvm_read OK
05-15 01:33:11.199   346   346 E         : 
05-15 01:33:11.199   753   753 I         : read mac from nv finished,wifi status = 1, bt status = 1
05-15 01:33:11.199   346   346 E         : pid 757, opration nvm_read OK
05-15 01:33:11.199   346   346 E         : 
05-15 01:33:11.199   753   753 I mac_addr: macaddr_file_dir is /data/misc/wifi/macwifi
05-15 01:33:11.201   752   752 I hinetmanager: hinetmanager starts.
05-15 01:33:11.201   752   752 I hinetmanager: init_hinetmagager
05-15 01:33:11.201   752   752 I hinetmanager: hinetmanager first start
05-15 01:33:11.210   753   753 I mac_addr: macaddr_file_dir is /data/misc/bluedroid/macbt
05-15 01:33:11.214   737   737 I chatty  : uid=1013 mediametrics expire 3 lines
05-15 01:33:11.216   755   755 I FusionDaemon: (main:1195):fusion deamon started. V2.1.23.1
05-15 01:33:11.218   741   741 I wificond: wificond is starting up...
05-15 01:33:11.219   752   752 I hinetmanager_record: file path exists.
05-15 01:33:11.221   346   346 E         : pid 1, opration oeminfo_read OK
05-15 01:33:11.221   346   346 E         : 
05-15 01:33:11.221   744   744 E check_root: write_result_to_persist:set dev status flag
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_dev_init:463):enter.
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_init:141):enter.
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_socket_setup:114):enter. fd[8]
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_thread_create:64):success, tid[0x78d4ddd4f0]
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_dev_init:463):enter.
05-15 01:33:11.224   755   765 I FusionDaemon: (comm_netlink_thread:225):thread start.
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_init:141):enter.
05-15 01:33:11.224   740   763 I ServiceManager: Waiting for service package_native...
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_socket_setup:114):enter. fd[9]
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_thread_create:64):success, tid[0x78d4ce04f0]
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_dev_init:463):enter.
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_init:141):enter.
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_netlink_socket_setup:114):enter. fd[10]
05-15 01:33:11.224   755   755 I FusionDaemon: (comm_thread_create:64):success, tid[0x78d4be34f0]
05-15 01:33:11.225   755   767 I FusionDaemon: (comm_netlink_thread:225):thread start.
05-15 01:33:11.228   755   766 I FusionDaemon: (comm_netlink_thread:225):thread start.
05-15 01:33:11.235   755   755 I         : [gnsslog_higeo_get_fused_logmgr_interface]
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_set_logmgr_config]higeo_log_level=0, higeo_log_size=1, higeo_log_num_max_limit=800
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_set_logmgr_config] log level is commercial(0)
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_init_logmgr]
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_init_logmgr] log level is commercial(0)
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_run_logmgr]
05-15 01:33:11.235   755   755 I         : [gnsslog_gnss_run_logmgr] log level is commercial(0)
05-15 01:33:11.240   751   751 I /system/bin/tombstoned: tombstoned successfully initialized
05-15 01:33:11.241   749   749 I gatekeeperd: Starting gatekeeperd...
05-15 01:33:11.243   759   759 I chatty  : uid=1000(system) fingerprint@2.1 expire 25 lines
05-15 01:33:11.256   746   746 I chatty  : uid=1013(media) /vendor/bin/CameraDaemon expire 1502 lines
05-15 01:33:11.256   752   752 I hinetmanager_record: init record files done
05-15 01:33:11.257   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:11.259   752   752 D hinetmanager: registerhinetmanagerService return status =0
05-15 01:33:11.259   752   752 I hinetmanager_nmgrsocket: init_hinetmanager_client_socket
05-15 01:33:11.272   755   755 I FusionDaemon: (init:98):fused_manager.so loaded
05-15 01:33:11.272   755   755 I FusionDaemon: (comm_thread_create:64):success, tid[0x78d47924f0]
05-15 01:33:11.280   755   755 I NamedPipeComm: (init:97):NamedPipeComm init done
05-15 01:33:11.280   755   755 I FusionDaemon: (FusdLbs:35):FusdLbs: open HAL.
05-15 01:33:11.295   736   736 V MediaUtils: physMem: 3844882432
05-15 01:33:11.295   736   736 V MediaUtils: requested limit: 768976480
05-15 01:33:11.295   736   736 V MediaUtils: cfi shadow size: 2147483648
05-15 01:33:11.295   736   736 V MediaUtils: actual limit: 2916460128
05-15 01:33:11.295   736   736 V MediaUtils: original limits: -1/-1
05-15 01:33:11.295   736   736 V MediaUtils: new limits: 2916460128/-1
05-15 01:33:11.301   745   745 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:11.301   745   745 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:11.301   745   745 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:11.301   745   745 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:11.301   745   745 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:11.303   754   754 E         : [gpsdaemon] after rm crash.cont file
05-15 01:33:11.303   754   754 E         : [gpsdaemon] Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:11.303   754   754 E         : 
05-15 01:33:11.303   754   754 E         : [gpsdaemon] To get Gps IC type 4774
05-15 01:33:11.303   754   754 E         : [gpsdaemon] the gps_ic_type is 4774
05-15 01:33:11.303   754   754 E         : [gpsdaemon] GPS_CopyConfigFile entry ...
05-15 01:33:11.303   754   754 E         : [gpsdaemon]  GPS_Loadxmlfile entry filename:/vendor/etc/gps4774config.xml ... 
05-15 01:33:11.309   754   754 E         : [gpsdaemon]  GPS_Loadxmlfile out  ... 
05-15 01:33:11.310   754   754 E         : [gpsdaemon]Open /proc/device-tree/gps_power/broadcom_config,tty_port success!
05-15 01:33:11.310   754   754 E         : [gpsdaemon] [gpsdaemon]tty port is ttyAMA3
05-15 01:33:11.310   754   754 E         : 
05-15 01:33:11.310   754   754 E         : [gpsdaemon]  GPS_CopyConfigFile start save /data/gps/gpsconfig.xml  
05-15 01:33:11.310   742   742 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:11.310   742   742 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:11.310   742   742 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:11.310   742   742 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:11.310   742   742 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:11.310   739   739 I Netd    : Netd 1.0 starting
05-15 01:33:11.312   736   736 W /system/bin/mediaextractor: Could not read additional policy file '/vendor/etc/seccomp_policy/mediaextractor.policy'
05-15 01:33:11.312   736   736 W /system/bin/mediaextractor: libminijail[736]: allowing syscall: connect
05-15 01:33:11.312   736   736 W /system/bin/mediaextractor: libminijail[736]: allowing syscall: fcntl
05-15 01:33:11.312   736   736 W /system/bin/mediaextractor: libminijail[736]: allowing syscall: sendto
05-15 01:33:11.313   736   736 W /system/bin/mediaextractor: libminijail[736]: allowing syscall: socket
05-15 01:33:11.313   736   736 W /system/bin/mediaextractor: libminijail[736]: allowing syscall: writev
05-15 01:33:11.313   736   736 W /system/bin/mediaextractor: libminijail[736]: compile_file: nonexistent syscall '_llseek'
05-15 01:33:11.313   736   736 W /system/bin/mediaextractor: libminijail[736]: logging seccomp filter failures
05-15 01:33:11.313   727   727 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:11.314   754   754 E         : [gpsdaemon]  GPS_CopyConfigFile start save /data/gps/gpsconfig.xml, ret = 4913  
05-15 01:33:11.316   754   754 E         : [gpsdaemon] system do cp gpsconfig work done!
05-15 01:33:11.317   754   754 E         : [gpsdaemon]  main  copyGpsConfigFile end
05-15 01:33:11.317   754   754 E         : [gpsdaemon] srcFile = /vendor/etc/lhd.conf,dtsFilePath = /data/gps/lhd.conf
05-15 01:33:11.321   739   739 D TetherController: Setting IP forward enable = 0
05-15 01:33:11.326   742   742 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:11.326   745   745 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:11.327   745   745 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:11.327   742   742 E GnssHAL_GnssInterface: hw_get_module failed......try to get gps.default
05-15 01:33:11.327   742   742 D vndksupport: Loading /vendor/lib64/hw/gps.default.so from current namespace instead of sphal namespace.
05-15 01:33:11.327   745   745 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:11.332   754   754 E         : [gpsdaemon] system do cp gpsconfig work done!
05-15 01:33:11.333   754   754 E         : [gpsdaemon] srcFile = /vendor/etc/SensorHub.patch,dtsFilePath = /data/gps/SensorHub.patch
05-15 01:33:11.351   742   742 E GnssHAL_GnssInterface: hw_get_module err=0
05-15 01:33:11.352   742   742 I ServiceManagement: Removing namespace from process name android.hardware.gnss@1.0-service to gnss@1.0-servic.
05-15 01:33:11.353   742   742 I android.hardware.gnss@1.0-service: Registration complete for android.hardware.gnss@1.0::IGnss/default.
05-15 01:33:11.366   739   739 I Netd    : Creating child chains: 40.8ms
05-15 01:33:11.366   739   739 I Netd    : Setting up OEM hooks: 0.1ms
05-15 01:33:11.368   739   739 I Netd    : Setting up FirewallController hooks: 1.9ms
05-15 01:33:11.369   739   739 I Netd    : Setting up NatController hooks: 1.2ms
05-15 01:33:11.370   739   739 I Netd    : Setting up BandwidthController hooks: 1.1ms
05-15 01:33:11.370   739   739 I Netd    : Setting up IdletimerController hooks: 0.0ms
05-15 01:33:11.372   739   739 I Netd    : Disabling bandwidth control: 2.3ms
05-15 01:33:11.373   739   739 E Netd    : cannot find interface dummy0
05-15 01:33:11.377   754   754 E         : [gpsdaemon] system do cp gpsconfig work done!
05-15 01:33:11.378   754   754 E         : [gpsdaemon] start service lhd_4774
05-15 01:33:11.380   754   754 E         : [gpsdaemon] start service gpsd_4774
05-15 01:33:11.381   739   739 I Netd    : Initializing RouteController: 8.8ms
05-15 01:33:11.382   739   739 E Netd    : Unable to create netlink socket: Protocol not supported
05-15 01:33:11.382   739   739 W Netd    : Unable to open qlog quota socket, check if xt_quota2 can send via UeventHandler
05-15 01:33:11.382   739   739 D MDnsDS  : MDnsSdListener::Hander starting up
05-15 01:33:11.382   739   801 D MDnsDS  : MDnsSdListener starting to monitor
05-15 01:33:11.382   739   801 D MDnsDS  : Going to poll with pollCount 1
05-15 01:33:11.383   739   739 I Netd    : Registering NetdNativeService: 1.1ms
05-15 01:33:11.383   739   739 I Netd    : Starting CommandListener: 0.1ms
05-15 01:33:11.385   739   739 I Netd    : Registering NetdHwService: 1.7ms
05-15 01:33:11.385   739   739 I Netd    : Netd started in 75ms
05-15 01:33:11.404   757   757 W libc    : Set property "ctl.stop" to "kmsglogcat"
05-15 01:33:11.404   757   757 W libc    : Set property "ctl.stop" to "chargelogcat"
05-15 01:33:11.404   757   757 W libc    : Set property "ctl.stop" to "isplogcat"
05-15 01:33:11.405   757   757 W libc    : Set property "ctl.stop" to "shex"
05-15 01:33:11.405   757   757 W libc    : Set property "ctl.stop" to "shlogd"
05-15 01:33:11.406   757   757 W libc    : Set property "ctl.stop" to "applogcat"
05-15 01:33:11.406   757   757 W libc    : Set property "ctl.stop" to "rillogcat"
05-15 01:33:11.406   757   757 W libc    : Set property "ctl.stop" to "eventslogcat"
05-15 01:33:11.406   757   757 W libc    : Set property "ctl.stop" to "kmsgcat_cp"
05-15 01:33:11.406   757   757 W libc    : Set property "ctl.stop" to "inputlogcat"
05-15 01:33:11.407   757   757 W libc    : Set property "ctl.stop" to "sleeplogcat"
05-15 01:33:11.407   757   757 W libc    : Set property "ctl.stop" to "hilogcat"
05-15 01:33:11.407   757   757 W libc    : Set property "ctl.stop" to "logcat_service"
05-15 01:33:11.412   793   793 V lhd     : GlLhdInterface::Init(/data/gps/lhd.conf)
05-15 01:33:11.412   793   793 V lhd     : SetCfgValue: LHD config "LheRsmResetTimeoutMS"="10000"
05-15 01:33:11.412   793   793 V lhd     : SetCfgValue: LHD config "LhePatch"="/data/gps/SensorHub.patch"
05-15 01:33:11.412   793   793 V lhd     : SetCfgValue: LHD config "LheConsole"="/data/gps/LheConsole"
05-15 01:33:11.459   735   735 I chatty  : uid=1013(media) /system/bin/mediadrmserver expire 1 line
05-15 01:33:11.486   727   727 I zygote64: option[0]=-Xzygote
05-15 01:33:11.486   727   727 I zygote64: option[1]=-Xusetombstonedtraces
05-15 01:33:11.486   727   727 I zygote64: option[2]=exit
05-15 01:33:11.486   727   727 I zygote64: option[3]=vfprintf
05-15 01:33:11.486   727   727 I zygote64: option[4]=sensitiveThread
05-15 01:33:11.486   727   727 I zygote64: option[5]=-verbose:gc
05-15 01:33:11.486   727   727 I zygote64: option[6]=-Xms8m
05-15 01:33:11.486   727   727 I zygote64: option[7]=-Xmx512m
05-15 01:33:11.486   727   727 I zygote64: option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:11.486   727   727 I zygote64: option[9]=-XX:HeapMinFree=2m
05-15 01:33:11.486   727   727 I zygote64: option[10]=-XX:HeapMaxFree=8m
05-15 01:33:11.486   727   727 I zygote64: option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:11.486   727   727 I zygote64: option[12]=-Xusejit:true
05-15 01:33:11.486   727   727 I zygote64: option[13]=-Xjitsaveprofilinginfo
05-15 01:33:11.486   727   727 I zygote64: option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:11.486   727   727 I zygote64: option[15]=-Xlockprofthreshold:500
05-15 01:33:11.486   727   727 I zygote64: option[16]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[17]=--runtime-arg
05-15 01:33:11.486   727   727 I zygote64: option[18]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[19]=-Xms64m
05-15 01:33:11.486   727   727 I zygote64: option[20]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[21]=--runtime-arg
05-15 01:33:11.486   727   727 I zygote64: option[22]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[23]=-Xmx64m
05-15 01:33:11.486   727   727 I zygote64: option[24]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:11.486   727   727 I zygote64: option[26]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:11.486   727   727 I zygote64: option[28]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:11.486   727   727 I zygote64: option[30]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[31]=--runtime-arg
05-15 01:33:11.486   727   727 I zygote64: option[32]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[33]=-Xms64m
05-15 01:33:11.486   727   727 I zygote64: option[34]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[35]=--runtime-arg
05-15 01:33:11.486   727   727 I zygote64: option[36]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[37]=-Xmx512m
05-15 01:33:11.486   727   727 I zygote64: option[38]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[39]=-j4
05-15 01:33:11.486   727   727 I zygote64: option[40]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[41]=-j4
05-15 01:33:11.486   727   727 I zygote64: option[42]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[43]=--instruction-set-variant=generic
05-15 01:33:11.486   727   727 I zygote64: option[44]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[45]=--instruction-set-variant=generic
05-15 01:33:11.486   727   727 I zygote64: option[46]=-Ximage-compiler-option
05-15 01:33:11.486   727   727 I zygote64: option[47]=--instruction-set-features=default
05-15 01:33:11.486   727   727 I zygote64: option[48]=-Xcompiler-option
05-15 01:33:11.486   727   727 I zygote64: option[49]=--instruction-set-features=default
05-15 01:33:11.486   727   727 I zygote64: option[50]=-Duser.locale=en-US
05-15 01:33:11.486   727   727 I zygote64: option[51]=--cpu-abilist=arm64-v8a
05-15 01:33:11.486   727   727 I zygote64: option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:11.566   731   731 I cameraserver: ServiceManager: 0xf21979a0
05-15 01:33:11.566   731   731 I CameraService: CameraService started (pid=731)
05-15 01:33:11.572   731   731 I CameraService: CameraService process starting
05-15 01:33:11.572   731   731 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:11.572   731   731 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:11.581   793   793 D lhd     : OnIpcConnect
05-15 01:33:11.599   731   731 W cameraserver: type=1400 audit(0.0:119): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2092 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:11.599   731   731 W cameraserver: type=1400 audit(0.0:120): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2295 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:11.605   731   731 E vndksupport: Could not load /vendor/lib/hw/android.hardware.camera.provider@2.4-impl.so from sphal namespace: dlopen failed: library "android.hardware.camera.device@1.0.so" not found.
05-15 01:33:11.605   731   731 E /system/bin/cameraserver: Failed to dlopen android.hardware.camera.provider@2.4-impl.so: unknown error
05-15 01:33:11.613   794   823 D gpsd_d  : CustomerModule::ueventThreadProc uevent thread started
05-15 01:33:11.613   794   794 D gpsd_d  : Create : default BreadcrumbMaxLocsToStore = 280
05-15 01:33:11.613   794   794 D gpsd_d  : Create : default BreadcrumbWakeupDistance = 0
05-15 01:33:11.613   794   794 D         : gps client init!
05-15 01:33:11.662   730   730 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 30 lines
05-15 01:33:11.664   743   743 I /vendor/bin/hw/android.hardware.media.omx@1.0-service: mediacodecservice starting
05-15 01:33:11.664   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: Could not read additional policy file '/vendor/etc/seccomp_policy/mediacodec.policy'
05-15 01:33:11.664   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: allowing syscall: clock_gettime
05-15 01:33:11.665   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: allowing syscall: connect
05-15 01:33:11.665   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: allowing syscall: fcntl64
05-15 01:33:11.665   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: allowing syscall: socket
05-15 01:33:11.665   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: allowing syscall: writev
05-15 01:33:11.665   743   743 W /vendor/bin/hw/android.hardware.media.omx@1.0-service: libminijail[743]: logging seccomp filter failures
05-15 01:33:11.674   738   738 I chatty  : uid=1013(media) /system/bin/mediaserver expire 2 lines
05-15 01:33:11.679   743   743 W MediaCodecsXmlParser2: unable to open media codecs configuration xml file: /data/misc/media/media_codecs_profiling_results.xml
05-15 01:33:11.679   743   743 W MediaCodecsXmlParser2: parseTopLevelXMLFile(/data/misc/media/media_codecs_profiling_results.xml) failed
05-15 01:33:11.679   743   743 E MediaCodecsXmlParser2: Cannot find the role for a decoder of type video/mpeg
05-15 01:33:11.679   743   743 E MediaCodecsXmlParser2: Cannot find the role for a decoder of type video/x-pn-realvideo
05-15 01:33:11.679   743   743 E MediaCodecsXmlParser2: Cannot find the role for a decoder of type video/x-flv
05-15 01:33:11.679   743   743 E MediaCodecsXmlParser2: Cannot find the role for a decoder of type video/vc1
05-15 01:33:11.679   743   743 I ServiceManagement: Removing namespace from process name android.hardware.media.omx@1.0-service to omx@1.0-service.
05-15 01:33:11.688   743   743 I IMG-OMX : IMG_OMXLibWrapper library libomx_vxd.so mLibHandle:0xb8a38d05
05-15 01:33:11.689   743   743 D IMG-OMX : IMG_OMXLibWrapper 13 components in libomx_vxd.so
05-15 01:33:11.696   511   826 I chatty  : uid=1041(audioserver) HwBinder:511_1 expire 241 lines
05-15 01:33:11.709   743   743 I IMG-OMX : IMG_OMXLibWrapper library libomx_vxe.so mLibHandle:0x83cc5f1b
05-15 01:33:11.709   743   743 E IMGTOPAZ: OMX_Init done
05-15 01:33:11.709   743   743 D IMG-OMX : IMG_OMXLibWrapper 2 components in libomx_vxe.so
05-15 01:33:11.710   743   743 W AString : ctor got NULL, using empty string instead
05-15 01:33:11.710   743   743 W AString : ctor got NULL, using empty string instead
05-15 01:33:11.712   743   743 E MediaCodecsXmlParser: addTypeFromAttributes: updating non-existing type
05-15 01:33:11.712   743   743 W MediaCodecsXmlParser: unable to open media codecs configuration xml file: /data/misc/media/media_codecs_profiling_results.xml
05-15 01:33:11.712   743   743 I ServiceManagement: Removing namespace from process name android.hardware.media.omx@1.0-service to omx@1.0-service.
05-15 01:33:11.713   743   743 I /vendor/bin/hw/android.hardware.media.omx@1.0-service: Treble OMX service created.
05-15 01:33:11.751   503   503 I GRALLOC : 	 shrFd=10,fmt=0x21,intFmt=0x21,btStrd=6172,size=8192,pid=503 
05-15 01:33:11.751   503   503 I GRALLOC : 	 yuv=2,w=6172,h=1,Stride u=0 v=0,offset u=0 v=0 
05-15 01:33:11.751   503   503 I GRALLOC : 	 iova_size=8192,conUsg=0x2080000,proUsg=0x2080000,	 strd=6172,[afbc]HdrStrd=0 PyldStrd=0 Scrmbl=0,ionhnd = 1 
05-15 01:33:11.771   346   346 E         : pid 511, opration oeminfo_read OK
05-15 01:33:11.771   346   346 E         : 
05-15 01:33:11.773   511   851 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 1 line
05-15 01:33:11.859   746   838 I chatty  : uid=1013(media) OV8865_2L expire 3 lines
05-15 01:33:11.867   746   845 I chatty  : uid=1013(media) ispack expire 10 lines
05-15 01:33:11.869   788   788 D ril_rore: run RomDaemon
05-15 01:33:11.869   788   788 D ril_rore: run RomDaemon end.
05-15 01:33:11.869   788   875 D ril_rore: RomDaemon started.
05-15 01:33:11.897   788   873 D         : use /vendor/etc/cellular_cloud/version.txt[version=1.10.17.112] to replace []
05-15 01:33:11.897   746   840 I chatty  : uid=1013(media) IMX179 expire 26 lines
05-15 01:33:11.897   788   873 D         : use /vendor/etc/cellular_cloud[version=1.10.17.112] to replace []
05-15 01:33:11.914   788   873 D         : use /vendor/etc/cellular_cloud[version=1.10.17.112] to replace []
05-15 01:33:11.916   788   873 D         : use /vendor/etc/cellular_cloud[version=1.10.17.112] to replace []
05-15 01:33:11.922   728   728 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:11.959   728   728 I zygote  : option[0]=-Xzygote
05-15 01:33:11.959   728   728 I zygote  : option[1]=-Xusetombstonedtraces
05-15 01:33:11.959   728   728 I zygote  : option[2]=exit
05-15 01:33:11.959   728   728 I zygote  : option[3]=vfprintf
05-15 01:33:11.959   728   728 I zygote  : option[4]=sensitiveThread
05-15 01:33:11.959   728   728 I zygote  : option[5]=-verbose:gc
05-15 01:33:11.959   728   728 I zygote  : option[6]=-Xms8m
05-15 01:33:11.959   728   728 I zygote  : option[7]=-Xmx512m
05-15 01:33:11.959   728   728 I zygote  : option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:11.959   728   728 I zygote  : option[9]=-XX:HeapMinFree=2m
05-15 01:33:11.959   728   728 I zygote  : option[10]=-XX:HeapMaxFree=8m
05-15 01:33:11.959   728   728 I zygote  : option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:11.959   728   728 I zygote  : option[12]=-Xusejit:true
05-15 01:33:11.959   728   728 I zygote  : option[13]=-Xjitsaveprofilinginfo
05-15 01:33:11.959   728   728 I zygote  : option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:11.959   728   728 I zygote  : option[15]=-Xlockprofthreshold:500
05-15 01:33:11.959   728   728 I zygote  : option[16]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[17]=--runtime-arg
05-15 01:33:11.959   728   728 I zygote  : option[18]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[19]=-Xms64m
05-15 01:33:11.959   728   728 I zygote  : option[20]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[21]=--runtime-arg
05-15 01:33:11.959   728   728 I zygote  : option[22]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[23]=-Xmx64m
05-15 01:33:11.959   728   728 I zygote  : option[24]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:11.959   728   728 I zygote  : option[26]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:11.959   728   728 I zygote  : option[28]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:11.959   728   728 I zygote  : option[30]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[31]=--runtime-arg
05-15 01:33:11.959   728   728 I zygote  : option[32]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[33]=-Xms64m
05-15 01:33:11.959   728   728 I zygote  : option[34]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[35]=--runtime-arg
05-15 01:33:11.959   728   728 I zygote  : option[36]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[37]=-Xmx512m
05-15 01:33:11.959   728   728 I zygote  : option[38]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[39]=-j4
05-15 01:33:11.959   728   728 I zygote  : option[40]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[41]=-j4
05-15 01:33:11.959   728   728 I zygote  : option[42]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[43]=--instruction-set-variant=cortex-a15
05-15 01:33:11.959   728   728 I zygote  : option[44]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[45]=--instruction-set-variant=cortex-a15
05-15 01:33:11.959   728   728 I zygote  : option[46]=-Ximage-compiler-option
05-15 01:33:11.959   728   728 I zygote  : option[47]=--instruction-set-features=default
05-15 01:33:11.959   728   728 I zygote  : option[48]=-Xcompiler-option
05-15 01:33:11.959   728   728 I zygote  : option[49]=--instruction-set-features=default
05-15 01:33:11.959   728   728 I zygote  : option[50]=-Duser.locale=en-US
05-15 01:33:11.959   728   728 I zygote  : option[51]=--cpu-abilist=armeabi-v7a,armeabi
05-15 01:33:11.959   728   728 I zygote  : option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:12.006   746   842 I chatty  : uid=1013(media) IMX286DUAL expire 31 lines
05-15 01:33:12.178   759   759 I fpc_fingerprint_hal: fingeprint module open ok!
05-15 01:33:12.179   759   887 D fpc_fingerprint_hal: worker idle
05-15 01:33:12.179   759   888 E fpc_fingerprint_hal: ldh unlink socket fail, errno=30
05-15 01:33:12.179   759   888 D fpc_fingerprint_hal: ldh run_socket_server() create listen socket OK!fpsensor_socket 9
05-15 01:33:12.228   740   763 I ServiceManager: Waiting for service package_native...
05-15 01:33:12.257   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:12.376   759   759 E fpc_fingerprint_hal: default  dev->sensor_calibration_status  = -1
05-15 01:33:12.376   759   759 D fpc_fingerprint_hal: dev->sensor_calibration_status  = -1
05-15 01:33:12.376   759   759 E fpc_fingerprint_hal: current calibration status = -1
05-15 01:33:12.384   759   759 I fpc_fingerprint_hal: testhub dir path = /data/log/fingerprint, len = 21
05-15 01:33:12.395   759   759 I fpc_fingerprint_hal: testhub dir path = /splash2/log/fingerprint, len = 24
05-15 01:33:12.398   759   759 E fpc_fingerprint_hal: check_file_exists, /data/log/fingerprint/fp_stats_tmp open erro, seems not exists
05-15 01:33:12.398   759   759 E fpc_fingerprint_hal: /data/log/fingerprint/fp_stats_tmp not exist, set to default
05-15 01:33:12.398   759   759 E fpc_fingerprint_hal: check_file_exists, /data/log/fingerprint/fp_stats_all open erro, seems not exists
05-15 01:33:12.398   759   759 E fpc_fingerprint_hal: /data/log/fingerprint/fp_stats_all not exist, set to default
05-15 01:33:12.401   759   759 D fpc_fingerprint_hal: /splash2/log/fingerprint/fp_stats_all exist read values from file
05-15 01:33:12.403   759   759 E fpc_fingerprint_hal: check_file_exists, /splash2/log/fingerprint/fp_key_paras open erro, seems not exists
05-15 01:33:12.403   759   759 D fpc_fingerprint_hal: /splash2/log/fingerprint/fp_key_paras not exist, set to default
05-15 01:33:12.403   759   759 D fpc_fingerprint_hal: SNR = 0, SNRSINGAL = 0
05-15 01:33:12.404   759   759 E fpc_fingerprint_hal: fp_get_dts_config_value: invalid path /proc/device-tree/fingerprint/fingerprint,enroll_fp_tp_anti.
05-15 01:33:12.404   759   759 D fpc_fingerprint_hal: fpc_set_notify_impl
05-15 01:33:12.404   759   759 D fpc_fingerprint_hal: fido_set_authenticate_cb_impl
05-15 01:33:12.414   759   887 D fpc_fingerprint_hal: worker idle
05-15 01:33:12.414   759   759 I vendor.huawei.hardware.biometrics.fingerprint@2.1-service: set fido call back
05-15 01:33:12.415   759   759 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.biometrics.fingerprint@2.1-service to fingerprint@2.1.
05-15 01:33:12.425   759   887 D fpc_fingerprint_hal: worker idle
05-15 01:33:12.691   727   727 D Zygote  : begin preload
05-15 01:33:12.691   727   727 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:12.691   727   727 I Zygote  : Preloading ICU data...
05-15 01:33:12.804   727   727 D Zygote64Timing: BeginIcuCachePinning took to complete: 113ms
05-15 01:33:12.804   727   727 I Zygote  : Preloading classes...
05-15 01:33:12.852   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:12.852   346   346 E         : 
05-15 01:33:12.856   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:12.856   346   346 E         : 
05-15 01:33:12.862   511   901 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 4 lines
05-15 01:33:12.862   511   902 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 4 lines
05-15 01:33:12.863   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 216 lines
05-15 01:33:12.870   746   852 I chatty  : uid=1013(media) laser expire 5 lines
05-15 01:33:12.900   730   906 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 3 lines
05-15 01:33:12.907   730   908 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:12.908   730   911 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:12.908   730   913 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:12.994   730   917 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:13.033   728   728 I zygote  : Explicit concurrent copying GC freed 186(8KB) AllocSpace objects, 0(0B) LOS objects, 99% free, 23KB/6MB, paused 36us total 3.735ms
05-15 01:33:13.037   728   728 I zygote  : Explicit concurrent copying GC freed 9(32KB) AllocSpace objects, 0(0B) LOS objects, 99% free, 22KB/6MB, paused 21us total 2.480ms
05-15 01:33:13.037   728   728 D Zygote32Timing: PostZygoteInitGC took to complete: 8ms
05-15 01:33:13.037   728   728 D Zygote32Timing: ZygoteInit took to complete: 10ms
05-15 01:33:13.082   728   728 I zygote  : Global filter of size 170 installed
05-15 01:33:13.082   728   728 I Zygote  : Accepting command socket connections
05-15 01:33:13.107   788   861 D         : use /vendor/etc/cellular_cloud/version.txt[version=1.10.17.112] to replace []
05-15 01:33:13.107   788   861 D         : use /vendor/etc/cellular_cloud[version=1.10.17.112] to replace []
05-15 01:33:13.108   788   861 I chatty  : uid=0(root) balong_modem0 identical 1 line
05-15 01:33:13.110   788   861 D         : use /vendor/etc/cellular_cloud[version=1.10.17.112] to replace []
05-15 01:33:13.228   740   763 I ServiceManager: Waiting for service package_native...
05-15 01:33:13.229   727   727 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:13.253   727   727 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:13.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:13.271   727   727 I zygote64: Thread[1,tid=727,Native,Thread*=0x7a06abfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:13.271   727   727 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:13.272   727   727 I zygote64: Thread[1,tid=727,Native,Thread*=0x7a06abfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:13.272   727   727 I zygote64: Thread[1,tid=727,Native,Thread*=0x7a06abfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:13.357   727   727 I Zygote  : ...preloaded 4715 classes in 553ms.
05-15 01:33:13.357   727   727 I zygote64: VMRuntime.preloadDexCaches starting
05-15 01:33:13.393   727   727 I zygote64: VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:13.393   727   727 I zygote64: VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:13.393   727   727 I zygote64: VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:13.393   727   727 I zygote64: VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:13.393   727   727 I zygote64: VMRuntime.preloadDexCaches finished
05-15 01:33:13.393   727   727 D Zygote64Timing: PreloadClasses took to complete: 589ms
05-15 01:33:13.534   727   727 I Zygote  : Preloading resources...
05-15 01:33:13.548   727   727 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:13.557   727   727 I Zygote  : ...preloaded 64 resources in 23ms.
05-15 01:33:13.559   727   727 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:13.560   727   727 I Zygote  : ...preloaded 41 resources in 3ms.
05-15 01:33:13.560   727   727 D Zygote64Timing: PreloadResources took to complete: 167ms
05-15 01:33:13.576   727   727 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:13.585   727   727 I Zygote  : Preloading shared libraries...
05-15 01:33:13.599   727   727 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:13.601   727   727 I Zygote  : Installed AndroidKeyStoreProvider in 2ms.
05-15 01:33:13.605   727   727 I Zygote  : Warmed up JCA providers in 4ms.
05-15 01:33:13.605   727   727 D Zygote  : end preload
05-15 01:33:13.605   727   727 D Zygote64Timing: ZygotePreload took to complete: 914ms
05-15 01:33:13.616   727   727 I zygote64: Explicit concurrent copying GC freed 29303(2MB) AllocSpace objects, 25(476KB) LOS objects, 80% free, 1524KB/7MB, paused 31us total 10.872ms
05-15 01:33:13.624   727   727 I zygote64: Explicit concurrent copying GC freed 5435(198KB) AllocSpace objects, 0(0B) LOS objects, 81% free, 1357KB/7MB, paused 21us total 6.009ms
05-15 01:33:13.624   727   727 D Zygote64Timing: PostZygoteInitGC took to complete: 19ms
05-15 01:33:13.624   727   727 D Zygote64Timing: ZygoteInit took to complete: 935ms
05-15 01:33:13.682   727   727 I zygote64: Global filter of size 170 installed
05-15 01:33:13.708   727   727 I Zygote  : System server process 922 has been created
05-15 01:33:13.708   727   727 E Zygote  : couldn't write 922 to /dev/memcg/system/tasks
05-15 01:33:13.709   727   727 I Zygote  : Accepting command socket connections
05-15 01:33:13.727   922   922 I chatty  : uid=1000 system_server expire 145 lines
05-15 01:33:13.788   922   922 I SystemServer: InitBeforeStartServices
05-15 01:33:13.790   922   922 I SystemServer: Entered the Android system server!
05-15 01:33:13.929   733   733 W Binder:733_1: type=1400 audit(0.0:122): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:13.929   733   733 W Binder:733_1: type=1400 audit(0.0:123): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:13.934   922   922 D SystemServerTiming: InitBeforeStartServices took to complete: 146ms
05-15 01:33:13.934   922   922 I SystemServer: StartServices
05-15 01:33:13.934   922   922 I SystemServer: Reading configuration...
05-15 01:33:13.934   922   922 I SystemServer: ReadingSystemConfig
05-15 01:33:13.935   922   922 D SystemServerTiming: ReadingSystemConfig took to complete: 0ms
05-15 01:33:13.935   922   922 I SystemServer: StartInstaller
05-15 01:33:13.935   922   922 I SystemServiceManager: Starting com.android.server.pm.Installer
05-15 01:33:13.935   922   935 D SystemServerInitThreadPool: Started executing ReadingSystemConfig
05-15 01:33:13.938   922   922 D SystemServerTiming: StartInstaller took to complete: 4ms
05-15 01:33:13.938   922   922 I SystemServer: DeviceIdentifiersPolicyService
05-15 01:33:13.938   922   922 I SystemServiceManager: Starting com.android.server.os.DeviceIdentifiersPolicyService
05-15 01:33:13.939   922   922 D SystemServerTiming: DeviceIdentifiersPolicyService took to complete: 1ms
05-15 01:33:13.939   922   922 I SystemServer: StartActivityManager
05-15 01:33:13.939   922   922 I SystemServiceManager: Starting com.android.server.am.ActivityManagerService$Lifecycle
05-15 01:33:13.962   922   922 I ActivityManager: Memory class: 384
05-15 01:33:13.962   922   937 I ServiceThread: Enabled StrictMode logging for ActivityManager looper.
05-15 01:33:13.963   922   938 I ServiceThread: Enabled StrictMode logging for android.ui looper.
05-15 01:33:13.973   922   935 D SystemServerInitThreadPool: Finished executing ReadingSystemConfig
05-15 01:33:13.979   922   922 D BatteryStatsImpl: Reading daily items from /data/system/batterystats-daily.xml
05-15 01:33:13.982   922   940 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:13.986   922   940 E BatteryExternalStatsWorker: no controller energy info supplied for telephony
05-15 01:33:13.988   922   940 E KernelUidCpuFreqTimeReader: Failed to read /proc/uid_time_in_state: java.io.FileNotFoundException: /proc/uid_time_in_state (No such file or directory)
05-15 01:33:14.023   922   922 I AppOps  : No existing app ops /data/system/appops.xml; starting empty
05-15 01:33:14.030   942   942 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:14.030   941   941 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:14.031   941   941 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:14.031   941   941 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:14.031   941   941 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:14.032   922   922 I IntentFirewall: Read new rules (A:0 B:0 S:0)
05-15 01:33:14.033   942   942 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:14.034   942   942 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:14.034   922   947 I ServiceThread: Enabled StrictMode logging for android.display looper.
05-15 01:33:14.039   922   922 D AppOps  : AppOpsService published
05-15 01:33:14.040   922   922 D SystemServerTiming: StartActivityManager took to complete: 100ms
05-15 01:33:14.040   922   922 I SystemServer: StartPowerManager
05-15 01:33:14.040   922   922 I SystemServiceManager: Starting com.android.server.power.PowerManagerService
05-15 01:33:14.044   922   949 I ServiceThread: Enabled StrictMode logging for PowerManagerService looper.
05-15 01:33:14.049   922   922 D SystemServerTiming: StartPowerManager took to complete: 10ms
05-15 01:33:14.050   922   922 I SystemServer: InitPowerManagement
05-15 01:33:14.052   922   922 D SystemServerTiming: InitPowerManagement took to complete: 3ms
05-15 01:33:14.052   922   922 I SystemServer: StartRecoverySystemService
05-15 01:33:14.052   922   922 I SystemServiceManager: Starting com.android.server.RecoverySystemService
05-15 01:33:14.053   922   922 D SystemServerTiming: StartRecoverySystemService took to complete: 1ms
05-15 01:33:14.053   922   922 V RescueParty: Disabled because of active USB connection
05-15 01:33:14.053   922   922 I SystemServer: StartLightsService
05-15 01:33:14.053   922   922 I SystemServiceManager: Starting com.android.server.lights.LightsService
05-15 01:33:14.054   922   922 D SystemServerTiming: StartLightsService took to complete: 0ms
05-15 01:33:14.054   922   922 I SystemServer: StartDisplayManager
05-15 01:33:14.054   922   922 I SystemServiceManager: Starting com.android.server.display.DisplayManagerService
05-15 01:33:14.055   922   922 D SystemServerTiming: StartDisplayManager took to complete: 2ms
05-15 01:33:14.055   922   922 I SystemServer: WaitForDisplay
05-15 01:33:14.055   922   922 I SystemServiceManager: Starting phase 100
05-15 01:33:14.060   922   947 I DisplayManagerService: Display device added: DisplayDeviceInfo{"Built-in Screen": uniqueId="local:0", 1080 x 1920, modeId 1, defaultModeId 1, supportedModes [{id=1, width=1080, height=1920, fps=60.000004}], colorMode 0, supportedColorModes [0], HdrCapabilities android.view.Display$HdrCapabilities@1d6308, density 480, 365.76 x 366.676 dpi, appVsyncOff 2000000, presDeadline 13666666, touch INTERNAL, rotation 0, type BUILT_IN, state UNKNOWN, FLAG_DEFAULT_DISPLAY, FLAG_ROTATES_WITH_CONTENT, FLAG_SECURE, FLAG_SUPPORTS_PROTECTED_BUFFERS}
05-15 01:33:14.060   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:14.063   922   922 D SystemServerTiming: WaitForDisplay took to complete: 8ms
05-15 01:33:14.063   922   947 I DisplayManagerService: Display device changed state: "Built-in Screen", ON
05-15 01:33:14.063   922   922 I SystemServer: StartPackageManagerService
05-15 01:33:14.081   922   922 D SELinuxMMAC: Using policy file /system/etc/selinux/plat_mac_permissions.xml
05-15 01:33:14.083   922   922 D SELinuxMMAC: Using policy file /vendor/etc/selinux/nonplat_mac_permissions.xml
05-15 01:33:14.125   922   922 W PackageManager: Failed to parse /system/framework/arm64: Missing base APK in /system/framework/arm64
05-15 01:33:14.126   922   922 W PackageManager: Failed to parse /system/framework/oat: Missing base APK in /system/framework/oat
05-15 01:33:14.126   922   922 W PackageManager: Failed to parse /system/framework/arm: Missing base APK in /system/framework/arm
05-15 01:33:14.177   746   853 I chatty  : uid=1013(media) depthisp expire 1 line
05-15 01:33:14.182   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.182   346   346 E         : 
05-15 01:33:14.182   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.182   346   346 E         : 
05-15 01:33:14.190   746   965 I chatty  : uid=1013(media) HwaCameraMonito expire 1 line
05-15 01:33:14.215   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.215   346   346 E         : 
05-15 01:33:14.215   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.215   346   346 E         : 
05-15 01:33:14.216   922   922 I PackageManager: Finished scanning system apps. Time: 95 ms, packageCount: 94 , timePerPackage: 1 , cached: 94
05-15 01:33:14.217   922   922 I PackageManager: Finished scanning non-system apps. Time: 1 ms, packageCount: 0 , timePerPackage: 0 , cached: 0
05-15 01:33:14.220   922   922 I PackageManager: Time to scan packages: 0.099 seconds
05-15 01:33:14.221   922   922 V PackageManager: reconcileAppsData for null u0 0x3 migrateAppData=true
05-15 01:33:14.225   733   760 I SELinux : SELinux: Loaded file_contexts
05-15 01:33:14.226   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.226   346   346 E         : 
05-15 01:33:14.226   346   346 E         : pid 746, opration nvm_read OK
05-15 01:33:14.226   346   346 E         : 
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(640) ,h(480),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(320) ,h(240),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(1280) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(1920) ,h(1080),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(3264) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(2448) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(3264) ,h(1840),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_BLOB:kAvailableFormats = 33,w(1536) ,h(864),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(3264) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(2448) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(3264) ,h(1840),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(1920) ,h(1080),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(1440) ,h(1080),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(1536) ,h(864),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(1280) ,h(960),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(1280) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(960) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(720) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(640) ,h(480),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(320) ,h(240),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(352) ,h(288),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(208) ,h(144),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_IMPLEMENTATION_DEFINED:kAvailableFormats = 34,w(176) ,h(144),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(3264) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(2448) ,h(2448),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(3264) ,h(1840),minduartion(50000000)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(1920) ,h(1080),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(1440) ,h(1080),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(1536) ,h(864),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(1280) ,h(960),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(1280) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(960) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(720) ,h(720),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(640) ,h(480),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(320) ,h(240),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(352) ,h(288),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(208) ,h(144),minduartion(33331760)
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability:HAL_PIXEL_FORMAT_YCBCR_420_888:kAvailableFormats = 35,w(176) ,h(144),minduartion(33331760)
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability, Active Array [0] = 0
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability, Active Array [1] = 0
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability, Active Array [2] = 3264
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability, Active Array [3] = 2448
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability fix scene AE mode .
05-15 01:33:14.227   746   746 I HispManager: queryApi2Capability fix scene AF mode .
05-15 01:33:14.227   746   746 D HispManager: queryApi2Capability(1970): instance[0x7d46277fc0] depthPreview(0) depthCapture(0), size(0). 
05-15 01:33:14.227   746   746 D AlgoFilterStage: [HWA_CAM3]STAGELIFECTRL enter getAndCreatePluginOrCreateOne(), pipeline id=3
05-15 01:33:14.227   746   746 D IppAlgo : [HWA_CAM3]ipp=StatIpp KEY_CA_CAM3 PREV exit IppAlgo this=0x7d462e0490
05-15 01:33:14.227   746   746 D IppFrameAllocatorImpl: [HWA_CAM3]this=0x7d462e04d0, enter IppFrameAllocatorImpl()
05-15 01:33:14.227   746   746 D IppAlgo : [HWA_CAM3]ipp=PostIpp KEY_CA_CAM3 PREV exit IppAlgo this=0x7d462e07a0
05-15 01:33:14.227   746   746 D IppFrameAllocatorImpl: [HWA_CAM3]this=0x7d462e07e0, enter IppFrameAllocatorImpl()
05-15 01:33:14.227   746   746 D PpFrameCallbackImpl: [HWA_CAM3]enter PpFrameCallbackImpl()
05-15 01:33:14.227   746   746 D PpMemStatListenerImpl: [HWA_CAM3]enter PpMemStatListenerImpl()
05-15 01:33:14.227   746   746 D PpAlgo  : [HWA_CAM3]algo=PostPp post=1 KEY_CA_CAM3 SNAP enter PpAlgo
05-15 01:33:14.227   746   746 D PpFrameCallbackImpl: [HWA_CAM3]enter PpFrameCallbackImpl()
05-15 01:33:14.227   746   746 D PpMemStatListenerImpl: [HWA_CAM3]enter PpMemStatListenerImpl()
05-15 01:33:14.227   746   746 D PpAlgo  : [HWA_CAM3]algo=ForePp post=0 KEY_CA_CAM3 SNAP enter PpAlgo
05-15 01:33:14.227   746   746 D AlgoFilterManager: [HWA_CAM3]STAGELIFECTRL enter AlgoFilterManager(), mPipeLineId=3
05-15 01:33:14.227   746   746 D AlgoFilterManager: [HWA_CAM3]initAlgoDevice() Isp Info = 2
05-15 01:33:14.227   746   746 D AlgoFilterManager: [HWA_CAM3]KEY_CA_CAM3 enter create, mPipeLineId=3, mIsPlugInCreated=0
05-15 01:33:14.227   746   746 D HwaCore : [aaf4016_64D] enter newHwaPlugin()
05-15 01:33:14.227   746   746 D HwaCore : [aaf4016_64D] enter HwaCore(), HwaCore=0x7d4623d840
05-15 01:33:14.227   746   746 I HwaCameraMonitor: [aaf4016_64I] enter newMonitor()
05-15 01:33:14.227   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.227   746   746 I         : , len = 6
05-15 01:33:14.227   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.227   746   746 D HwaCore : [aaf4016_64D] enter initialize(), HwaCore=0x7d4623d840
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV this=0x7d462fe200, ipptype=0, enter HwaIppPluginImpl()
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: LOG START
05-15 01:33:14.228   746   746 D SdkDepthIppAlgo: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SdkDepthIppAlgo, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FaceDetection, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SceneDetection, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoStabilization, type=258, synctype=1, cbcount=1 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoStabMph, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VidHance, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=TargetTracking, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=MirrorDenoise, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SmartAE, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FrontBokehAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DocVFaceBeauty, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FaceSmooth, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=Mono, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=IppAlgoDM, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.228   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.228   746   746 I         : , len = 6
05-15 01:33:14.228   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.228   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ColorEffect, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DualCamAlgo, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaDMapIpp, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=BigApertureAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=hwa_af, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DebugAeAwb, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   740   763 I ServiceManager: Waiting for service package_native...
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=Misc, type=0, synctype=0, cbcount=2 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=BShutterTryAE, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaAe, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 D NiceFoodIppAlgo: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=NiceFoodIppAlgo, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaFlash, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 D AssistAF: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=AssistAF, type=0, synctype=0, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 D ContrastCalculate: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ContrastCalculate, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ContrastCalculateGyro, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DepthSelfLearnAlgo, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.229   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwBeautyIpp, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.229   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.229   746   746 I         : , len = 6
05-15 01:33:14.229   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=MakeUpIppAlgo, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoBokehAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoBokehDspAlgo, type=258, synctype=1, cbcount=1 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=LaserMgr, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=IspEnhncAlgo, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.230   746   746 D OisMgr  : [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=OisMgr, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: LOG END
05-15 01:33:14.230   746   746 I HwaRuntimeMonitorManager: [aaf4016_64I] enter HwaRuntimeMonitorManager() mMonitorType = IPP_stat, this = 0x7d462f46a0
05-15 01:33:14.230   746   746 I HwaCameraMonitor: [aaf4016_64I] enter registerMoniterImpl()
05-15 01:33:14.230   746   746 I HwaCameraMonitor: [aaf4016_64I] exit registerMoniterImpl() add 0x7d462f46a0 to list, list size = 9
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV this=0x7d462ff000, ipptype=256, enter HwaIppPluginImpl()
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: LOG START
05-15 01:33:14.230   746   746 D SdkDepthIppAlgo: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SdkDepthIppAlgo, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FaceDetection, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SceneDetection, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoStabilization, type=258, synctype=1, cbcount=1 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoStabMph, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VidHance, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=TargetTracking, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=MirrorDenoise, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.230   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.230   746   746 I         : , len = 6
05-15 01:33:14.230   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.230   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=SmartAE, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FrontBokehAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DocVFaceBeauty, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=FaceSmooth, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=Mono, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=IppAlgoDM, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ColorEffect, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DualCamAlgo, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaDMapIpp, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=BigApertureAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=hwa_af, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DebugAeAwb, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=Misc, type=0, synctype=0, cbcount=2 is loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=BShutterTryAE, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaAe, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.231   746   746 D NiceFoodIppAlgo: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.231   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.231   746   746 I         : , len = 6
05-15 01:33:14.231   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.231   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=NiceFoodIppAlgo, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwaFlash, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.232   746   746 D AssistAF: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=AssistAF, type=0, synctype=0, cbcount=0 is loaded.
05-15 01:33:14.232   746   746 D ContrastCalculate: [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ContrastCalculate, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=ContrastCalculateGyro, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=DepthSelfLearnAlgo, type=0, synctype=0, cbcount=1 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=HwBeautyIpp, type=257, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=MakeUpIppAlgo, type=257, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoBokehAlgo, type=258, synctype=1, cbcount=1 is not loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=VideoBokehDspAlgo, type=258, synctype=1, cbcount=1 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=LaserMgr, type=0, synctype=1, cbcount=0 is loaded.
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=IspEnhncAlgo, type=0, synctype=0, cbcount=0 is not loaded.
05-15 01:33:14.232   746   746 D OisMgr  : [aaf4016_64D] enter checkIppalgo()
05-15 01:33:14.232   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.232   746   746 I         : , len = 6
05-15 01:33:14.232   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: algo name=OisMgr, type=0, synctype=1, cbcount=0 is not loaded.
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] KEY_CA_ALGO PREV mIppAlgoInfos: LOG END
05-15 01:33:14.232   746   746 I HwaRuntimeMonitorManager: [aaf4016_64I] enter HwaRuntimeMonitorManager() mMonitorType = IPP_post, this = 0x7d462f46e0
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] enter registerMoniterImpl()
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] exit registerMoniterImpl() add 0x7d462f46e0 to list, list size = 10
05-15 01:33:14.232   746   746 D HwaPpPluginImpl: [aaf4016_64D] SNAP ALGO enter HwaPpPluginImpl
05-15 01:33:14.232   746   746 I HwaRuntimeMonitorManager: [aaf4016_64I] enter HwaRuntimeMonitorManager() mMonitorType = PP_background, this = 0x7d462f4720
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] enter registerMoniterImpl()
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] exit registerMoniterImpl() add 0x7d462f4720 to list, list size = 11
05-15 01:33:14.232   746   746 D HwaPpPluginImpl: [aaf4016_64D] SNAP ALGO enter HwaPpPluginImpl
05-15 01:33:14.232   746   746 I HwaRuntimeMonitorManager: [aaf4016_64I] enter HwaRuntimeMonitorManager() mMonitorType = PP_foreground, this = 0x7d462f4760
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] enter registerMoniterImpl()
05-15 01:33:14.232   746   746 I HwaCameraMonitor: [aaf4016_64I] exit registerMoniterImpl() add 0x7d462f4760 to list, list size = 12
05-15 01:33:14.232   746   746 D IppAlgoPortIn: [HWA_CAM3]this=0x7d46311880, enter IppAlgoPortIn()
05-15 01:33:14.232   746   746 D IppAlgoPortOut: [HWA_CAM3]this=0x7d46311aa8, enter IppAlgoPortOut()
05-15 01:33:14.232   746   746 D IppAlgoPortOut: [HWA_CAM3]this=0x7d46311c78, enter IppAlgoPortOut()
05-15 01:33:14.232   746   746 D IppAlgoFilter: [HWA_CAM3]FRMC_ this=0x7d46311800, ipptype=0, enter IppAlgoFilter()
05-15 01:33:14.232   746   746 D IppAlgo : [HWA_CAM3]ipp=StatIpp KEY_CA_CAM3 PREV enter create this=0x7d462e0490
05-15 01:33:14.232   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, enter create()
05-15 01:33:14.233   746   746 I HwaStatInfo: [aaf4016_64I] enter initialize()
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SdkDepthIppAlgo, type=257, synctype=1, cbcount=0 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 D FaceDetection: [aaf4016_64D] enter FaceDetection()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: FaceDetection
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created FaceDetection
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: FaceDetection
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: FaceDetection
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=FaceDetection, type=0, synctype=0, cbcount=1 is created.
05-15 01:33:14.233   746   746 D SceneDetection: [aaf4016_64D] enter SceneDetection()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: SceneDetection
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created SceneDetection
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: SceneDetection
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: SceneDetection
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SceneDetection, type=0, synctype=0, cbcount=1 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=VideoStabilization, type=258, synctype=1, cbcount=1 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 D TargetTracking: [aaf4016_64D] enter TargetTracking()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: TargetTracking
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created TargetTracking
05-15 01:33:14.233   746   746 D TargetTracking: [aaf4016_64D] enter getSyncType(), result=0
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: TargetTracking
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: TargetTracking
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=TargetTracking, type=0, synctype=0, cbcount=1 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=MirrorDenoise, type=257, synctype=1, cbcount=0 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 I DLibLoader: [aaf4016_64I] enter DLibLoader(), soName=libSmartAE.so
05-15 01:33:14.233   746   746 D SmartAEDLibLoader: [aaf4016_64D] enter SmartAEDLibLoader()
05-15 01:33:14.233   746   746 D SmartAEDLibLoader: [aaf4016_64D] enter setFunsToDefault()
05-15 01:33:14.233   746   746 D IppAlgoSmartAE: [aaf4016_64D] enter IppAlgoSmartAE()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: SmartAE
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created SmartAE
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SmartAE, type=0, synctype=1, cbcount=0 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=ColorEffect, type=257, synctype=1, cbcount=0 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 I DualCamAlgo: [aaf4016_64I] enter DualCamAlgo()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: DualCamAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created DualCamAlgo
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: DualCamAlgo
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: DualCamAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=DualCamAlgo, type=0, synctype=0, cbcount=1 is created.
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: Misc
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created Misc
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: Misc
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: Misc
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=Misc, type=0, synctype=0, cbcount=2 is created.
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: BShutterTryAE
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created BShutterTryAE
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=BShutterTryAE, type=0, synctype=1, cbcount=0 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=NiceFoodIppAlgo, type=257, synctype=1, cbcount=0 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 D AssistAF: [aaf4016_64D] enter newIppalgo()
05-15 01:33:14.233   746   746 D AssistAF: [aaf4016_64D] enter AssistAF()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: AssistAF
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created AssistAF
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: AssistAF
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: AssistAF
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=AssistAF, type=0, synctype=0, cbcount=0 is created.
05-15 01:33:14.233   746   746 D ContrastCalculate: [aaf4016_64D] enter newIppalgo()
05-15 01:33:14.233   746   746 D ContrastCalculate: [aaf4016_64D] enter ContrastCalculate()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: ContrastCalculate
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created ContrastCalculate
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=ContrastCalculate, type=0, synctype=1, cbcount=0 is created.
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: DepthSelfLearnAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created DepthSelfLearnAlgo
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter HwaIppAlgoExeThread(), algo name: DepthSelfLearnAlgo
05-15 01:33:14.233   746   746 D HwaIppAlgoExeThread: [aaf4016_64D] enter create(), algo name: DepthSelfLearnAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=DepthSelfLearnAlgo, type=0, synctype=0, cbcount=1 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=HwBeautyIpp, type=257, synctype=1, cbcount=0 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=VideoBokehDspAlgo, type=258, synctype=1, cbcount=1 is not created for type is not compared mType=0x0.
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: LaserMgr
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created LaserMgr
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=LaserMgr, type=0, synctype=1, cbcount=0 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, exit  create()
05-15 01:33:14.233   746   746 D IppAlgo : [HWA_CAM3]ipp=StatIpp KEY_CA_CAM3 PREV exit create this=0x7d462e0490
05-15 01:33:14.233   746   746 D IppAlgoPortIn: [HWA_CAM3]this=0x7d46313080, enter IppAlgoPortIn()
05-15 01:33:14.233   746   746 D IppAlgoPortOut: [HWA_CAM3]this=0x7d463132a8, enter IppAlgoPortOut()
05-15 01:33:14.233   746   746 D IppAlgoPortOut: [HWA_CAM3]this=0x7d46313478, enter IppAlgoPortOut()
05-15 01:33:14.233   746   746 D IppAlgoFilter: [HWA_CAM3]FRMC_ this=0x7d46313000, ipptype=256, enter IppAlgoFilter()
05-15 01:33:14.233   746   746 D IppAlgo : [HWA_CAM3]ipp=PostIpp KEY_CA_CAM3 PREV enter create this=0x7d462e07a0
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, enter create()
05-15 01:33:14.233   746   746 D SdkDepthIppAlgo: [aaf4016_64D] enter newIppalgo()
05-15 01:33:14.233   746   746 D SdkDepthIppAlgo: [aaf4016_64D] enter SdkDepthIppAlgo()
05-15 01:33:14.233   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: SdkDepthIppAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created SdkDepthIppAlgo
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SdkDepthIppAlgo, type=257, synctype=1, cbcount=0 is created.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=FaceDetection, type=0, synctype=0, cbcount=1 is not created for type is not compared mType=0x100.
05-15 01:33:14.233   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SceneDetection, type=0, synctype=0, cbcount=1 is not created for type is not compared mType=0x100.
05-15 01:33:14.233   746   746 D VideoStabilization: [aaf4016_64D] enter VideoStabilization()
05-15 01:33:14.233   746   746 V HwaUtils: [aaf4016_64V] Custom Parameter[NEED_ENLARGE_INPUT_FRAME] = 100
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: VideoStabilization
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created VideoStabilization
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=VideoStabilization, type=258, synctype=1, cbcount=1 is created.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=TargetTracking, type=0, synctype=0, cbcount=1 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D MirrorDenoise: [aaf4016_64D] enter MirrorDenoise()
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: MirrorDenoise
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created MirrorDenoise
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=MirrorDenoise, type=257, synctype=1, cbcount=0 is created.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=SmartAE, type=0, synctype=1, cbcount=0 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D ColorEffect: [aaf4016_64D] enter ColorEffect()
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: ColorEffect
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created ColorEffect
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=ColorEffect, type=257, synctype=1, cbcount=0 is created.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=DualCamAlgo, type=0, synctype=0, cbcount=1 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=Misc, type=0, synctype=0, cbcount=2 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=BShutterTryAE, type=0, synctype=1, cbcount=0 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D NiceFoodIppAlgo: [aaf4016_64D] enter newIppalgo()
05-15 01:33:14.234   746   746 D NiceFoodIppAlgo: [aaf4016_64D] enter NiceFoodIppAlgo()
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: NiceFoodIppAlgo
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created NiceFoodIppAlgo
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=NiceFoodIppAlgo, type=257, synctype=1, cbcount=0 is created.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=AssistAF, type=0, synctype=0, cbcount=0 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=ContrastCalculate, type=0, synctype=1, cbcount=0 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=DepthSelfLearnAlgo, type=0, synctype=0, cbcount=1 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwBeautyIpp: [aaf4016_64D] enter HwBeautyIpp()
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: HwBeautyIpp
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created HwBeautyIpp
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=HwBeautyIpp, type=257, synctype=1, cbcount=0 is created.
05-15 01:33:14.234   746   746 D HwaIppAlgoExecutor: [aaf4016_64D] enter HwaIppAlgoExecutor(), algo name: VideoBokehDspAlgo
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] enter create(), algo is created VideoBokehDspAlgo
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=VideoBokehDspAlgo, type=258, synctype=1, cbcount=1 is created.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] mIppAlgoInfos: algo name=LaserMgr, type=0, synctype=1, cbcount=0 is not created for type is not compared mType=0x100.
05-15 01:33:14.234   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, exit  create()
05-15 01:33:14.234   746   746 D IppAlgo : [HWA_CAM3]ipp=PostIpp KEY_CA_CAM3 PREV exit create this=0x7d462e07a0
05-15 01:33:14.234   746   746 D PpAlgoFilter: [HWA_CAM3]algo=PostPp post=1 KEY_CA_CAM3 SNAP enter PpAlgoFilter(): 0x7d462bde00 
05-15 01:33:14.234   746   746 D PpAlgo  : [HWA_CAM3]algo=PostPp KEY_CA_CAM3 SNAP enter create
05-15 01:33:14.234   746   746 D HwaPpPluginImpl: [aaf4016_64D] SNAP ALGO enter create env: 0x7d462df910, eventCallback: 0x7d462e0828, device: 0x7d46295440, framecallback: 0x7d462e0aa0
05-15 01:33:14.234   746   746 D PPAlgoConfig: [aaf4016_64D] enter PPAlgoConfig()
05-15 01:33:14.234   746   746 D PPAlgoConfig: [aaf4016_64D] enter loadPPConfig()
05-15 01:33:14.234   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.234   746   746 I         : , len = 6
05-15 01:33:14.234   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.234   746   746 I PPAlgoConfig: [aaf4016_64I] [huawei_memory]loadPPConfig() curRamSize=4194304
05-15 01:33:14.234   746   746 I HwaUtils: [aaf4016_64I] getOneCfgFile() path=/odm/etc/camera/ppconfig.xml
05-15 01:33:14.234   746   746 D PPAlgoConfig: [aaf4016_64D] enter loadConfig()
05-15 01:33:14.234   746   746 I PPAlgoConfig: [aaf4016_64I] [huawei_memory]loadPPConfig() path=/odm/etc/camera/ppconfig.xml
05-15 01:33:14.234   746   746 D PPAlgoConfig: [aaf4016_64D] oneShotNum: 29
05-15 01:33:14.234   746   746 D HwaPPExecuter: [aaf4016_64D] KEY_CA_ALGO SNAP enter HwaPPExecuter
05-15 01:33:14.234   746   746 D HwaPPExecuter: [aaf4016_64D] SNAP ALGO enter create
05-15 01:33:14.234   746   746 D HwaPPAlgoManager: [aaf4016_64D] enter HwaPPAlgoManager
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462adf00, name=PPRender enter MsgProcesser()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462adf00, name=PPRender enter create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462adf00, name=PPRender exit  create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae080, name=Processer enter MsgProcesser()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae080, name=Processer enter create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae080, name=Processer exit  create()
05-15 01:33:14.235   746   746 D HwaPPExecuter: [aaf4016_64D] SNAP ALGO exit create
05-15 01:33:14.235   746   746 D PpAlgoFilter: [HWA_CAM3]algo=ForePp post=0 KEY_CA_CAM3 SNAP enter PpAlgoFilter(): 0x7d462be800 
05-15 01:33:14.235   746   746 D PpAlgo  : [HWA_CAM3]algo=ForePp KEY_CA_CAM3 SNAP enter create
05-15 01:33:14.235   746   746 D HwaPpPluginImpl: [aaf4016_64D] SNAP ALGO enter create env: 0x7d462df910, eventCallback: 0x7d462e0c70, device: 0x7d46295300, framecallback: 0x7d462e0ee8
05-15 01:33:14.235   746   746 D PPAlgoConfig: [aaf4016_64D] enter PPAlgoConfig()
05-15 01:33:14.235   746   746 D PPAlgoConfig: [aaf4016_64D] enter loadPPConfig()
05-15 01:33:14.235   746   746 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:14.235   746   746 I         : , len = 6
05-15 01:33:14.235   746   746 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.235   746   746 I PPAlgoConfig: [aaf4016_64I] [huawei_memory]loadPPConfig() curRamSize=4194304
05-15 01:33:14.235   746   746 I HwaUtils: [aaf4016_64I] getOneCfgFile() path=/odm/etc/camera/ppconfig.xml
05-15 01:33:14.235   746   746 D PPAlgoConfig: [aaf4016_64D] enter loadConfig()
05-15 01:33:14.235   746   746 I PPAlgoConfig: [aaf4016_64I] [huawei_memory]loadPPConfig() path=/odm/etc/camera/ppconfig.xml
05-15 01:33:14.235   746   746 D PPAlgoConfig: [aaf4016_64D] oneShotNum: 29
05-15 01:33:14.235   746   746 D HwaPPExecuter: [aaf4016_64D] KEY_CA_ALGO SNAP enter HwaPPExecuter
05-15 01:33:14.235   746   746 D HwaPPExecuter: [aaf4016_64D] SNAP ALGO enter create
05-15 01:33:14.235   746   746 D HwaPPAlgoManager: [aaf4016_64D] enter HwaPPAlgoManager
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae200, name=PPRender enter MsgProcesser()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae200, name=PPRender enter create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae200, name=PPRender exit  create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae380, name=Processer enter MsgProcesser()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae380, name=Processer enter create()
05-15 01:33:14.235   746   746 D MsgProcesser: [aaf4016_64D] MSGPROCESSER_TRACE this=0x7d462ae380, name=Processer exit  create()
05-15 01:33:14.235   746   746 D HwaPPExecuter: [aaf4016_64D] SNAP ALGO exit create
05-15 01:33:14.235   746   746 D AlgoFilterManager: [HWA_CAM3]KEY_CA_CAM3 exit create, mPipeLineId=3, mIsPlugInCreated=1
05-15 01:33:14.235   746   746 D AlgoFilterStage: [HWA_CAM3]STAGELIFECTRL exit  getAndCreatePluginOrCreateOne(), pipeline id=3, index=2, manger=0x7d462df000
05-15 01:33:14.235   746   746 D AlgoFilterManager: [HWA_CAM3]STAGELIFECTRL enter queryCapability(), mPipeLineId=3
05-15 01:33:14.235   746   746 I HwaUtils: [aaf4016_64I] DMWaterMarkPpAlgo ro.build.hide hide result is false, commerical=true
05-15 01:33:14.235   746   746 D HwaUtils: [aaf4016_64D] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, start=2, step=-1, count = 3,
05-15 01:33:14.235   746   746 I HwaUtils: [aaf4016_64I] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, tstart=2, tcount=1, path=/cust_spec/camera/watermark/dm.argb, access=0, ret=-1
05-15 01:33:14.235   746   746 D HwaUtils: [aaf4016_64D] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, tstart=1, tcount=2, path=/odm/etc/camera/watermark/dm.argb, access=1
05-15 01:33:14.235   746   746 I PPAlgoConfig: [aaf4016_64I] DMWaterMarkPpalgo watermark path is /odm/etc/camera/watermark/dm.argb
05-15 01:33:14.235   746   746 I HwaUtils: [aaf4016_64I] DMWaterMarkPpAlgo ro.build.hide hide result is false, commerical=true
05-15 01:33:14.235   746   746 D HwaUtils: [aaf4016_64D] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, start=2, step=-1, count = 3,
05-15 01:33:14.235   746   746 I HwaUtils: [aaf4016_64I] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, tstart=2, tcount=1, path=/cust_spec/camera/watermark/dm.argb, access=0, ret=-1
05-15 01:33:14.235   746   746 D HwaUtils: [aaf4016_64D] DMWaterMarkPpAlgo bcommericalversion=1, filename=watermark/dm.argb, tstart=1, tcount=2, path=/odm/etc/camera/watermark/dm.argb, access=1
05-15 01:33:14.235   746   746 I PPAlgoConfig: [aaf4016_64I] DMWaterMarkPpalgo watermark path is /odm/etc/camera/watermark/dm.argb
05-15 01:33:14.235   746   746 D IppAlgo : [HWA_CAM3]enter queryCap()
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: FaceDetection
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: SceneDetection
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: TargetTracking
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: SmartAE
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: DualCamAlgo
05-15 01:33:14.235   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: Misc
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: BShutterTryAE
05-15 01:33:14.236   746   746 D AssistAF: [aaf4016_64D] enter onQueryCap()
05-15 01:33:14.236   746   746 E HwaUtils: [aaf4016_64E] FirstLevelXmlParser() LoadFile /odm/etc/camera/mmi/config.xml Failed
05-15 01:33:14.236   746   746 E HwaUtils: [aaf4016_64E] getAttributeString() mFirstLevelElement Is NULL
05-15 01:33:14.236   746   746 E AssistAF: [aaf4016_64E] queryMMICapability() get front testlist fail
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: AssistAF
05-15 01:33:14.236   746   746 D ContrastCalculate: [aaf4016_64D] enter onQueryCap()
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: ContrastCalculate
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: DepthSelfLearnAlgo
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462fe200, ipptype=0, onQueryCap(), algo is queried cap: LaserMgr
05-15 01:33:14.236   746   746 D IppAlgo : [HWA_CAM3]enter queryCap()
05-15 01:33:14.236   746   746 D SdkDepthIppAlgo: [aaf4016_64D] enter onQueryCap()
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: SdkDepthIppAlgo
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: VideoStabilization
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: MirrorDenoise
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: ColorEffect
05-15 01:33:14.236   746   746 D NiceFoodIppAlgo: [aaf4016_64D] enter onQueryCap()
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: NiceFoodIppAlgo
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: HwBeautyIpp
05-15 01:33:14.236   746   746 D HwaIppPluginImpl: [aaf4016_64D] FRMC_ this=0x7d462ff000, ipptype=256, onQueryCap(), algo is queried cap: VideoBokehDspAlgo
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability()digitalzoom supported
05-15 01:33:14.236   746   746 D AlgoFilterManager: [HWA_CAM3]enter queryCapability() facing 0, mPipeLineId=3
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() pre shutter supported
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() DM watermark supported
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability()digitalzoom supported
05-15 01:33:14.236   746   746 D AlgoFilterManager: [HWA_CAM3]enter queryCapability() facing 0, mPipeLineId=3
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() pre shutter supported
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() DM watermark supported
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() LCD Flash Status supported
05-15 01:33:14.236   746   746 I AlgoFilterManager: [HWA_CAM3]enter queryCapability() bshutter and manual AE supported
05-15 01:33:14.236   746   746 I ImagingSystem: queryCapability
05-15 01:33:14.236   746   746 I ImagingSystem: createPipeline: alloc datatable end
05-15 01:33:14.236   746   746 I ImagingSystem: createPipeline(49). 
05-15 01:33:14.236   746   746 I ImagingSystem: queryCapability apiVersion = 770
05-15 01:33:14.237   746   746 I ImagingSystem: [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.237   746   746 I ImagingSystem: [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:14.237   746   746 D ImagingServer: CCfgServer: instance[0x0x7d462d7000]. 
05-15 01:33:14.237   746   746 I ImagingServer: setCallback: enter.
05-15 01:33:14.237   746   746 I ConfigService: CHwCamCfgSvr: instance[0x7d46227b00] ctor
05-15 01:33:14.238   746   746 I ImagingSystem: initConfigService: register camera cfgsvr success
05-15 01:33:14.239   384   384 I chatty  : uid=1000(system) /system/bin/servicemanager expire 182 lines
05-15 01:33:14.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:14.289   922   922 V PackageManager: reconcileAppsData finished 21 packages
05-15 01:33:14.290   922   978 D SystemServerInitThreadPool: Started executing prepareAppData
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:14.290   922   922 V PackageManager: Disabling com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:14.290   922   922 W PackageManager: Unable to disable com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:14.290   922   922 V PackageManager: Enabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:14.290   922   922 W PackageManager: Unable to enable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:14.290   922   922 V PackageManager: Enabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:14.290   922   922 W PackageManager: Unable to enable com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:14.324   733   760 W installd: Ignoring /data/data/com.android.webview/lib with unexpected GID 0 instead of 10038
05-15 01:33:14.326   733   760 W installd: Ignoring /data/data/com.svox.pico/lib with unexpected GID 0 instead of 10045
05-15 01:33:14.383   922   978 D SystemServerTimingAsync: AppDataFixup took to complete: 92ms
05-15 01:33:14.394   922   922 D PackageManager: Ephemeral resolver not found with new action; try old one
05-15 01:33:14.394   922   922 D PackageManager: Ephemeral resolver NOT found; no matching intent filters
05-15 01:33:14.394   922   922 D PackageManager: Ephemeral installer not found with new action; try old one
05-15 01:33:14.394   922   922 D PackageManager: Clear ephemeral installer activity
05-15 01:33:14.423   922   922 D SystemServerTiming: StartPackageManagerService took to complete: 360ms
05-15 01:33:14.424   922   922 I SystemServer: StartOtaDexOptService
05-15 01:33:14.425   922   922 D OTADexopt: No upgrade, skipping A/B artifacts check.
05-15 01:33:14.425   922   922 D SystemServerTiming: StartOtaDexOptService took to complete: 2ms
05-15 01:33:14.425   922   922 I SystemServer: StartUserManagerService
05-15 01:33:14.425   922   922 I SystemServiceManager: Starting com.android.server.pm.UserManagerService$LifeCycle
05-15 01:33:14.425   922   922 D SystemServerTiming: StartUserManagerService took to complete: 0ms
05-15 01:33:14.426   922   922 I SystemServer: InitAttributerCache
05-15 01:33:14.426   922   922 D SystemServerTiming: InitAttributerCache took to complete: 1ms
05-15 01:33:14.426   922   922 I SystemServer: SetSystemProcess
05-15 01:33:14.434   536   536 I lowmemorykiller: ActivityManager connected
05-15 01:33:14.434   922   922 D SystemServerTiming: SetSystemProcess took to complete: 8ms
05-15 01:33:14.435   922   980 I ServiceThread: Enabled StrictMode logging for android.anim looper.
05-15 01:33:14.435   922   922 I SystemServer: StartOverlayManagerService
05-15 01:33:14.438   922   922 I SystemServer: StartSubstratumService
05-15 01:33:14.438   922   981 D SystemServerInitThreadPool: Started executing Init OverlayManagerService
05-15 01:33:14.442   922   922 D SystemServerTiming: StartSubstratumService took to complete: 4ms
05-15 01:33:14.442   922   922 I SystemServer: StartDropBoxManager
05-15 01:33:14.442   922   982 D SystemServerInitThreadPool: Started executing StartSensorService
05-15 01:33:14.442   922   982 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:14.443   922   922 I SystemServiceManager: Starting com.android.server.DropBoxManagerService
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-11 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 11, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-12 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 12, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-13 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 13, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-14 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 14, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-15 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 15, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-17 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 17, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-18 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.445   531   983 D SensorHub: Channel activate-> handle: 18, enabled:0, err: 0
05-15 01:33:14.445   531   983 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-21 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:14.446   531   983 D SensorHub: Channel activate-> handle: 21, enabled:0, err: 0
05-15 01:33:14.446   922   922 D SystemServerTiming: StartDropBoxManager took to complete: 4ms
05-15 01:33:14.446   922   922 I SystemServer: StartBatteryService
05-15 01:33:14.446   922   922 I SystemServiceManager: Starting com.android.server.BatteryService
05-15 01:33:14.447   922   985 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:14.447   922   986 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:14.447   922   982 D SystemServerTimingAsync: StartSensorService took to complete: 5ms
05-15 01:33:14.447   922   982 D SystemServerInitThreadPool: Finished executing StartSensorService
05-15 01:33:14.458   922   922 D SystemServerTiming: StartBatteryService took to complete: 12ms
05-15 01:33:14.458   922   922 I SystemServer: StartUsageService
05-15 01:33:14.459   922   922 I SystemServiceManager: Starting com.android.server.usage.UsageStatsService
05-15 01:33:14.460   922   934 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:14.469   922   922 D SystemServerTiming: StartUsageService took to complete: 11ms
05-15 01:33:14.469   922   922 I SystemServer: StartWebViewUpdateService
05-15 01:33:14.470   922   922 I SystemServiceManager: Starting com.android.server.webkit.WebViewUpdateService
05-15 01:33:14.478   922   922 D SystemServerTiming: StartWebViewUpdateService took to complete: 9ms
05-15 01:33:14.479   922   922 I SystemServer: StartKeyAttestationApplicationIdProviderService
05-15 01:33:14.479   922   935 D SystemServerInitThreadPool: Started executing SecondaryZygotePreload
05-15 01:33:14.479   922   935 I SystemServer: SecondaryZygotePreload
05-15 01:33:14.481   922   922 D SystemServerTiming: StartKeyAttestationApplicationIdProviderService took to complete: 2ms
05-15 01:33:14.481   922   922 I SystemServer: StartKeyChainSystemService
05-15 01:33:14.481   922   922 I SystemServiceManager: Starting com.android.server.security.KeyChainSystemService
05-15 01:33:14.482   922   922 D SystemServerTiming: StartKeyChainSystemService took to complete: 0ms
05-15 01:33:14.482   922   922 I SystemServer: StartSchedulingPolicyService
05-15 01:33:14.482   922   922 D SystemServerTiming: StartSchedulingPolicyService took to complete: 1ms
05-15 01:33:14.482   922   922 I SystemServer: StartTelecomLoaderService
05-15 01:33:14.483   922   922 I SystemServiceManager: Starting com.android.server.telecom.TelecomLoaderService
05-15 01:33:14.483   922   922 D SystemServerTiming: StartTelecomLoaderService took to complete: 1ms
05-15 01:33:14.483   922   922 I SystemServer: StartTelephonyRegistry
05-15 01:33:14.489   922   935 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:14.490   922   922 D SystemServerTiming: StartTelephonyRegistry took to complete: 7ms
05-15 01:33:14.490   922   922 I SystemServer: StartEntropyMixer
05-15 01:33:14.492   922   922 I EntropyMixer: Writing entropy...
05-15 01:33:14.499   922   922 D SystemServerTiming: StartEntropyMixer took to complete: 9ms
05-15 01:33:14.499   922   922 I SystemServer: StartAccountManagerService
05-15 01:33:14.500   728   728 I Zygote  : Lazily preloading resources.
05-15 01:33:14.500   728   728 D Zygote  : begin preload
05-15 01:33:14.500   728   728 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:14.500   728   728 I Zygote  : Preloading ICU data...
05-15 01:33:14.500   922   922 I SystemServiceManager: Starting com.android.server.accounts.AccountManagerService$Lifecycle
05-15 01:33:14.514   922   922 D SystemServerTiming: StartAccountManagerService took to complete: 15ms
05-15 01:33:14.515   922   922 I SystemServer: StartContentService
05-15 01:33:14.518   922   922 I SystemServiceManager: Starting com.android.server.content.ContentService$Lifecycle
05-15 01:33:14.521   922   922 D SystemServerTiming: StartContentService took to complete: 7ms
05-15 01:33:14.521   922   922 I SystemServer: InstallSystemProviders
05-15 01:33:14.539   728   728 D ZygoteInitTiming_lazy: BeginIcuCachePinning took to complete: 38ms
05-15 01:33:14.539   728   728 I Zygote  : Preloading classes...
05-15 01:33:14.567   922   981 D SystemServerInitThreadPool: Finished executing Init OverlayManagerService
05-15 01:33:14.581   922   922 I SettingsState: No settings state /data/system/users/0/settings_ssaid.xml
05-15 01:33:14.585   922   922 D SystemServerTiming: InstallSystemProviders took to complete: 64ms
05-15 01:33:14.585   922   922 I SystemServer: StartVibratorService
05-15 01:33:14.590   922   922 D SystemServerTiming: StartVibratorService took to complete: 5ms
05-15 01:33:14.590   922   922 I SystemServer: StartConsumerIrService
05-15 01:33:14.591   922   922 E System  : ******************************************
05-15 01:33:14.592   922   922 E System  : ************ Failure starting core service
05-15 01:33:14.592   922   922 E System  : java.lang.RuntimeException: IR HAL present, but FEATURE_CONSUMER_IR is not set!
05-15 01:33:14.592   922   922 E System  : 	at com.android.server.ConsumerIrService.<init>(ConsumerIrService.java:54)
05-15 01:33:14.592   922   922 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:831)
05-15 01:33:14.592   922   922 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:14.592   922   922 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:14.592   922   922 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:14.592   922   922 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:14.592   922   922 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:14.592   922   922 I SystemServer: StartInputMethodManagerLifecycle
05-15 01:33:14.593   922   922 I SystemServiceManager: Starting com.android.server.InputMethodManagerService$Lifecycle
05-15 01:33:14.599   922   922 D SystemServerTiming: StartInputMethodManagerLifecycle took to complete: 7ms
05-15 01:33:14.599   922   922 I SystemServer: StartAccessibilityManagerService
05-15 01:33:14.605   922   922 D SystemServerTiming: StartAccessibilityManagerService took to complete: 5ms
05-15 01:33:14.605   922   922 I SystemServer: MakeDisplayReady
05-15 01:33:14.605   922   922 W SystemServer: ***********************************************
05-15 01:33:14.605   922   922 E SystemServer: BOOT FAILURE making display ready
05-15 01:33:14.605   922   922 E SystemServer: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.wm.WindowManagerService.displayReady()' on a null object reference
05-15 01:33:14.605   922   922 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:947)
05-15 01:33:14.605   922   922 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:14.605   922   922 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:14.605   922   922 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:14.605   922   922 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:14.605   922   922 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:14.607   922   922 D SystemServerTiming: MakeDisplayReady took to complete: 2ms
05-15 01:33:14.607   922   922 I SystemServer: StartStorageManagerService
05-15 01:33:14.607   922   922 I SystemServiceManager: Starting com.android.server.StorageManagerService$Lifecycle
05-15 01:33:14.609   733   733 W Binder:733_1: type=1400 audit(0.0:124): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:14.609   733   733 I chatty  : uid=0(root) Binder:733_2 identical 10 lines
05-15 01:33:14.609   733   733 W Binder:733_1: type=1400 audit(0.0:127): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:14.614   922   922 D SystemServerTiming: StartStorageManagerService took to complete: 7ms
05-15 01:33:14.614   922   998 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:14.614   922   922 I SystemServer: StartStorageStatsService
05-15 01:33:14.614   922   998 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:14.614   922   998 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:14.614   922   998 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:14.614   922   922 I SystemServiceManager: Starting com.android.server.usage.StorageStatsService$Lifecycle
05-15 01:33:14.614   922   998 D CryptdConnector: SND -> {1 cryptfs getfield SystemLocale}
05-15 01:33:14.618   922   922 D SystemServerTiming: StartStorageStatsService took to complete: 4ms
05-15 01:33:14.618   922   922 I SystemServer: StartUiModeManager
05-15 01:33:14.618   922   922 I SystemServiceManager: Starting com.android.server.UiModeManagerService
05-15 01:33:14.620   922   982 D SystemServerInitThreadPool: Started executing UiModeManager.onStart
05-15 01:33:14.620   922  1000 D CryptdConnector: RCV <- {200 1 -1}
05-15 01:33:14.620   922   922 D SystemServerTiming: StartUiModeManager took to complete: 2ms
05-15 01:33:14.620   922   922 I SystemServer: UpdatePackagesIfNeeded
05-15 01:33:14.620   922   922 D SystemServerTiming: UpdatePackagesIfNeeded took to complete: 0ms
05-15 01:33:14.620   922   922 I SystemServer: PerformFstrimIfNeeded
05-15 01:33:14.621   922   998 W StorageManagerService: No primary storage mounted!
05-15 01:33:14.621   922   998 D VoldConnector: SND -> {1 asec list}
05-15 01:33:14.621   922   922 D SystemServerTiming: PerformFstrimIfNeeded took to complete: 1ms
05-15 01:33:14.621   922   922 I SystemServer: StartLockSettingsService
05-15 01:33:14.621   922   982 I ActivityManager: Config changes=200 {1.0 ?mcc?mnc [en_US] ldltr ?swdp ?wdp ?hdp ?density ?lsize ?long ?ldr ?wideColorGamut ?orien ?touch ?keyb/?/? ?nav/? s.2}
05-15 01:33:14.621   922   999 D VoldConnector: RCV <- {200 1 asec operation succeeded}
05-15 01:33:14.622   922   998 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:14.624   922   922 I SystemServiceManager: Starting com.android.server.locksettings.LockSettingsService$Lifecycle
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: Failure in UiModeManager.onStart: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityStackSupervisor.getDisplayOverrideConfiguration(ActivityStackSupervisor.java:488)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.performDisplayOverrideConfigUpdate(ActivityManagerService.java:20762)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateGlobalConfiguration(ActivityManagerService.java:20669)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfigurationLocked(ActivityManagerService.java:20547)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfiguration(ActivityManagerService.java:20486)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.sendConfigurationLocked(UiModeManagerService.java:478)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.lambda$-com_android_server_UiModeManagerService_9177(UiModeManagerService.java:236)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.$m$4(Unknown Source:4)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.run(Unknown Source:27)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.SystemServerInitThreadPool.lambda$-com_android_server_SystemServerInitThreadPool_2249(SystemServerInitThreadPool.java:64)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.$m$2(Unknown Source:8)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.run(Unknown Source:19)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:457)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1162)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:636)
05-15 01:33:14.632   922   982 E SystemServerInitThreadPool: 	at com.android.internal.util.ConcurrentUtils$1$1.run(ConcurrentUtils.java:59)
05-15 01:33:14.659   922   922 D SystemServerTiming: StartLockSettingsService took to complete: 38ms
05-15 01:33:14.664   728   728 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:14.665   922   922 I OemLock : OemLock HAL not present on device
05-15 01:33:14.665   922   922 I SystemServer: StartDeviceIdleController
05-15 01:33:14.665   922   922 I SystemServiceManager: Starting com.android.server.DeviceIdleController
05-15 01:33:14.678   728   728 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:14.695   728   728 I zygote  : Thread[1,tid=728,Native,Thread*=0xed3da000,peer=0x12cc0228,"main"] recursive attempt to load library "/system/lib/libmedia_jni.so"
05-15 01:33:14.695   728   728 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:14.696   728   728 I zygote  : Thread[1,tid=728,Native,Thread*=0xed3da000,peer=0x12cc0228,"main"] recursive attempt to load library "/system/lib/libmedia_jni.so"
05-15 01:33:14.696   728   728 I zygote  : Thread[1,tid=728,Native,Thread*=0xed3da000,peer=0x12cc0228,"main"] recursive attempt to load library "/system/lib/libmedia_jni.so"
05-15 01:33:14.766   922   978 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:14.766   922   998 W StorageManagerService: No primary storage mounted!
05-15 01:33:14.766   922   998 D VoldConnector: SND -> {2 asec list}
05-15 01:33:14.766   922   999 D VoldConnector: RCV <- {200 2 asec operation succeeded}
05-15 01:33:14.767   922   922 W SystemServiceManager: Service com.android.server.DeviceIdleController took 101 ms in onStart
05-15 01:33:14.767   922   922 D SystemServerTiming: StartDeviceIdleController took to complete: 103ms
05-15 01:33:14.767   922   922 I SystemServer: StartDevicePolicyManager
05-15 01:33:14.767   922   922 I SystemServiceManager: Starting com.android.server.devicepolicy.DevicePolicyManagerService$Lifecycle
05-15 01:33:14.776   922   922 D SystemServerTiming: StartDevicePolicyManager took to complete: 9ms
05-15 01:33:14.776   922   922 I SystemServer: StartStatusBarManagerService
05-15 01:33:14.782   922   922 D SystemServerTiming: StartStatusBarManagerService took to complete: 6ms
05-15 01:33:14.782   922   922 I SystemServer: StartClipboardService
05-15 01:33:14.782   922   922 I SystemServiceManager: Starting com.android.server.clipboard.ClipboardService
05-15 01:33:14.783   922   922 D SystemServerTiming: StartClipboardService took to complete: 1ms
05-15 01:33:14.783   922   922 I SystemServer: StartNetworkManagementService
05-15 01:33:14.786   728   728 I Zygote  : ...preloaded 4715 classes in 247ms.
05-15 01:33:14.786   728   728 I zygote  : VMRuntime.preloadDexCaches starting
05-15 01:33:14.787   922  1005 I NetworkManagement: onDaemonConnected()
05-15 01:33:14.789   922   922 D SystemServerTiming: StartNetworkManagementService took to complete: 6ms
05-15 01:33:14.789   922   922 I SystemServer: StartTextServicesManager
05-15 01:33:14.789   922   922 I SystemServiceManager: Starting com.android.server.TextServicesManagerService$Lifecycle
05-15 01:33:14.831   728   728 I zygote  : VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:14.831   728   728 I zygote  : VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:14.831   728   728 I zygote  : VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:14.831   728   728 I zygote  : VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:14.831   728   728 I zygote  : VMRuntime.preloadDexCaches finished
05-15 01:33:14.831   728   728 D ZygoteInitTiming_lazy: PreloadClasses took to complete: 293ms
05-15 01:33:14.831   922   922 D SystemServerTiming: StartTextServicesManager took to complete: 42ms
05-15 01:33:14.831   922   922 I SystemServer: StartNetworkScoreService
05-15 01:33:14.833   922   922 D SystemServerTiming: StartNetworkScoreService took to complete: 1ms
05-15 01:33:14.833   922   922 I SystemServer: StartNetworkStatsService
05-15 01:33:14.848   728   728 I Zygote  : Preloading resources...
05-15 01:33:14.856   728   728 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:14.860   922   922 W SystemServer: ***********************************************
05-15 01:33:14.860   922   922 E SystemServer: BOOT FAILURE starting NetworkStats Service
05-15 01:33:14.860   922   922 E SystemServer: java.lang.NullPointerException: missing AlarmManager
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.server.net.NetworkStatsService.<init>(NetworkStatsService.java:309)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:289)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:14.860   922   922 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:14.860   922   922 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:14.860   922   922 D SystemServerTiming: StartNetworkStatsService took to complete: 28ms
05-15 01:33:14.860   922   922 I SystemServer: StartNetworkPolicyManagerService
05-15 01:33:14.863   922   922 W SystemServer: ***********************************************
05-15 01:33:14.863   922   922 E SystemServer: BOOT FAILURE starting NetworkPolicy Service
05-15 01:33:14.863   922   922 E SystemServer: java.lang.NullPointerException: missing networkStats
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:501)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:487)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1096)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:14.863   922   922 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:14.863   922   922 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:14.864   922   922 D SystemServerTiming: StartNetworkPolicyManagerService took to complete: 3ms
05-15 01:33:14.864   922   922 I SystemServer: StartWifi
05-15 01:33:14.866   922   936 I UsageStatsService: User[0] Rollover scheduled @ 2018-05-16 01:33:14(1526434394858)
05-15 01:33:14.866   728   728 I Zygote  : ...preloaded 64 resources in 18ms.
05-15 01:33:14.866   922   936 E AppIdleHistory: Unable to read app idle file for user 0
05-15 01:33:14.868   728   728 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:14.869   728   728 I Zygote  : ...preloaded 41 resources in 3ms.
05-15 01:33:14.869   728   728 D ZygoteInitTiming_lazy: PreloadResources took to complete: 38ms
05-15 01:33:14.875   922   978 D SystemServerTimingAsync: AppDataPrepare took to complete: 492ms
05-15 01:33:14.875   922   978 I PackageManager: Deferred reconcileAppsData finished 73 packages
05-15 01:33:14.875   922   978 D SystemServerInitThreadPool: Finished executing prepareAppData
05-15 01:33:14.879   922   922 I SystemServiceManager: Starting com.android.server.wifi.WifiService
05-15 01:33:14.957   739   805 D CommandListener: Clearing all IP addresses on wlan0
05-15 01:33:14.957   922  1008 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:14.961   728   728 D libEGL  : loaded /vendor/lib/egl/libGLES_mali.so
05-15 01:33:14.963   922   922 D SystemServerTiming: StartWifi took to complete: 99ms
05-15 01:33:14.963   922   922 I SystemServer: StartWifiScanning
05-15 01:33:14.965   922   922 I SystemServiceManager: Starting com.android.server.wifi.scanner.WifiScanningService
05-15 01:33:14.968   922   922 D SystemServerTiming: StartWifiScanning took to complete: 5ms
05-15 01:33:14.968   922   922 I SystemServer: StartWifiRtt
05-15 01:33:14.968   922   922 I SystemServiceManager: Starting com.android.server.wifi.RttService
05-15 01:33:14.969   922   922 D SystemServerTiming: StartWifiRtt took to complete: 1ms
05-15 01:33:14.969   922   922 I SystemServer: No Wi-Fi Aware Service (Aware support Not Present)
05-15 01:33:14.969   922   922 I SystemServer: StartWifiP2P
05-15 01:33:14.970   922   922 I SystemServiceManager: Starting com.android.server.wifi.p2p.WifiP2pService
05-15 01:33:14.974   922   922 D SystemServerTiming: StartWifiP2P took to complete: 5ms
05-15 01:33:14.975   922   922 I SystemServer: StartEthernet
05-15 01:33:14.975   922   922 I SystemServiceManager: Starting com.android.server.ethernet.EthernetService
05-15 01:33:14.978   922   922 D SystemServerTiming: StartEthernet took to complete: 4ms
05-15 01:33:14.978   922   922 I SystemServer: StartConnectivityService
05-15 01:33:14.981   728   728 I Zygote  : Preloading shared libraries...
05-15 01:33:14.982   922   922 D ConnectivityService: ConnectivityService starting up
05-15 01:33:14.983   922   922 W SystemServer: ***********************************************
05-15 01:33:14.983   922   922 E SystemServer: BOOT FAILURE starting Connectivity Service
05-15 01:33:14.983   922   922 E SystemServer: java.lang.NullPointerException: missing INetworkStatsService
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:722)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:690)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1151)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:14.983   922   922 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:14.983   922   922 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:14.983   922   922 D SystemServerTiming: StartConnectivityService took to complete: 5ms
05-15 01:33:14.983   922   922 I SystemServer: StartNsdService
05-15 01:33:14.984   922   922 D NsdService: Network service discovery is enabled
05-15 01:33:14.986   922   922 D SystemServerTiming: StartNsdService took to complete: 3ms
05-15 01:33:14.986   922   922 I SystemServer: StartUpdateLockService
05-15 01:33:14.987   922   922 D SystemServerTiming: StartUpdateLockService took to complete: 1ms
05-15 01:33:14.987   922   922 I SystemServer: WaitForAsecScan
05-15 01:33:14.987   922   922 D SystemServerTiming: WaitForAsecScan took to complete: 0ms
05-15 01:33:14.987   922   922 I SystemServer: StartNotificationManager
05-15 01:33:14.991   922   922 I SystemServiceManager: Starting com.android.server.notification.NotificationManagerService
05-15 01:33:14.993   728   728 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:14.996   728   728 I Zygote  : Installed AndroidKeyStoreProvider in 3ms.
05-15 01:33:15.001   728   728 I Zygote  : Warmed up JCA providers in 5ms.
05-15 01:33:15.001   728   728 D Zygote  : end preload
05-15 01:33:15.001   922   935 D SystemServerTimingAsync: SecondaryZygotePreload took to complete: 522ms
05-15 01:33:15.001   922   935 D SystemServerInitThreadPool: Finished executing SecondaryZygotePreload
05-15 01:33:15.023   922   922 D ConditionProviders.SCP: new ScheduleConditionProvider()
05-15 01:33:15.024   922   922 I ConditionProviders:  Allowing condition provider org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:15.024   922   922 I NotificationListeners:  Allowing notification listener org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:15.024   922   922 I ConditionProviders:  Allowing condition provider com.android.camera2
05-15 01:33:15.025   922   922 D ZenLog  : set_zen_mode: off,init
05-15 01:33:15.036   526   526 D lights  : set_light_notification colorRGB=00000000, onMS=0, offMS=0
05-15 01:33:15.036   526   526 E lights  : failed to open /sys/class/led_config/led_config/led_config_status, fd=-1
05-15 01:33:15.036   526   526 E lights  : failed to open /sys/class/led_alwayson/led_alwayson/version_mode
05-15 01:33:15.040   922   922 E System  : ******************************************
05-15 01:33:15.040   922   922 E System  : ************ Failure starting system services
05-15 01:33:15.040   922   922 E System  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:15.040   922   922 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:15.040   922   922 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:15.040   922   922 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:15.040   922   922 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:15.040   922   922 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:15.040   922   922 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:15.040   922   922 D SystemServerTiming: StartNotificationManager took to complete: 53ms
05-15 01:33:15.040   922   922 E Zygote  : System zygote died with exception
05-15 01:33:15.040   922   922 E Zygote  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:15.040   922   922 E Zygote  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:15.040   922   922 E Zygote  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:15.040   922   922 E Zygote  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:15.040   922   922 E Zygote  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:15.040   922   922 E Zygote  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:15.040   922   922 E Zygote  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:15.040   922   922 D AndroidRuntime: Shutting down VM
--------- beginning of crash
05-15 01:33:15.040   922   922 E AndroidRuntime: *** FATAL EXCEPTION IN SYSTEM PROCESS: main
05-15 01:33:15.040   922   922 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:15.040   922   922 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:15.041   922   922 I Process : Sending signal. PID: 922 SIG: 9
05-15 01:33:15.092   536   536 I lowmemorykiller: ActivityManager disconnected
05-15 01:33:15.092   536   536 I lowmemorykiller: Closing Activity Manager data connection
05-15 01:33:15.093   727   727 E Zygote  : Exit zygote because system server (922) has terminated
05-15 01:33:15.093   727   727 F libc    : Fatal signal 6 (SIGABRT), code 0 in tid 727 (main), pid 727 (main)
05-15 01:33:15.120  1029  1029 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-15 01:33:15.120   751   751 I /system/bin/tombstoned: received crash request for pid 727
05-15 01:33:15.121  1029  1029 I crash_dump64: performing dump of process 727 (target tid = 727)
05-15 01:33:15.121   727   727 F libc    : failed to wait for crash_dump helper: No child processes
05-15 01:33:15.121  1029  1029 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-15 01:33:15.121  1029  1029 F DEBUG   : LineageOS Version: 'unknown'
05-15 01:33:15.121  1029  1029 F DEBUG   : Build fingerprint: 'Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys'
05-15 01:33:15.121  1029  1029 F DEBUG   : Revision: '0'
05-15 01:33:15.121  1029  1029 F DEBUG   : ABI: 'arm64'
05-15 01:33:15.121  1029  1029 F DEBUG   : pid: 727, tid: 727, name: main  >>> zygote64 <<<
05-15 01:33:15.121  1029  1029 F DEBUG   : signal 6 (SIGABRT), code 0 (SI_USER), fault addr --------
05-15 01:33:15.121  1029  1029 F DEBUG   :     x0   0000000000000000  x1   0000000000000009  x2   0000000000000005  x3   0000000000000003
05-15 01:33:15.121  1029  1029 F DEBUG   :     x4   0000000040100401  x5   80404000a800a800  x6   0000000000000000  x7   7f7f7f7f7f7f7f7f
05-15 01:33:15.121  1029  1029 F DEBUG   :     x8   0000000000000081  x9   3421590554d99019  x10  0000007fe3a49810  x11  0000000000000037
05-15 01:33:15.121  1029  1029 F DEBUG   :     x12  000000000000000b  x13  ffffffffffffffff  x14  ff00000000000000  x15  ffffffffffffffff
05-15 01:33:15.121  1029  1029 F DEBUG   :     x16  0000007a8aea8300  x17  0000007a88a3b55c  x18  0000000070215150  x19  0000007a8b7a6a50
05-15 01:33:15.121  1029  1029 F DEBUG   :     x20  0000007a8ae541e6  x21  0000007a8ae5464a  x22  0000007a8ae546a6  x23  000000000000039a
05-15 01:33:15.121  1029  1029 F DEBUG   :     x24  0000007a8ae5468e  x25  0000007a8ae54669  x26  0000007a8b7a6a40  x27  0000000000000002
05-15 01:33:15.121  1029  1029 F DEBUG   :     x28  0000007a8aead000  x29  0000007fe3a49de0  x30  0000007a8ae0e00c
05-15 01:33:15.121  1029  1029 F DEBUG   :     sp   0000007fe3a49d80  pc   0000007a88a3b564  pstate 0000000060000000
05-15 01:33:15.229   740   763 E /system/bin/storaged: getService package_native failed
05-15 01:33:15.234   740   763 I /system/bin/storaged: storaged: Start
05-15 01:33:15.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:15.302   793   793 I lhd     : Lhd::LHD Init took 3.890s
05-15 01:33:15.370  1029  1029 F DEBUG   : 
05-15 01:33:15.370  1029  1029 F DEBUG   : backtrace:
05-15 01:33:15.370  1029  1029 F DEBUG   :     #00 pc 000000000006a564  /system/lib64/libc.so (kill+8)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #01 pc 0000000000176008  /system/lib64/libandroid_runtime.so ((anonymous namespace)::SigChldHandler(int)+280)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #02 pc 00000000000005f0  [vdso:0000007a8b63b000]
05-15 01:33:15.370  1029  1029 F DEBUG   :     #03 pc 0000000000069ea0  /system/lib64/libc.so (__ppoll+4)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #04 pc 00000000000265e4  /system/lib64/libc.so (poll+88)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #05 pc 000000000002e9a8  /system/lib64/libjavacore.so (Linux_poll(_JNIEnv*, _jobject*, _jobjectArray*, int)+800)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #06 pc 000000000030bad0  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.Linux.fcntlVoid [DEDUPED]+160)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #07 pc 0000000000300a74  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.BlockGuardOs.poll+228)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #08 pc 00000000002b67a4  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (android.system.Os.poll+84)
05-15 01:33:15.370  1029  1029 F DEBUG   :     #09 pc 000000000164e488  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteServer.runSelectLoop+664)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #10 pc 0000000001652ed8  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteInit.main+2728)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #11 pc 000000000054744c  /system/lib64/libart.so (art_quick_invoke_static_stub+604)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #12 pc 00000000000dc7b0  /system/lib64/libart.so (art::ArtMethod::Invoke(art::Thread*, unsigned int*, unsigned int, art::JValue*, char const*)+260)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #13 pc 000000000046bb70  /system/lib64/libart.so (art::InvokeWithArgArray(art::ScopedObjectAccessAlreadyRunnable const&, art::ArtMethod*, art::ArgArray*, art::JValue*, char const*)+100)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #14 pc 000000000046b79c  /system/lib64/libart.so (art::InvokeWithVarArgs(art::ScopedObjectAccessAlreadyRunnable const&, _jobject*, _jmethodID*, std::__va_list)+420)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #15 pc 0000000000372a54  /system/lib64/libart.so (art::JNI::CallStaticVoidMethodV(_JNIEnv*, _jclass*, _jmethodID*, std::__va_list)+620)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #16 pc 00000000000a6fb8  /system/lib64/libandroid_runtime.so (_JNIEnv::CallStaticVoidMethod(_jclass*, _jmethodID*, ...)+120)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #17 pc 00000000000a9728  /system/lib64/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+832)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #18 pc 0000000000002440  /system/bin/app_process64 (main+1328)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #19 pc 00000000000a14d4  /system/lib64/libc.so (__libc_init+88)
05-15 01:33:15.374  1029  1029 F DEBUG   :     #20 pc 0000000000001e70  /system/bin/app_process64 (_start_main+80)
05-15 01:33:15.517  1029  1029 E crash_dump64: unable to connect to activity manager: No such file or directory
05-15 01:33:15.518   751   751 E /system/bin/tombstoned: Tombstone written to: /data/tombstones/tombstone_08
05-15 01:33:15.889  1035  1035 W ksdioirqd/mmc3: type=1400 audit(0.0:128): avc: granted { setsched } for scontext=u:r:kernel:s0 tcontext=u:r:kernel:s0 tclass=process
05-15 01:33:16.151  1042  1042 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:16.152  1042  1042 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:16.152  1042  1042 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:16.152  1042  1042 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:16.152  1042  1042 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:16.166  1041  1041 I wificond: wificond is starting up...
05-15 01:33:16.170  1042  1042 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:16.170  1042  1042 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:16.170  1042  1042 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:16.170  1040  1040 I Netd    : Netd 1.0 starting
05-15 01:33:16.170  1040  1040 D TetherController: Setting IP forward enable = 0
05-15 01:33:16.185  1040  1040 I Netd    : Creating child chains: 11.1ms
05-15 01:33:16.186  1040  1040 I Netd    : Setting up OEM hooks: 0.2ms
05-15 01:33:16.189  1040  1040 I Netd    : Setting up FirewallController hooks: 3.6ms
05-15 01:33:16.191  1040  1040 I Netd    : Setting up NatController hooks: 2.1ms
05-15 01:33:16.193  1040  1040 I Netd    : Setting up BandwidthController hooks: 1.4ms
05-15 01:33:16.193  1040  1040 I Netd    : Setting up IdletimerController hooks: 0.1ms
05-15 01:33:16.196  1040  1040 I Netd    : Disabling bandwidth control: 3.2ms
05-15 01:33:16.197  1040  1040 E Netd    : cannot find interface dummy0
05-15 01:33:16.197  1040  1040 I Netd    : Initializing RouteController: 1.6ms
05-15 01:33:16.198  1040  1040 E Netd    : Unable to create netlink socket: Protocol not supported
05-15 01:33:16.198  1040  1040 W Netd    : Unable to open qlog quota socket, check if xt_quota2 can send via UeventHandler
05-15 01:33:16.198  1040  1040 D MDnsDS  : MDnsSdListener::Hander starting up
05-15 01:33:16.199  1040  1055 D MDnsDS  : MDnsSdListener starting to monitor
05-15 01:33:16.199  1040  1055 D MDnsDS  : Going to poll with pollCount 1
05-15 01:33:16.199  1040  1040 I Netd    : Registering NetdNativeService: 0.6ms
05-15 01:33:16.199  1040  1040 I Netd    : Starting CommandListener: 0.1ms
05-15 01:33:16.201  1040  1040 I Netd    : Registering NetdHwService: 1.3ms
05-15 01:33:16.201  1040  1040 I Netd    : Netd started in 31ms
05-15 01:33:16.219  1038  1038 W cameraserver: type=1400 audit(0.0:129): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2092 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:16.219  1038  1038 W cameraserver: type=1400 audit(0.0:130): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2295 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:16.220  1038  1038 I cameraserver: ServiceManager: 0xe5d179a0
05-15 01:33:16.220  1038  1038 I CameraService: CameraService started (pid=1038)
05-15 01:33:16.220  1038  1038 I CameraService: CameraService process starting
05-15 01:33:16.220  1038  1038 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:16.220  1038  1038 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:16.222  1038  1038 E vndksupport: Could not load /vendor/lib/hw/android.hardware.camera.provider@2.4-impl.so from sphal namespace: dlopen failed: library "android.hardware.camera.device@1.0.so" not found.
05-15 01:33:16.222  1038  1038 E /system/bin/cameraserver: Failed to dlopen android.hardware.camera.provider@2.4-impl.so: unknown error
05-15 01:33:16.226  1037  1037 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 30 lines
05-15 01:33:16.229  1039  1039 I mediaserver: ServiceManager: 0xec497a40
05-15 01:33:16.230  1039  1039 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:16.235   511  1034 I chatty  : uid=1041(audioserver) HwBinder:511_3 expire 268 lines
05-15 01:33:16.255   346   346 E         : pid 511, opration oeminfo_read OK
05-15 01:33:16.255   346   346 E         : 
05-15 01:33:16.257   511  1073 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 1 line
05-15 01:33:16.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:16.290  1036  1036 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:16.293  1036  1036 I zygote64: option[0]=-Xzygote
05-15 01:33:16.293  1036  1036 I zygote64: option[1]=-Xusetombstonedtraces
05-15 01:33:16.293  1036  1036 I zygote64: option[2]=exit
05-15 01:33:16.293  1036  1036 I zygote64: option[3]=vfprintf
05-15 01:33:16.293  1036  1036 I zygote64: option[4]=sensitiveThread
05-15 01:33:16.293  1036  1036 I zygote64: option[5]=-verbose:gc
05-15 01:33:16.293  1036  1036 I zygote64: option[6]=-Xms8m
05-15 01:33:16.293  1036  1036 I zygote64: option[7]=-Xmx512m
05-15 01:33:16.293  1036  1036 I zygote64: option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:16.293  1036  1036 I zygote64: option[9]=-XX:HeapMinFree=2m
05-15 01:33:16.293  1036  1036 I zygote64: option[10]=-XX:HeapMaxFree=8m
05-15 01:33:16.293  1036  1036 I zygote64: option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:16.293  1036  1036 I zygote64: option[12]=-Xusejit:true
05-15 01:33:16.293  1036  1036 I zygote64: option[13]=-Xjitsaveprofilinginfo
05-15 01:33:16.293  1036  1036 I zygote64: option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:16.293  1036  1036 I zygote64: option[15]=-Xlockprofthreshold:500
05-15 01:33:16.293  1036  1036 I zygote64: option[16]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[17]=--runtime-arg
05-15 01:33:16.293  1036  1036 I zygote64: option[18]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[19]=-Xms64m
05-15 01:33:16.293  1036  1036 I zygote64: option[20]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[21]=--runtime-arg
05-15 01:33:16.293  1036  1036 I zygote64: option[22]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[23]=-Xmx64m
05-15 01:33:16.293  1036  1036 I zygote64: option[24]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:16.293  1036  1036 I zygote64: option[26]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:16.293  1036  1036 I zygote64: option[28]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:16.293  1036  1036 I zygote64: option[30]=-Xcompiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[31]=--runtime-arg
05-15 01:33:16.293  1036  1036 I zygote64: option[32]=-Xcompiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[33]=-Xms64m
05-15 01:33:16.293  1036  1036 I zygote64: option[34]=-Xcompiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[35]=--runtime-arg
05-15 01:33:16.293  1036  1036 I zygote64: option[36]=-Xcompiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[37]=-Xmx512m
05-15 01:33:16.293  1036  1036 I zygote64: option[38]=-Xcompiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[39]=-j4
05-15 01:33:16.293  1036  1036 I zygote64: option[40]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[41]=-j4
05-15 01:33:16.293  1036  1036 I zygote64: option[42]=-Ximage-compiler-option
05-15 01:33:16.293  1036  1036 I zygote64: option[43]=--instruction-set-variant=generic
05-15 01:33:16.294  1036  1036 I zygote64: option[44]=-Xcompiler-option
05-15 01:33:16.294  1036  1036 I zygote64: option[45]=--instruction-set-variant=generic
05-15 01:33:16.294  1036  1036 I zygote64: option[46]=-Ximage-compiler-option
05-15 01:33:16.294  1036  1036 I zygote64: option[47]=--instruction-set-features=default
05-15 01:33:16.294  1036  1036 I zygote64: option[48]=-Xcompiler-option
05-15 01:33:16.294  1036  1036 I zygote64: option[49]=--instruction-set-features=default
05-15 01:33:16.294  1036  1036 I zygote64: option[50]=-Duser.locale=en-US
05-15 01:33:16.294  1036  1036 I zygote64: option[51]=--cpu-abilist=arm64-v8a
05-15 01:33:16.294  1036  1036 I zygote64: option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:16.386  1036  1036 D Zygote  : begin preload
05-15 01:33:16.386  1036  1036 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:16.386  1036  1036 I Zygote  : Preloading ICU data...
05-15 01:33:16.390  1036  1036 D Zygote64Timing: BeginIcuCachePinning took to complete: 5ms
05-15 01:33:16.390  1036  1036 I Zygote  : Preloading classes...
05-15 01:33:16.458  1036  1036 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:16.463  1036  1036 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:16.467  1036  1036 I zygote64: Thread[1,tid=1036,Native,Thread*=0x7eca6bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:16.467  1036  1036 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:16.467  1036  1036 I zygote64: Thread[1,tid=1036,Native,Thread*=0x7eca6bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:16.467  1036  1036 I zygote64: Thread[1,tid=1036,Native,Thread*=0x7eca6bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:16.502  1036  1036 I Zygote  : ...preloaded 4715 classes in 112ms.
05-15 01:33:16.502  1036  1036 I zygote64: VMRuntime.preloadDexCaches starting
05-15 01:33:16.531  1036  1036 I zygote64: VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:16.531  1036  1036 I zygote64: VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:16.531  1036  1036 I zygote64: VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:16.531  1036  1036 I zygote64: VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:16.531  1036  1036 I zygote64: VMRuntime.preloadDexCaches finished
05-15 01:33:16.531  1036  1036 D Zygote64Timing: PreloadClasses took to complete: 141ms
05-15 01:33:16.546  1036  1036 I Zygote  : Preloading resources...
05-15 01:33:16.550  1036  1036 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:16.558  1036  1036 I Zygote  : ...preloaded 64 resources in 12ms.
05-15 01:33:16.560  1036  1036 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:16.560  1036  1036 I Zygote  : ...preloaded 41 resources in 2ms.
05-15 01:33:16.560  1036  1036 D Zygote64Timing: PreloadResources took to complete: 29ms
05-15 01:33:16.576  1036  1036 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:16.586  1036  1036 I Zygote  : Preloading shared libraries...
05-15 01:33:16.592  1036  1036 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:16.593  1036  1036 I Zygote  : Installed AndroidKeyStoreProvider in 1ms.
05-15 01:33:16.597  1036  1036 I Zygote  : Warmed up JCA providers in 4ms.
05-15 01:33:16.597  1036  1036 D Zygote  : end preload
05-15 01:33:16.597  1036  1036 D Zygote64Timing: ZygotePreload took to complete: 212ms
05-15 01:33:16.607  1036  1036 I zygote64: Explicit concurrent copying GC freed 29303(2MB) AllocSpace objects, 25(476KB) LOS objects, 80% free, 1524KB/7MB, paused 31us total 9.388ms
05-15 01:33:16.614  1036  1036 I zygote64: Explicit concurrent copying GC freed 5435(198KB) AllocSpace objects, 0(0B) LOS objects, 81% free, 1357KB/7MB, paused 20us total 6.042ms
05-15 01:33:16.614  1036  1036 D Zygote64Timing: PostZygoteInitGC took to complete: 17ms
05-15 01:33:16.614  1036  1036 D Zygote64Timing: ZygoteInit took to complete: 229ms
05-15 01:33:16.643  1036  1036 I zygote64: Global filter of size 170 installed
05-15 01:33:16.664  1036  1036 I Zygote  : System server process 1079 has been created
05-15 01:33:16.664  1036  1036 E Zygote  : couldn't write 1079 to /dev/memcg/system/tasks
05-15 01:33:16.665  1036  1036 I Zygote  : Accepting command socket connections
05-15 01:33:16.670  1079  1079 I chatty  : uid=1000 system_server expire 144 lines
05-15 01:33:16.685  1079  1079 I SystemServer: InitBeforeStartServices
05-15 01:33:16.685  1079  1079 I SystemServer: Entered the Android system server!
05-15 01:33:16.739   733   733 W Binder:733_1: type=1400 audit(0.0:131): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:16.739   733   733 W Binder:733_1: type=1400 audit(0.0:132): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:16.749  1079  1079 D SystemServerTiming: InitBeforeStartServices took to complete: 64ms
05-15 01:33:16.749  1079  1079 I SystemServer: StartServices
05-15 01:33:16.749  1079  1079 I SystemServer: Reading configuration...
05-15 01:33:16.749  1079  1079 I SystemServer: ReadingSystemConfig
05-15 01:33:16.750  1079  1079 D SystemServerTiming: ReadingSystemConfig took to complete: 0ms
05-15 01:33:16.750  1079  1079 I SystemServer: StartInstaller
05-15 01:33:16.750  1079  1079 I SystemServiceManager: Starting com.android.server.pm.Installer
05-15 01:33:16.750  1079  1092 D SystemServerInitThreadPool: Started executing ReadingSystemConfig
05-15 01:33:16.751  1079  1079 D SystemServerTiming: StartInstaller took to complete: 2ms
05-15 01:33:16.751  1079  1079 I SystemServer: DeviceIdentifiersPolicyService
05-15 01:33:16.751  1079  1079 I SystemServiceManager: Starting com.android.server.os.DeviceIdentifiersPolicyService
05-15 01:33:16.751  1079  1079 D SystemServerTiming: DeviceIdentifiersPolicyService took to complete: 0ms
05-15 01:33:16.752  1079  1079 I SystemServer: StartActivityManager
05-15 01:33:16.752  1079  1079 I SystemServiceManager: Starting com.android.server.am.ActivityManagerService$Lifecycle
05-15 01:33:16.758  1079  1092 D SystemServerInitThreadPool: Finished executing ReadingSystemConfig
05-15 01:33:16.759  1079  1079 I ActivityManager: Memory class: 384
05-15 01:33:16.760  1079  1094 I ServiceThread: Enabled StrictMode logging for ActivityManager looper.
05-15 01:33:16.760  1079  1095 I ServiceThread: Enabled StrictMode logging for android.ui looper.
05-15 01:33:16.768  1079  1079 D BatteryStatsImpl: Reading daily items from /data/system/batterystats-daily.xml
05-15 01:33:16.769  1079  1097 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:16.770  1079  1097 E BatteryExternalStatsWorker: no controller energy info supplied for telephony
05-15 01:33:16.771  1079  1097 E KernelUidCpuFreqTimeReader: Failed to read /proc/uid_time_in_state: java.io.FileNotFoundException: /proc/uid_time_in_state (No such file or directory)
05-15 01:33:16.804  1079  1079 I AppOps  : No existing app ops /data/system/appops.xml; starting empty
05-15 01:33:16.805  1079  1079 I IntentFirewall: Read new rules (A:0 B:0 S:0)
05-15 01:33:16.806  1079  1101 I ServiceThread: Enabled StrictMode logging for android.display looper.
05-15 01:33:16.810  1079  1079 D AppOps  : AppOpsService published
05-15 01:33:16.810  1079  1079 D SystemServerTiming: StartActivityManager took to complete: 59ms
05-15 01:33:16.810  1079  1079 I SystemServer: StartPowerManager
05-15 01:33:16.810  1079  1079 I SystemServiceManager: Starting com.android.server.power.PowerManagerService
05-15 01:33:16.811  1079  1103 I ServiceThread: Enabled StrictMode logging for PowerManagerService looper.
05-15 01:33:16.812  1079  1079 D SystemServerTiming: StartPowerManager took to complete: 2ms
05-15 01:33:16.812  1079  1079 I SystemServer: InitPowerManagement
05-15 01:33:16.812  1079  1079 D SystemServerTiming: InitPowerManagement took to complete: 0ms
05-15 01:33:16.812  1079  1079 I SystemServer: StartRecoverySystemService
05-15 01:33:16.813  1079  1079 I SystemServiceManager: Starting com.android.server.RecoverySystemService
05-15 01:33:16.813  1079  1079 D SystemServerTiming: StartRecoverySystemService took to complete: 1ms
05-15 01:33:16.813  1079  1079 V RescueParty: Disabled because of active USB connection
05-15 01:33:16.813  1079  1079 I SystemServer: StartLightsService
05-15 01:33:16.813  1079  1079 I SystemServiceManager: Starting com.android.server.lights.LightsService
05-15 01:33:16.813  1079  1079 D SystemServerTiming: StartLightsService took to complete: 0ms
05-15 01:33:16.813  1079  1079 I SystemServer: StartDisplayManager
05-15 01:33:16.813  1079  1079 I SystemServiceManager: Starting com.android.server.display.DisplayManagerService
05-15 01:33:16.814  1079  1079 D SystemServerTiming: StartDisplayManager took to complete: 1ms
05-15 01:33:16.814  1079  1079 I SystemServer: WaitForDisplay
05-15 01:33:16.814  1079  1079 I SystemServiceManager: Starting phase 100
05-15 01:33:16.816  1079  1101 I DisplayManagerService: Display device added: DisplayDeviceInfo{"Built-in Screen": uniqueId="local:0", 1080 x 1920, modeId 1, defaultModeId 1, supportedModes [{id=1, width=1080, height=1920, fps=60.000004}], colorMode 0, supportedColorModes [0], HdrCapabilities android.view.Display$HdrCapabilities@1d6308, density 480, 365.76 x 366.676 dpi, appVsyncOff 2000000, presDeadline 13666666, touch INTERNAL, rotation 0, type BUILT_IN, state UNKNOWN, FLAG_DEFAULT_DISPLAY, FLAG_ROTATES_WITH_CONTENT, FLAG_SECURE, FLAG_SUPPORTS_PROTECTED_BUFFERS}
05-15 01:33:16.817   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:16.818  1079  1079 D SystemServerTiming: WaitForDisplay took to complete: 4ms
05-15 01:33:16.818  1079  1101 I DisplayManagerService: Display device changed state: "Built-in Screen", ON
05-15 01:33:16.818  1079  1079 I SystemServer: StartPackageManagerService
05-15 01:33:16.823  1079  1079 D SELinuxMMAC: Using policy file /system/etc/selinux/plat_mac_permissions.xml
05-15 01:33:16.823  1079  1079 D SELinuxMMAC: Using policy file /vendor/etc/selinux/nonplat_mac_permissions.xml
05-15 01:33:16.854  1079  1079 W PackageManager: Failed to parse /system/framework/arm: Missing base APK in /system/framework/arm
05-15 01:33:16.854  1079  1079 W PackageManager: Failed to parse /system/framework/oat: Missing base APK in /system/framework/oat
05-15 01:33:16.854  1079  1079 W PackageManager: Failed to parse /system/framework/arm64: Missing base APK in /system/framework/arm64
05-15 01:33:16.905  1079  1079 I PackageManager: Finished scanning system apps. Time: 53 ms, packageCount: 94 , timePerPackage: 0 , cached: 94
05-15 01:33:16.905  1079  1079 I PackageManager: Finished scanning non-system apps. Time: 0 ms, packageCount: 0 , timePerPackage: 0 , cached: 0
05-15 01:33:16.908  1079  1079 I PackageManager: Time to scan packages: 0.054 seconds
05-15 01:33:16.910  1079  1079 V PackageManager: reconcileAppsData for null u0 0x3 migrateAppData=true
05-15 01:33:16.939  1079  1079 V PackageManager: reconcileAppsData finished 21 packages
05-15 01:33:16.939  1079  1119 D SystemServerInitThreadPool: Started executing prepareAppData
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:16.939  1079  1079 V PackageManager: Disabling com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to disable com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:16.939  1079  1079 V PackageManager: Enabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to enable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:16.939  1079  1079 V PackageManager: Enabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:16.939  1079  1079 W PackageManager: Unable to enable com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:16.941   733   760 W installd: Ignoring /data/data/com.android.webview/lib with unexpected GID 0 instead of 10038
05-15 01:33:16.941   733   760 W installd: Ignoring /data/data/com.svox.pico/lib with unexpected GID 0 instead of 10045
05-15 01:33:16.943  1079  1119 D SystemServerTimingAsync: AppDataFixup took to complete: 4ms
05-15 01:33:16.960  1079  1079 D PackageManager: Ephemeral resolver not found with new action; try old one
05-15 01:33:16.960  1079  1079 D PackageManager: Ephemeral resolver NOT found; no matching intent filters
05-15 01:33:16.960  1079  1079 D PackageManager: Ephemeral installer not found with new action; try old one
05-15 01:33:16.961  1079  1079 D PackageManager: Clear ephemeral installer activity
05-15 01:33:16.986  1079  1079 D SystemServerTiming: StartPackageManagerService took to complete: 168ms
05-15 01:33:16.986  1079  1079 I SystemServer: StartOtaDexOptService
05-15 01:33:16.987  1079  1079 D OTADexopt: No upgrade, skipping A/B artifacts check.
05-15 01:33:16.987  1079  1079 D SystemServerTiming: StartOtaDexOptService took to complete: 1ms
05-15 01:33:16.987  1079  1079 I SystemServer: StartUserManagerService
05-15 01:33:16.987  1079  1079 I SystemServiceManager: Starting com.android.server.pm.UserManagerService$LifeCycle
05-15 01:33:16.987  1079  1079 D SystemServerTiming: StartUserManagerService took to complete: 0ms
05-15 01:33:16.987  1079  1079 I SystemServer: InitAttributerCache
05-15 01:33:16.987  1079  1079 D SystemServerTiming: InitAttributerCache took to complete: 0ms
05-15 01:33:16.987  1079  1079 I SystemServer: SetSystemProcess
05-15 01:33:16.991   536   536 I lowmemorykiller: ActivityManager connected
05-15 01:33:16.991  1079  1079 D SystemServerTiming: SetSystemProcess took to complete: 4ms
05-15 01:33:16.992  1079  1121 I ServiceThread: Enabled StrictMode logging for android.anim looper.
05-15 01:33:16.992  1079  1079 I SystemServer: StartOverlayManagerService
05-15 01:33:16.993  1079  1079 I SystemServer: StartSubstratumService
05-15 01:33:16.993  1079  1122 D SystemServerInitThreadPool: Started executing Init OverlayManagerService
05-15 01:33:16.994  1079  1079 D SystemServerTiming: StartSubstratumService took to complete: 0ms
05-15 01:33:16.994  1079  1079 I SystemServer: StartDropBoxManager
05-15 01:33:16.994  1079  1079 I SystemServiceManager: Starting com.android.server.DropBoxManagerService
05-15 01:33:16.994  1079  1123 D SystemServerInitThreadPool: Started executing StartSensorService
05-15 01:33:16.994  1079  1123 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:16.995  1079  1079 D SystemServerTiming: StartDropBoxManager took to complete: 1ms
05-15 01:33:16.995  1079  1079 I SystemServer: StartBatteryService
05-15 01:33:16.995  1079  1079 I SystemServiceManager: Starting com.android.server.BatteryService
05-15 01:33:16.995   531   531 E /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: ISensors::poll() re-entry. I do not know what to do except killing myself.
05-15 01:33:17.002  1079  1079 D SystemServerTiming: StartBatteryService took to complete: 7ms
05-15 01:33:17.002  1079  1091 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:17.002  1079  1079 I SystemServer: StartUsageService
05-15 01:33:17.002  1079  1079 I SystemServiceManager: Starting com.android.server.usage.UsageStatsService
05-15 01:33:17.004  1079  1079 D SystemServerTiming: StartUsageService took to complete: 2ms
05-15 01:33:17.004  1079  1079 I SystemServer: StartWebViewUpdateService
05-15 01:33:17.004  1079  1079 I SystemServiceManager: Starting com.android.server.webkit.WebViewUpdateService
05-15 01:33:17.006  1079  1079 D SystemServerTiming: StartWebViewUpdateService took to complete: 2ms
05-15 01:33:17.006  1079  1079 I SystemServer: StartKeyAttestationApplicationIdProviderService
05-15 01:33:17.006  1079  1092 D SystemServerInitThreadPool: Started executing SecondaryZygotePreload
05-15 01:33:17.006  1079  1092 I SystemServer: SecondaryZygotePreload
05-15 01:33:17.007  1079  1079 D SystemServerTiming: StartKeyAttestationApplicationIdProviderService took to complete: 1ms
05-15 01:33:17.007  1079  1079 I SystemServer: StartKeyChainSystemService
05-15 01:33:17.007  1079  1079 I SystemServiceManager: Starting com.android.server.security.KeyChainSystemService
05-15 01:33:17.007  1079  1079 D SystemServerTiming: StartKeyChainSystemService took to complete: 0ms
05-15 01:33:17.007  1079  1079 I SystemServer: StartSchedulingPolicyService
05-15 01:33:17.008  1079  1079 D SystemServerTiming: StartSchedulingPolicyService took to complete: 0ms
05-15 01:33:17.008  1079  1079 I SystemServer: StartTelecomLoaderService
05-15 01:33:17.008  1079  1079 I SystemServiceManager: Starting com.android.server.telecom.TelecomLoaderService
05-15 01:33:17.008  1079  1079 D SystemServerTiming: StartTelecomLoaderService took to complete: 0ms
05-15 01:33:17.008  1079  1079 I SystemServer: StartTelephonyRegistry
05-15 01:33:17.010  1079  1079 D SystemServerTiming: StartTelephonyRegistry took to complete: 2ms
05-15 01:33:17.010  1079  1079 I SystemServer: StartEntropyMixer
05-15 01:33:17.011  1079  1079 I EntropyMixer: Writing entropy...
05-15 01:33:17.012  1079  1079 D SystemServerTiming: StartEntropyMixer took to complete: 2ms
05-15 01:33:17.012  1079  1079 I SystemServer: StartAccountManagerService
05-15 01:33:17.012  1079  1079 I SystemServiceManager: Starting com.android.server.accounts.AccountManagerService$Lifecycle
05-15 01:33:17.015  1079  1079 D SystemServerTiming: StartAccountManagerService took to complete: 3ms
05-15 01:33:17.016  1079  1079 I SystemServer: StartContentService
05-15 01:33:17.016  1079  1079 I SystemServiceManager: Starting com.android.server.content.ContentService$Lifecycle
05-15 01:33:17.016  1079  1079 D SystemServerTiming: StartContentService took to complete: 1ms
05-15 01:33:17.016  1079  1079 I SystemServer: InstallSystemProviders
05-15 01:33:17.017  1079  1092 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:17.029  1124  1124 I chatty  : uid=1000(system) /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service expire 62 lines
05-15 01:33:17.033  1079  1079 I SettingsState: No settings state /data/system/users/0/settings_ssaid.xml
05-15 01:33:17.036  1079  1079 D SystemServerTiming: InstallSystemProviders took to complete: 20ms
05-15 01:33:17.036  1079  1079 I SystemServer: StartVibratorService
05-15 01:33:17.037  1079  1092 E SystemServer: Unable to preload default resources
05-15 01:33:17.037  1079  1092 D SystemServerTimingAsync: SecondaryZygotePreload took to complete: 31ms
05-15 01:33:17.037  1079  1092 D SystemServerInitThreadPool: Finished executing SecondaryZygotePreload
05-15 01:33:17.041  1079  1079 D SystemServerTiming: StartVibratorService took to complete: 5ms
05-15 01:33:17.041  1079  1079 I SystemServer: StartConsumerIrService
05-15 01:33:17.042  1079  1079 E System  : ******************************************
05-15 01:33:17.042  1079  1079 E System  : ************ Failure starting core service
05-15 01:33:17.042  1079  1079 E System  : java.lang.RuntimeException: IR HAL present, but FEATURE_CONSUMER_IR is not set!
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.server.ConsumerIrService.<init>(ConsumerIrService.java:54)
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:831)
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.042  1079  1079 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.042  1079  1079 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.042  1079  1079 I SystemServer: StartInputMethodManagerLifecycle
05-15 01:33:17.042  1079  1079 I SystemServiceManager: Starting com.android.server.InputMethodManagerService$Lifecycle
05-15 01:33:17.045  1079  1079 D SystemServerTiming: StartInputMethodManagerLifecycle took to complete: 3ms
05-15 01:33:17.045  1079  1079 I SystemServer: StartAccessibilityManagerService
05-15 01:33:17.047  1079  1079 D SystemServerTiming: StartAccessibilityManagerService took to complete: 2ms
05-15 01:33:17.047  1079  1079 I SystemServer: MakeDisplayReady
05-15 01:33:17.047  1079  1079 W SystemServer: ***********************************************
05-15 01:33:17.047  1079  1079 E SystemServer: BOOT FAILURE making display ready
05-15 01:33:17.047  1079  1079 E SystemServer: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.wm.WindowManagerService.displayReady()' on a null object reference
05-15 01:33:17.047  1079  1079 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:947)
05-15 01:33:17.047  1079  1079 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.047  1079  1079 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.047  1079  1079 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.047  1079  1079 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.047  1079  1079 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.048  1079  1079 D SystemServerTiming: MakeDisplayReady took to complete: 1ms
05-15 01:33:17.048  1079  1079 I SystemServer: StartStorageManagerService
05-15 01:33:17.048  1079  1079 I SystemServiceManager: Starting com.android.server.StorageManagerService$Lifecycle
05-15 01:33:17.049   733   733 W Binder:733_3: type=1400 audit(0.0:133): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:17.049   733   733 W Binder:733_5: type=1400 audit(0.0:136): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:17.051  1079  1079 D SystemServerTiming: StartStorageManagerService took to complete: 3ms
05-15 01:33:17.051  1079  1133 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:17.051  1079  1133 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:17.051  1079  1133 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:17.051  1079  1079 I SystemServer: StartStorageStatsService
05-15 01:33:17.051  1079  1133 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:17.051  1079  1079 I SystemServiceManager: Starting com.android.server.usage.StorageStatsService$Lifecycle
05-15 01:33:17.051  1079  1133 D CryptdConnector: SND -> {1 cryptfs getfield SystemLocale}
05-15 01:33:17.054  1079  1135 D CryptdConnector: RCV <- {200 1 -1}
05-15 01:33:17.055  1079  1133 W StorageManagerService: No primary storage mounted!
05-15 01:33:17.055  1079  1133 D VoldConnector: SND -> {1 asec list}
05-15 01:33:17.055  1079  1134 D VoldConnector: RCV <- {200 1 asec operation succeeded}
05-15 01:33:17.055  1079  1133 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:17.056  1079  1079 D SystemServerTiming: StartStorageStatsService took to complete: 5ms
05-15 01:33:17.056  1079  1079 I SystemServer: StartUiModeManager
05-15 01:33:17.056  1079  1079 I SystemServiceManager: Starting com.android.server.UiModeManagerService
05-15 01:33:17.057  1079  1092 D SystemServerInitThreadPool: Started executing UiModeManager.onStart
05-15 01:33:17.057  1079  1079 D SystemServerTiming: StartUiModeManager took to complete: 1ms
05-15 01:33:17.057  1079  1079 I SystemServer: UpdatePackagesIfNeeded
05-15 01:33:17.057  1079  1079 D SystemServerTiming: UpdatePackagesIfNeeded took to complete: 0ms
05-15 01:33:17.057  1079  1079 I SystemServer: PerformFstrimIfNeeded
05-15 01:33:17.057  1079  1079 D SystemServerTiming: PerformFstrimIfNeeded took to complete: 0ms
05-15 01:33:17.057  1079  1079 I SystemServer: StartLockSettingsService
05-15 01:33:17.058  1079  1079 I SystemServiceManager: Starting com.android.server.locksettings.LockSettingsService$Lifecycle
05-15 01:33:17.058  1079  1092 I ActivityManager: Config changes=200 {1.0 ?mcc?mnc [en_US] ldltr ?swdp ?wdp ?hdp ?density ?lsize ?long ?ldr ?wideColorGamut ?orien ?touch ?keyb/?/? ?nav/? s.2}
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: Failure in UiModeManager.onStart: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityStackSupervisor.getDisplayOverrideConfiguration(ActivityStackSupervisor.java:488)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.performDisplayOverrideConfigUpdate(ActivityManagerService.java:20762)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateGlobalConfiguration(ActivityManagerService.java:20669)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfigurationLocked(ActivityManagerService.java:20547)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfiguration(ActivityManagerService.java:20486)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.sendConfigurationLocked(UiModeManagerService.java:478)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.lambda$-com_android_server_UiModeManagerService_9177(UiModeManagerService.java:236)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.$m$4(Unknown Source:4)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.run(Unknown Source:27)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.SystemServerInitThreadPool.lambda$-com_android_server_SystemServerInitThreadPool_2249(SystemServerInitThreadPool.java:64)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.$m$2(Unknown Source:8)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.run(Unknown Source:19)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:457)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1162)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:636)
05-15 01:33:17.067  1079  1092 E SystemServerInitThreadPool: 	at com.android.internal.util.ConcurrentUtils$1$1.run(ConcurrentUtils.java:59)
05-15 01:33:17.068  1079  1079 D SystemServerTiming: StartLockSettingsService took to complete: 11ms
05-15 01:33:17.069  1079  1079 I OemLock : OemLock HAL not present on device
05-15 01:33:17.069  1079  1079 I SystemServer: StartDeviceIdleController
05-15 01:33:17.069  1079  1079 I SystemServiceManager: Starting com.android.server.DeviceIdleController
05-15 01:33:17.078  1079  1133 W StorageManagerService: No primary storage mounted!
05-15 01:33:17.078  1079  1133 D VoldConnector: SND -> {2 asec list}
05-15 01:33:17.079  1079  1134 D VoldConnector: RCV <- {200 2 asec operation succeeded}
05-15 01:33:17.079  1079  1079 D SystemServerTiming: StartDeviceIdleController took to complete: 10ms
05-15 01:33:17.079  1079  1079 I SystemServer: StartDevicePolicyManager
05-15 01:33:17.079  1079  1079 I SystemServiceManager: Starting com.android.server.devicepolicy.DevicePolicyManagerService$Lifecycle
05-15 01:33:17.079  1079  1093 I UsageStatsService: User[0] Rollover scheduled @ 2018-05-16 01:33:17(1526434397058)
05-15 01:33:17.080  1079  1093 E AppIdleHistory: Unable to read app idle file for user 0
05-15 01:33:17.082  1079  1079 D SystemServerTiming: StartDevicePolicyManager took to complete: 3ms
05-15 01:33:17.082  1079  1079 I SystemServer: StartStatusBarManagerService
05-15 01:33:17.083  1079  1079 D SystemServerTiming: StartStatusBarManagerService took to complete: 1ms
05-15 01:33:17.083  1079  1079 I SystemServer: StartClipboardService
05-15 01:33:17.084  1079  1079 I SystemServiceManager: Starting com.android.server.clipboard.ClipboardService
05-15 01:33:17.084  1079  1079 D SystemServerTiming: StartClipboardService took to complete: 1ms
05-15 01:33:17.084  1079  1079 I SystemServer: StartNetworkManagementService
05-15 01:33:17.086  1079  1141 I NetworkManagement: onDaemonConnected()
05-15 01:33:17.087  1079  1079 D SystemServerTiming: StartNetworkManagementService took to complete: 2ms
05-15 01:33:17.087  1079  1079 I SystemServer: StartTextServicesManager
05-15 01:33:17.087  1079  1079 I SystemServiceManager: Starting com.android.server.TextServicesManagerService$Lifecycle
05-15 01:33:17.091  1079  1079 D SystemServerTiming: StartTextServicesManager took to complete: 4ms
05-15 01:33:17.091  1079  1079 I SystemServer: StartNetworkScoreService
05-15 01:33:17.091  1079  1079 D SystemServerTiming: StartNetworkScoreService took to complete: 0ms
05-15 01:33:17.092  1079  1079 I SystemServer: StartNetworkStatsService
05-15 01:33:17.095  1079  1079 W SystemServer: ***********************************************
05-15 01:33:17.095  1079  1079 E SystemServer: BOOT FAILURE starting NetworkStats Service
05-15 01:33:17.095  1079  1079 E SystemServer: java.lang.NullPointerException: missing AlarmManager
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.server.net.NetworkStatsService.<init>(NetworkStatsService.java:309)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:289)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.095  1079  1079 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.095  1079  1079 D SystemServerTiming: StartNetworkStatsService took to complete: 4ms
05-15 01:33:17.095  1079  1079 I SystemServer: StartNetworkPolicyManagerService
05-15 01:33:17.097  1079  1079 W SystemServer: ***********************************************
05-15 01:33:17.097  1079  1079 E SystemServer: BOOT FAILURE starting NetworkPolicy Service
05-15 01:33:17.097  1079  1079 E SystemServer: java.lang.NullPointerException: missing networkStats
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:501)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:487)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1096)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.097  1079  1079 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.097  1079  1079 D SystemServerTiming: StartNetworkPolicyManagerService took to complete: 2ms
05-15 01:33:17.097  1079  1079 I SystemServer: StartWifi
05-15 01:33:17.098  1079  1079 I SystemServiceManager: Starting com.android.server.wifi.WifiService
05-15 01:33:17.101  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-8 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.101  1124  1124 D SensorHub: Channel activate-> handle: 8, enabled:0, err: 0
05-15 01:33:17.101  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-11 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.101  1124  1124 D SensorHub: Channel activate-> handle: 11, enabled:0, err: 0
05-15 01:33:17.101  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-12 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.101  1124  1124 D SensorHub: Channel activate-> handle: 12, enabled:0, err: 0
05-15 01:33:17.101  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-13 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.101  1124  1124 D SensorHub: Channel activate-> handle: 13, enabled:0, err: 0
05-15 01:33:17.101  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-14 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.101  1124  1124 D SensorHub: Channel activate-> handle: 14, enabled:0, err: 0
05-15 01:33:17.102  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-15 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.102  1124  1124 D SensorHub: Channel activate-> handle: 15, enabled:0, err: 0
05-15 01:33:17.102  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-17 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.102  1124  1124 D SensorHub: Channel activate-> handle: 17, enabled:0, err: 0
05-15 01:33:17.102  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-18 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.102  1124  1124 D SensorHub: Channel activate-> handle: 18, enabled:0, err: 0
05-15 01:33:17.102  1124  1124 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-21 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:17.102  1124  1124 D SensorHub: Channel activate-> handle: 21, enabled:0, err: 0
05-15 01:33:17.103  1079  1151 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:17.103  1079  1123 D SystemServerTimingAsync: StartSensorService took to complete: 109ms
05-15 01:33:17.103  1079  1123 D SystemServerInitThreadPool: Finished executing StartSensorService
05-15 01:33:17.103  1079  1152 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:17.112  1079  1122 D SystemServerInitThreadPool: Finished executing Init OverlayManagerService
05-15 01:33:17.134  1079  1150 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:17.134  1040  1059 D CommandListener: Clearing all IP addresses on wlan0
05-15 01:33:17.140  1079  1079 D SystemServerTiming: StartWifi took to complete: 42ms
05-15 01:33:17.140  1079  1079 I SystemServer: StartWifiScanning
05-15 01:33:17.140  1079  1079 I SystemServiceManager: Starting com.android.server.wifi.scanner.WifiScanningService
05-15 01:33:17.142  1079  1079 D SystemServerTiming: StartWifiScanning took to complete: 3ms
05-15 01:33:17.142  1079  1079 I SystemServer: StartWifiRtt
05-15 01:33:17.142  1079  1079 I SystemServiceManager: Starting com.android.server.wifi.RttService
05-15 01:33:17.143  1079  1079 D SystemServerTiming: StartWifiRtt took to complete: 1ms
05-15 01:33:17.143  1079  1079 I SystemServer: No Wi-Fi Aware Service (Aware support Not Present)
05-15 01:33:17.143  1079  1079 I SystemServer: StartWifiP2P
05-15 01:33:17.143  1079  1079 I SystemServiceManager: Starting com.android.server.wifi.p2p.WifiP2pService
05-15 01:33:17.147  1079  1079 D SystemServerTiming: StartWifiP2P took to complete: 4ms
05-15 01:33:17.147  1079  1079 I SystemServer: StartEthernet
05-15 01:33:17.149  1079  1079 I SystemServiceManager: Starting com.android.server.ethernet.EthernetService
05-15 01:33:17.159  1079  1079 D SystemServerTiming: StartEthernet took to complete: 11ms
05-15 01:33:17.159  1079  1079 I SystemServer: StartConnectivityService
05-15 01:33:17.161  1079  1079 D ConnectivityService: ConnectivityService starting up
05-15 01:33:17.162  1079  1079 W SystemServer: ***********************************************
05-15 01:33:17.162  1079  1079 E SystemServer: BOOT FAILURE starting Connectivity Service
05-15 01:33:17.162  1079  1079 E SystemServer: java.lang.NullPointerException: missing INetworkStatsService
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:722)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:690)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1151)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.162  1079  1079 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.162  1079  1079 D SystemServerTiming: StartConnectivityService took to complete: 4ms
05-15 01:33:17.163  1079  1079 I SystemServer: StartNsdService
05-15 01:33:17.163  1079  1079 D NsdService: Network service discovery is enabled
05-15 01:33:17.164  1079  1079 D SystemServerTiming: StartNsdService took to complete: 2ms
05-15 01:33:17.164  1079  1079 I SystemServer: StartUpdateLockService
05-15 01:33:17.165  1079  1079 D SystemServerTiming: StartUpdateLockService took to complete: 1ms
05-15 01:33:17.165  1079  1079 I SystemServer: WaitForAsecScan
05-15 01:33:17.165  1079  1079 D SystemServerTiming: WaitForAsecScan took to complete: 0ms
05-15 01:33:17.165  1079  1079 I SystemServer: StartNotificationManager
05-15 01:33:17.166  1079  1079 I SystemServiceManager: Starting com.android.server.notification.NotificationManagerService
05-15 01:33:17.186  1079  1079 D ConditionProviders.SCP: new ScheduleConditionProvider()
05-15 01:33:17.187  1079  1079 I ConditionProviders:  Allowing condition provider org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:17.187  1079  1079 I NotificationListeners:  Allowing notification listener org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:17.187  1079  1079 I ConditionProviders:  Allowing condition provider com.android.camera2
05-15 01:33:17.187  1079  1079 D ZenLog  : set_zen_mode: off,init
05-15 01:33:17.190  1079  1079 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:17.191  1079  1119 D SystemServerTimingAsync: AppDataPrepare took to complete: 248ms
05-15 01:33:17.191  1079  1119 I PackageManager: Deferred reconcileAppsData finished 73 packages
05-15 01:33:17.191  1079  1119 D SystemServerInitThreadPool: Finished executing prepareAppData
05-15 01:33:17.195   746   968 I         : getTotalMemoryFromDDRInfo, buffer = 0x4ff
05-15 01:33:17.195   746   968 I         : , len = 6
05-15 01:33:17.195   746   968 I         : [getTotalMemoryFromDDRInfo] total memory =4194304KB
05-15 01:33:17.196   526   526 D lights  : set_light_notification colorRGB=00000000, onMS=0, offMS=0
05-15 01:33:17.199  1079  1079 E System  : ******************************************
05-15 01:33:17.199  1079  1079 E System  : ************ Failure starting system services
05-15 01:33:17.199  1079  1079 E System  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:17.199  1079  1079 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:17.199  1079  1079 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.199  1079  1079 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.199  1079  1079 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.199  1079  1079 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.199  1079  1079 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.199  1079  1079 D SystemServerTiming: StartNotificationManager took to complete: 34ms
05-15 01:33:17.199  1079  1079 D AndroidRuntime: Shutting down VM
05-15 01:33:17.199  1079  1079 E AndroidRuntime: *** FATAL EXCEPTION IN SYSTEM PROCESS: main
05-15 01:33:17.199  1079  1079 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:17.199  1079  1079 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:17.200  1079  1079 I Process : Sending signal. PID: 1079 SIG: 9
05-15 01:33:17.200   746   968 I         : HwCamMem mempoolcfg dumpMemInfo Free=3332860, Total=4194304, Pss=11196 mTimeOutCount=1
05-15 01:33:17.200   746   968 I         : HwCamMem checkMemPool dumpMemInfo CHECK_INTERVAL:5000 ms, passTime:14458 ms
05-15 01:33:17.232   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:17.232   346   346 E         : 
05-15 01:33:17.236   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:17.236   346   346 E         : 
05-15 01:33:17.236   511  1165 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 4 lines
05-15 01:33:17.236   511  1166 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 2 lines
05-15 01:33:17.239  1037  1169 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 3 lines
05-15 01:33:17.241  1037  1171 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:17.242   536   536 I lowmemorykiller: ActivityManager disconnected
05-15 01:33:17.242   536   536 I lowmemorykiller: Closing Activity Manager data connection
05-15 01:33:17.243  1037  1173 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:17.243  1036  1036 E Zygote  : Exit zygote because system server (1079) has terminated
05-15 01:33:17.243  1036  1036 F libc    : Fatal signal 6 (SIGABRT), code 0 in tid 1036 (main), pid 1036 (main)
05-15 01:33:17.243  1037  1176 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:17.248  1037  1181 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:17.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:17.263  1183  1183 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-15 01:33:17.264   751   751 I /system/bin/tombstoned: received crash request for pid 1036
05-15 01:33:17.264  1183  1183 I crash_dump64: performing dump of process 1036 (target tid = 1036)
05-15 01:33:17.264  1036  1036 F libc    : failed to wait for crash_dump helper: No child processes
05-15 01:33:17.264  1183  1183 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-15 01:33:17.264  1183  1183 F DEBUG   : LineageOS Version: 'unknown'
05-15 01:33:17.264  1183  1183 F DEBUG   : Build fingerprint: 'Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys'
05-15 01:33:17.264  1183  1183 F DEBUG   : Revision: '0'
05-15 01:33:17.264  1183  1183 F DEBUG   : ABI: 'arm64'
05-15 01:33:17.264  1183  1183 F DEBUG   : pid: 1036, tid: 1036, name: main  >>> zygote64 <<<
05-15 01:33:17.264  1183  1183 F DEBUG   : signal 6 (SIGABRT), code 0 (SI_USER), fault addr --------
05-15 01:33:17.264  1183  1183 F DEBUG   :     x0   0000000000000000  x1   0000000000000009  x2   0000000000000005  x3   0000000000000003
05-15 01:33:17.264  1183  1183 F DEBUG   :     x4   0000000040100401  x5   a802a00080404000  x6   0000000000000000  x7   7f7f7f7f7f7f7f7f
05-15 01:33:17.264  1183  1183 F DEBUG   :     x8   0000000000000081  x9   7533f1ba8706b887  x10  0000007fda8071c0  x11  0000000000000038
05-15 01:33:17.264  1183  1183 F DEBUG   :     x12  000000000000000b  x13  ffffffffffffffff  x14  ff00000000000000  x15  ffffffffffffffff
05-15 01:33:17.264  1183  1183 F DEBUG   :     x16  0000007f4cea8300  x17  0000007f4c08455c  x18  0000000070215150  x19  0000007f4f345a50
05-15 01:33:17.264  1183  1183 F DEBUG   :     x20  0000007f4ce541e6  x21  0000007f4ce5464a  x22  0000007f4ce546a6  x23  0000000000000437
05-15 01:33:17.264  1183  1183 F DEBUG   :     x24  0000007f4ce5468e  x25  0000007f4ce54669  x26  0000007f4f345a40  x27  0000000000000002
05-15 01:33:17.264  1183  1183 F DEBUG   :     x28  0000007f4cead000  x29  0000007fda807790  x30  0000007f4ce0e00c
05-15 01:33:17.264  1183  1183 F DEBUG   :     sp   0000007fda807730  pc   0000007f4c084564  pstate 0000000060000000
05-15 01:33:17.500  1183  1183 F DEBUG   : 
05-15 01:33:17.500  1183  1183 F DEBUG   : backtrace:
05-15 01:33:17.500  1183  1183 F DEBUG   :     #00 pc 000000000006a564  /system/lib64/libc.so (kill+8)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #01 pc 0000000000176008  /system/lib64/libandroid_runtime.so ((anonymous namespace)::SigChldHandler(int)+280)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #02 pc 00000000000005f0  [vdso:0000007f4f1da000]
05-15 01:33:17.500  1183  1183 F DEBUG   :     #03 pc 0000000000069ea0  /system/lib64/libc.so (__ppoll+4)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #04 pc 00000000000265e4  /system/lib64/libc.so (poll+88)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #05 pc 000000000002e9a8  /system/lib64/libjavacore.so (Linux_poll(_JNIEnv*, _jobject*, _jobjectArray*, int)+800)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #06 pc 000000000030bad0  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.Linux.fcntlVoid [DEDUPED]+160)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #07 pc 0000000000300a74  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.BlockGuardOs.poll+228)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #08 pc 00000000002b67a4  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (android.system.Os.poll+84)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #09 pc 000000000164e488  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteServer.runSelectLoop+664)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #10 pc 0000000001652ed8  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteInit.main+2728)
05-15 01:33:17.500  1183  1183 F DEBUG   :     #11 pc 000000000054744c  /system/lib64/libart.so (art_quick_invoke_static_stub+604)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #12 pc 00000000000dc7b0  /system/lib64/libart.so (art::ArtMethod::Invoke(art::Thread*, unsigned int*, unsigned int, art::JValue*, char const*)+260)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #13 pc 000000000046bb70  /system/lib64/libart.so (art::InvokeWithArgArray(art::ScopedObjectAccessAlreadyRunnable const&, art::ArtMethod*, art::ArgArray*, art::JValue*, char const*)+100)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #14 pc 000000000046b79c  /system/lib64/libart.so (art::InvokeWithVarArgs(art::ScopedObjectAccessAlreadyRunnable const&, _jobject*, _jmethodID*, std::__va_list)+420)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #15 pc 0000000000372a54  /system/lib64/libart.so (art::JNI::CallStaticVoidMethodV(_JNIEnv*, _jclass*, _jmethodID*, std::__va_list)+620)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #16 pc 00000000000a6fb8  /system/lib64/libandroid_runtime.so (_JNIEnv::CallStaticVoidMethod(_jclass*, _jmethodID*, ...)+120)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #17 pc 00000000000a9728  /system/lib64/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+832)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #18 pc 0000000000002440  /system/bin/app_process64 (main+1328)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #19 pc 00000000000a14d4  /system/lib64/libc.so (__libc_init+88)
05-15 01:33:17.501  1183  1183 F DEBUG   :     #20 pc 0000000000001e70  /system/bin/app_process64 (_start_main+80)
05-15 01:33:17.632  1183  1183 E crash_dump64: unable to connect to activity manager: No such file or directory
05-15 01:33:17.632   751   751 E /system/bin/tombstoned: Tombstone written to: /data/tombstones/tombstone_09
05-15 01:33:18.258   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:19.030  1192  1192 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:19.031  1191  1191 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:19.032  1191  1191 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:19.032  1191  1191 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:19.032  1191  1191 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:19.033  1192  1192 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:19.034  1192  1192 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:19.259   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:20.259   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:21.160  1202  1202 I Netd    : Netd 1.0 starting
05-15 01:33:21.160  1202  1202 D TetherController: Setting IP forward enable = 0
05-15 01:33:21.168  1203  1203 I wificond: wificond is starting up...
05-15 01:33:21.180   385   385 I chatty  : uid=1000(system) hwservicemanage expire 11 lines
05-15 01:33:21.182  1204  1204 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:21.182  1204  1204 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:21.182  1204  1204 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:21.182  1204  1204 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:21.182  1204  1204 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:21.185  1204  1204 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:21.185  1204  1204 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:21.185  1204  1204 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:21.190  1202  1202 I Netd    : Creating child chains: 26.7ms
05-15 01:33:21.190  1202  1202 I Netd    : Setting up OEM hooks: 0.1ms
05-15 01:33:21.193  1202  1202 I Netd    : Setting up FirewallController hooks: 3.3ms
05-15 01:33:21.195  1202  1202 I Netd    : Setting up NatController hooks: 2.0ms
05-15 01:33:21.197  1202  1202 I Netd    : Setting up BandwidthController hooks: 1.6ms
05-15 01:33:21.197  1202  1202 I Netd    : Setting up IdletimerController hooks: 0.1ms
05-15 01:33:21.201  1202  1202 I Netd    : Disabling bandwidth control: 4.1ms
05-15 01:33:21.203  1202  1202 E Netd    : cannot find interface dummy0
05-15 01:33:21.203  1202  1202 I Netd    : Initializing RouteController: 1.9ms
05-15 01:33:21.203  1202  1202 E Netd    : Unable to create netlink socket: Protocol not supported
05-15 01:33:21.203  1202  1202 W Netd    : Unable to open qlog quota socket, check if xt_quota2 can send via UeventHandler
05-15 01:33:21.204  1202  1202 D MDnsDS  : MDnsSdListener::Hander starting up
05-15 01:33:21.205  1202  1215 D MDnsDS  : MDnsSdListener starting to monitor
05-15 01:33:21.205  1202  1215 D MDnsDS  : Going to poll with pollCount 1
05-15 01:33:21.206  1202  1202 I Netd    : Registering NetdNativeService: 1.0ms
05-15 01:33:21.206  1202  1202 I Netd    : Starting CommandListener: 0.1ms
05-15 01:33:21.207  1202  1202 I Netd    : Registering NetdHwService: 1.4ms
05-15 01:33:21.207  1202  1202 I Netd    : Netd started in 47ms
05-15 01:33:21.226  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 5 lines
05-15 01:33:21.229  1200  1200 W cameraserver: type=1400 audit(0.0:137): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2092 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:21.229  1200  1200 W cameraserver: type=1400 audit(0.0:138): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2295 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:21.233  1200  1200 I cameraserver: ServiceManager: 0xec7179a0
05-15 01:33:21.233  1200  1200 I CameraService: CameraService started (pid=1200)
05-15 01:33:21.233  1200  1200 I CameraService: CameraService process starting
05-15 01:33:21.233  1200  1200 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:21.234  1200  1200 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:21.236  1200  1200 E vndksupport: Could not load /vendor/lib/hw/android.hardware.camera.provider@2.4-impl.so from sphal namespace: dlopen failed: library "android.hardware.camera.device@1.0.so" not found.
05-15 01:33:21.236  1200  1200 E /system/bin/cameraserver: Failed to dlopen android.hardware.camera.provider@2.4-impl.so: unknown error
05-15 01:33:21.259   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:21.261  1201  1201 I mediaserver: ServiceManager: 0xed917a40
05-15 01:33:21.261   346   346 E         : pid 511, opration oeminfo_read OK
05-15 01:33:21.261   346   346 E         : 
05-15 01:33:21.261  1201  1201 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:21.263   511  1233 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 1 line
05-15 01:33:21.292  1198  1198 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:21.295  1198  1198 I zygote64: option[0]=-Xzygote
05-15 01:33:21.295  1198  1198 I zygote64: option[1]=-Xusetombstonedtraces
05-15 01:33:21.295  1198  1198 I zygote64: option[2]=exit
05-15 01:33:21.295  1198  1198 I zygote64: option[3]=vfprintf
05-15 01:33:21.295  1198  1198 I zygote64: option[4]=sensitiveThread
05-15 01:33:21.295  1198  1198 I zygote64: option[5]=-verbose:gc
05-15 01:33:21.295  1198  1198 I zygote64: option[6]=-Xms8m
05-15 01:33:21.295  1198  1198 I zygote64: option[7]=-Xmx512m
05-15 01:33:21.295  1198  1198 I zygote64: option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:21.295  1198  1198 I zygote64: option[9]=-XX:HeapMinFree=2m
05-15 01:33:21.295  1198  1198 I zygote64: option[10]=-XX:HeapMaxFree=8m
05-15 01:33:21.295  1198  1198 I zygote64: option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:21.295  1198  1198 I zygote64: option[12]=-Xusejit:true
05-15 01:33:21.295  1198  1198 I zygote64: option[13]=-Xjitsaveprofilinginfo
05-15 01:33:21.295  1198  1198 I zygote64: option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:21.295  1198  1198 I zygote64: option[15]=-Xlockprofthreshold:500
05-15 01:33:21.296  1198  1198 I zygote64: option[16]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[17]=--runtime-arg
05-15 01:33:21.296  1198  1198 I zygote64: option[18]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[19]=-Xms64m
05-15 01:33:21.296  1198  1198 I zygote64: option[20]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[21]=--runtime-arg
05-15 01:33:21.296  1198  1198 I zygote64: option[22]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[23]=-Xmx64m
05-15 01:33:21.296  1198  1198 I zygote64: option[24]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:21.296  1198  1198 I zygote64: option[26]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:21.296  1198  1198 I zygote64: option[28]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:21.296  1198  1198 I zygote64: option[30]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[31]=--runtime-arg
05-15 01:33:21.296  1198  1198 I zygote64: option[32]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[33]=-Xms64m
05-15 01:33:21.296  1198  1198 I zygote64: option[34]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[35]=--runtime-arg
05-15 01:33:21.296  1198  1198 I zygote64: option[36]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[37]=-Xmx512m
05-15 01:33:21.296  1198  1198 I zygote64: option[38]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[39]=-j4
05-15 01:33:21.296  1198  1198 I zygote64: option[40]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[41]=-j4
05-15 01:33:21.296  1198  1198 I zygote64: option[42]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[43]=--instruction-set-variant=generic
05-15 01:33:21.296  1198  1198 I zygote64: option[44]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[45]=--instruction-set-variant=generic
05-15 01:33:21.296  1198  1198 I zygote64: option[46]=-Ximage-compiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[47]=--instruction-set-features=default
05-15 01:33:21.296  1198  1198 I zygote64: option[48]=-Xcompiler-option
05-15 01:33:21.296  1198  1198 I zygote64: option[49]=--instruction-set-features=default
05-15 01:33:21.296  1198  1198 I zygote64: option[50]=-Duser.locale=en-US
05-15 01:33:21.296  1198  1198 I zygote64: option[51]=--cpu-abilist=arm64-v8a
05-15 01:33:21.296  1198  1198 I zygote64: option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:21.357   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 72 lines
05-15 01:33:21.387  1198  1198 D Zygote  : begin preload
05-15 01:33:21.387  1198  1198 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:21.387  1198  1198 I Zygote  : Preloading ICU data...
05-15 01:33:21.391  1198  1198 D Zygote64Timing: BeginIcuCachePinning took to complete: 4ms
05-15 01:33:21.391  1198  1198 I Zygote  : Preloading classes...
05-15 01:33:21.409  1249  1249 W rild    : type=1400 audit(0.0:139): avc: denied { execute_no_trans } for path="/vendor/bin/sh" dev="mmcblk0p55" ino=230 scontext=u:r:rild:s0 tcontext=u:object_r:vendor_shell_exec:s0 tclass=file permissive=0
05-15 01:33:21.460  1198  1198 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:21.465  1198  1198 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:21.469  1198  1198 I zygote64: Thread[1,tid=1198,Native,Thread*=0x77c48bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:21.469  1198  1198 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:21.469  1198  1198 I zygote64: Thread[1,tid=1198,Native,Thread*=0x77c48bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:21.470  1198  1198 I zygote64: Thread[1,tid=1198,Native,Thread*=0x77c48bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:21.504  1198  1198 I Zygote  : ...preloaded 4715 classes in 113ms.
05-15 01:33:21.504  1198  1198 I zygote64: VMRuntime.preloadDexCaches starting
05-15 01:33:21.532  1198  1198 I zygote64: VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:21.532  1198  1198 I zygote64: VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:21.532  1198  1198 I zygote64: VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:21.532  1198  1198 I zygote64: VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:21.532  1198  1198 I zygote64: VMRuntime.preloadDexCaches finished
05-15 01:33:21.532  1198  1198 D Zygote64Timing: PreloadClasses took to complete: 141ms
05-15 01:33:21.547  1198  1198 I Zygote  : Preloading resources...
05-15 01:33:21.551  1198  1198 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:21.559  1198  1198 I Zygote  : ...preloaded 64 resources in 12ms.
05-15 01:33:21.561  1198  1198 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:21.561  1198  1198 I Zygote  : ...preloaded 41 resources in 2ms.
05-15 01:33:21.561  1198  1198 D Zygote64Timing: PreloadResources took to complete: 29ms
05-15 01:33:21.577  1198  1198 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:21.587  1198  1198 I Zygote  : Preloading shared libraries...
05-15 01:33:21.593  1198  1198 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:21.594  1198  1198 I Zygote  : Installed AndroidKeyStoreProvider in 0ms.
05-15 01:33:21.598  1198  1198 I Zygote  : Warmed up JCA providers in 4ms.
05-15 01:33:21.598  1198  1198 D Zygote  : end preload
05-15 01:33:21.598  1198  1198 D Zygote64Timing: ZygotePreload took to complete: 211ms
05-15 01:33:21.607  1198  1198 I zygote64: Explicit concurrent copying GC freed 29303(2MB) AllocSpace objects, 25(476KB) LOS objects, 80% free, 1524KB/7MB, paused 30us total 9.385ms
05-15 01:33:21.615  1198  1198 I zygote64: Explicit concurrent copying GC freed 5435(198KB) AllocSpace objects, 0(0B) LOS objects, 81% free, 1357KB/7MB, paused 20us total 5.959ms
05-15 01:33:21.615  1198  1198 D Zygote64Timing: PostZygoteInitGC took to complete: 17ms
05-15 01:33:21.615  1198  1198 D Zygote64Timing: ZygoteInit took to complete: 228ms
05-15 01:33:21.672  1198  1198 I zygote64: Global filter of size 170 installed
05-15 01:33:21.693  1198  1198 I Zygote  : System server process 1252 has been created
05-15 01:33:21.693  1198  1198 E Zygote  : couldn't write 1252 to /dev/memcg/system/tasks
05-15 01:33:21.695  1198  1198 I Zygote  : Accepting command socket connections
05-15 01:33:21.709  1252  1252 I chatty  : uid=1000 system_server expire 145 lines
05-15 01:33:21.724  1252  1252 I SystemServer: InitBeforeStartServices
05-15 01:33:21.724  1252  1252 I SystemServer: Entered the Android system server!
05-15 01:33:21.789   733   733 W Binder:733_2: type=1400 audit(0.0:140): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:21.789   733   733 W Binder:733_2: type=1400 audit(0.0:141): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:21.793  1252  1252 D SystemServerTiming: InitBeforeStartServices took to complete: 69ms
05-15 01:33:21.793  1252  1252 I SystemServer: StartServices
05-15 01:33:21.793  1252  1252 I SystemServer: Reading configuration...
05-15 01:33:21.793  1252  1252 I SystemServer: ReadingSystemConfig
05-15 01:33:21.793  1252  1252 D SystemServerTiming: ReadingSystemConfig took to complete: 0ms
05-15 01:33:21.793  1252  1252 I SystemServer: StartInstaller
05-15 01:33:21.793  1252  1252 I SystemServiceManager: Starting com.android.server.pm.Installer
05-15 01:33:21.793  1252  1265 D SystemServerInitThreadPool: Started executing ReadingSystemConfig
05-15 01:33:21.795  1252  1252 D SystemServerTiming: StartInstaller took to complete: 1ms
05-15 01:33:21.795  1252  1252 I SystemServer: DeviceIdentifiersPolicyService
05-15 01:33:21.795  1252  1252 I SystemServiceManager: Starting com.android.server.os.DeviceIdentifiersPolicyService
05-15 01:33:21.795  1252  1252 D SystemServerTiming: DeviceIdentifiersPolicyService took to complete: 0ms
05-15 01:33:21.795  1252  1252 I SystemServer: StartActivityManager
05-15 01:33:21.795  1252  1252 I SystemServiceManager: Starting com.android.server.am.ActivityManagerService$Lifecycle
05-15 01:33:21.802  1252  1265 D SystemServerInitThreadPool: Finished executing ReadingSystemConfig
05-15 01:33:21.803  1252  1252 I ActivityManager: Memory class: 384
05-15 01:33:21.803  1252  1267 I ServiceThread: Enabled StrictMode logging for ActivityManager looper.
05-15 01:33:21.804  1252  1268 I ServiceThread: Enabled StrictMode logging for android.ui looper.
05-15 01:33:21.811  1252  1252 D BatteryStatsImpl: Reading daily items from /data/system/batterystats-daily.xml
05-15 01:33:21.813  1252  1270 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:21.814  1252  1270 E BatteryExternalStatsWorker: no controller energy info supplied for telephony
05-15 01:33:21.815  1252  1270 E KernelUidCpuFreqTimeReader: Failed to read /proc/uid_time_in_state: java.io.FileNotFoundException: /proc/uid_time_in_state (No such file or directory)
05-15 01:33:21.847  1252  1252 I AppOps  : No existing app ops /data/system/appops.xml; starting empty
05-15 01:33:21.848  1252  1252 I IntentFirewall: Read new rules (A:0 B:0 S:0)
05-15 01:33:21.849  1252  1274 I ServiceThread: Enabled StrictMode logging for android.display looper.
05-15 01:33:21.853  1252  1252 D AppOps  : AppOpsService published
05-15 01:33:21.853  1252  1252 D SystemServerTiming: StartActivityManager took to complete: 58ms
05-15 01:33:21.853  1252  1252 I SystemServer: StartPowerManager
05-15 01:33:21.853  1252  1252 I SystemServiceManager: Starting com.android.server.power.PowerManagerService
05-15 01:33:21.854  1252  1276 I ServiceThread: Enabled StrictMode logging for PowerManagerService looper.
05-15 01:33:21.855  1252  1252 D SystemServerTiming: StartPowerManager took to complete: 2ms
05-15 01:33:21.855  1252  1252 I SystemServer: InitPowerManagement
05-15 01:33:21.855  1252  1252 D SystemServerTiming: InitPowerManagement took to complete: 0ms
05-15 01:33:21.856  1252  1252 I SystemServer: StartRecoverySystemService
05-15 01:33:21.856  1252  1252 I SystemServiceManager: Starting com.android.server.RecoverySystemService
05-15 01:33:21.856  1252  1252 D SystemServerTiming: StartRecoverySystemService took to complete: 1ms
05-15 01:33:21.856  1252  1252 V RescueParty: Disabled because of active USB connection
05-15 01:33:21.856  1252  1252 I SystemServer: StartLightsService
05-15 01:33:21.856  1252  1252 I SystemServiceManager: Starting com.android.server.lights.LightsService
05-15 01:33:21.856  1252  1252 D SystemServerTiming: StartLightsService took to complete: 0ms
05-15 01:33:21.856  1252  1252 I SystemServer: StartDisplayManager
05-15 01:33:21.856  1252  1252 I SystemServiceManager: Starting com.android.server.display.DisplayManagerService
05-15 01:33:21.857  1252  1252 D SystemServerTiming: StartDisplayManager took to complete: 1ms
05-15 01:33:21.857  1252  1252 I SystemServer: WaitForDisplay
05-15 01:33:21.857  1252  1252 I SystemServiceManager: Starting phase 100
05-15 01:33:21.859  1252  1274 I DisplayManagerService: Display device added: DisplayDeviceInfo{"Built-in Screen": uniqueId="local:0", 1080 x 1920, modeId 1, defaultModeId 1, supportedModes [{id=1, width=1080, height=1920, fps=60.000004}], colorMode 0, supportedColorModes [0], HdrCapabilities android.view.Display$HdrCapabilities@1d6308, density 480, 365.76 x 366.676 dpi, appVsyncOff 2000000, presDeadline 13666666, touch INTERNAL, rotation 0, type BUILT_IN, state UNKNOWN, FLAG_DEFAULT_DISPLAY, FLAG_ROTATES_WITH_CONTENT, FLAG_SECURE, FLAG_SUPPORTS_PROTECTED_BUFFERS}
05-15 01:33:21.860   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:21.861  1252  1252 D SystemServerTiming: WaitForDisplay took to complete: 4ms
05-15 01:33:21.861  1252  1274 I DisplayManagerService: Display device changed state: "Built-in Screen", ON
05-15 01:33:21.861  1252  1252 I SystemServer: StartPackageManagerService
05-15 01:33:21.866  1252  1252 D SELinuxMMAC: Using policy file /system/etc/selinux/plat_mac_permissions.xml
05-15 01:33:21.866  1252  1252 D SELinuxMMAC: Using policy file /vendor/etc/selinux/nonplat_mac_permissions.xml
05-15 01:33:21.896  1252  1252 W PackageManager: Failed to parse /system/framework/arm: Missing base APK in /system/framework/arm
05-15 01:33:21.897  1252  1252 W PackageManager: Failed to parse /system/framework/arm64: Missing base APK in /system/framework/arm64
05-15 01:33:21.897  1252  1252 W PackageManager: Failed to parse /system/framework/oat: Missing base APK in /system/framework/oat
05-15 01:33:21.947  1252  1252 I PackageManager: Finished scanning system apps. Time: 53 ms, packageCount: 94 , timePerPackage: 0 , cached: 94
05-15 01:33:21.947  1252  1252 I PackageManager: Finished scanning non-system apps. Time: 0 ms, packageCount: 0 , timePerPackage: 0 , cached: 0
05-15 01:33:21.948  1252  1252 I PackageManager: Time to scan packages: 0.054 seconds
05-15 01:33:21.949  1252  1252 V PackageManager: reconcileAppsData for null u0 0x3 migrateAppData=true
05-15 01:33:21.977  1252  1252 V PackageManager: reconcileAppsData finished 21 packages
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:21.977  1252  1292 D SystemServerInitThreadPool: Started executing prepareAppData
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:21.977  1252  1252 V PackageManager: Disabling com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:21.977  1252  1252 W PackageManager: Unable to disable com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:21.977  1252  1252 V PackageManager: Enabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:21.978  1252  1252 W PackageManager: Unable to enable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:21.978  1252  1252 V PackageManager: Enabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:21.978  1252  1252 W PackageManager: Unable to enable com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:21.979   733   733 W installd: Ignoring /data/data/com.android.webview/lib with unexpected GID 0 instead of 10038
05-15 01:33:21.979   733   733 W installd: Ignoring /data/data/com.svox.pico/lib with unexpected GID 0 instead of 10045
05-15 01:33:21.981  1252  1292 D SystemServerTimingAsync: AppDataFixup took to complete: 4ms
05-15 01:33:22.001  1252  1252 D PackageManager: Ephemeral resolver not found with new action; try old one
05-15 01:33:22.001  1252  1252 D PackageManager: Ephemeral resolver NOT found; no matching intent filters
05-15 01:33:22.001  1252  1252 D PackageManager: Ephemeral installer not found with new action; try old one
05-15 01:33:22.002  1252  1252 D PackageManager: Clear ephemeral installer activity
05-15 01:33:22.027  1252  1252 D SystemServerTiming: StartPackageManagerService took to complete: 166ms
05-15 01:33:22.027  1252  1252 I SystemServer: StartOtaDexOptService
05-15 01:33:22.028  1252  1252 D OTADexopt: No upgrade, skipping A/B artifacts check.
05-15 01:33:22.028  1252  1252 D SystemServerTiming: StartOtaDexOptService took to complete: 0ms
05-15 01:33:22.028  1252  1252 I SystemServer: StartUserManagerService
05-15 01:33:22.028  1252  1252 I SystemServiceManager: Starting com.android.server.pm.UserManagerService$LifeCycle
05-15 01:33:22.028  1252  1252 D SystemServerTiming: StartUserManagerService took to complete: 1ms
05-15 01:33:22.028  1252  1252 I SystemServer: InitAttributerCache
05-15 01:33:22.028  1252  1252 D SystemServerTiming: InitAttributerCache took to complete: 0ms
05-15 01:33:22.028  1252  1252 I SystemServer: SetSystemProcess
05-15 01:33:22.032   536   536 I lowmemorykiller: ActivityManager connected
05-15 01:33:22.032  1252  1252 D SystemServerTiming: SetSystemProcess took to complete: 4ms
05-15 01:33:22.033  1252  1294 I ServiceThread: Enabled StrictMode logging for android.anim looper.
05-15 01:33:22.033  1252  1252 I SystemServer: StartOverlayManagerService
05-15 01:33:22.034  1252  1252 I SystemServer: StartSubstratumService
05-15 01:33:22.034  1252  1295 D SystemServerInitThreadPool: Started executing Init OverlayManagerService
05-15 01:33:22.035  1252  1252 D SystemServerTiming: StartSubstratumService took to complete: 1ms
05-15 01:33:22.035  1252  1252 I SystemServer: StartDropBoxManager
05-15 01:33:22.035  1252  1252 I SystemServiceManager: Starting com.android.server.DropBoxManagerService
05-15 01:33:22.035  1252  1296 D SystemServerInitThreadPool: Started executing StartSensorService
05-15 01:33:22.035  1252  1296 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:22.037  1252  1252 D SystemServerTiming: StartDropBoxManager took to complete: 1ms
05-15 01:33:22.037  1252  1252 I SystemServer: StartBatteryService
05-15 01:33:22.037  1252  1252 I SystemServiceManager: Starting com.android.server.BatteryService
05-15 01:33:22.037  1124  1146 E /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: ISensors::poll() re-entry. I do not know what to do except killing myself.
05-15 01:33:22.043  1252  1252 D SystemServerTiming: StartBatteryService took to complete: 6ms
05-15 01:33:22.043  1252  1264 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:22.043  1252  1252 I SystemServer: StartUsageService
05-15 01:33:22.043  1252  1252 I SystemServiceManager: Starting com.android.server.usage.UsageStatsService
05-15 01:33:22.045  1252  1252 D SystemServerTiming: StartUsageService took to complete: 2ms
05-15 01:33:22.045  1252  1252 I SystemServer: StartWebViewUpdateService
05-15 01:33:22.045  1252  1252 I SystemServiceManager: Starting com.android.server.webkit.WebViewUpdateService
05-15 01:33:22.046  1252  1252 D SystemServerTiming: StartWebViewUpdateService took to complete: 1ms
05-15 01:33:22.047  1252  1252 I SystemServer: StartKeyAttestationApplicationIdProviderService
05-15 01:33:22.047  1252  1265 D SystemServerInitThreadPool: Started executing SecondaryZygotePreload
05-15 01:33:22.047  1252  1265 I SystemServer: SecondaryZygotePreload
05-15 01:33:22.047  1252  1252 D SystemServerTiming: StartKeyAttestationApplicationIdProviderService took to complete: 0ms
05-15 01:33:22.047  1252  1252 I SystemServer: StartKeyChainSystemService
05-15 01:33:22.047  1252  1252 I SystemServiceManager: Starting com.android.server.security.KeyChainSystemService
05-15 01:33:22.048  1252  1252 D SystemServerTiming: StartKeyChainSystemService took to complete: 1ms
05-15 01:33:22.048  1252  1252 I SystemServer: StartSchedulingPolicyService
05-15 01:33:22.048  1252  1252 D SystemServerTiming: StartSchedulingPolicyService took to complete: 0ms
05-15 01:33:22.048  1252  1252 I SystemServer: StartTelecomLoaderService
05-15 01:33:22.048  1252  1252 I SystemServiceManager: Starting com.android.server.telecom.TelecomLoaderService
05-15 01:33:22.049  1252  1252 D SystemServerTiming: StartTelecomLoaderService took to complete: 1ms
05-15 01:33:22.049  1252  1252 I SystemServer: StartTelephonyRegistry
05-15 01:33:22.051  1252  1252 D SystemServerTiming: StartTelephonyRegistry took to complete: 2ms
05-15 01:33:22.051  1252  1252 I SystemServer: StartEntropyMixer
05-15 01:33:22.052  1252  1252 I EntropyMixer: Writing entropy...
05-15 01:33:22.058  1252  1265 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:22.059  1252  1252 D SystemServerTiming: StartEntropyMixer took to complete: 8ms
05-15 01:33:22.059  1252  1252 I SystemServer: StartAccountManagerService
05-15 01:33:22.059  1252  1252 I SystemServiceManager: Starting com.android.server.accounts.AccountManagerService$Lifecycle
05-15 01:33:22.062  1252  1252 D SystemServerTiming: StartAccountManagerService took to complete: 3ms
05-15 01:33:22.062  1252  1252 I SystemServer: StartContentService
05-15 01:33:22.062  1252  1252 I SystemServiceManager: Starting com.android.server.content.ContentService$Lifecycle
05-15 01:33:22.063  1252  1252 D SystemServerTiming: StartContentService took to complete: 1ms
05-15 01:33:22.063  1252  1252 I SystemServer: InstallSystemProviders
05-15 01:33:22.077  1298  1298 I chatty  : uid=1000(system) /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service expire 62 lines
05-15 01:33:22.079  1252  1265 E SystemServer: Unable to preload default resources
05-15 01:33:22.079  1252  1265 D SystemServerTimingAsync: SecondaryZygotePreload took to complete: 32ms
05-15 01:33:22.079  1252  1265 D SystemServerInitThreadPool: Finished executing SecondaryZygotePreload
05-15 01:33:22.080  1252  1252 I SettingsState: No settings state /data/system/users/0/settings_ssaid.xml
05-15 01:33:22.083  1252  1252 D SystemServerTiming: InstallSystemProviders took to complete: 20ms
05-15 01:33:22.083  1252  1252 I SystemServer: StartVibratorService
05-15 01:33:22.087  1252  1252 D SystemServerTiming: StartVibratorService took to complete: 4ms
05-15 01:33:22.087  1252  1252 I SystemServer: StartConsumerIrService
05-15 01:33:22.088  1252  1252 E System  : ******************************************
05-15 01:33:22.088  1252  1252 E System  : ************ Failure starting core service
05-15 01:33:22.088  1252  1252 E System  : java.lang.RuntimeException: IR HAL present, but FEATURE_CONSUMER_IR is not set!
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.server.ConsumerIrService.<init>(ConsumerIrService.java:54)
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:831)
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.088  1252  1252 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.088  1252  1252 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.088  1252  1252 I SystemServer: StartInputMethodManagerLifecycle
05-15 01:33:22.089   733   733 W Binder:733_4: type=1400 audit(0.0:142): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:22.089   733   733 W Binder:733_5: type=1400 audit(0.0:145): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:22.089  1252  1252 I SystemServiceManager: Starting com.android.server.InputMethodManagerService$Lifecycle
05-15 01:33:22.092  1252  1252 D SystemServerTiming: StartInputMethodManagerLifecycle took to complete: 3ms
05-15 01:33:22.092  1252  1252 I SystemServer: StartAccessibilityManagerService
05-15 01:33:22.093  1252  1252 D SystemServerTiming: StartAccessibilityManagerService took to complete: 1ms
05-15 01:33:22.093  1252  1252 I SystemServer: MakeDisplayReady
05-15 01:33:22.093  1252  1252 W SystemServer: ***********************************************
05-15 01:33:22.094  1252  1252 E SystemServer: BOOT FAILURE making display ready
05-15 01:33:22.094  1252  1252 E SystemServer: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.wm.WindowManagerService.displayReady()' on a null object reference
05-15 01:33:22.094  1252  1252 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:947)
05-15 01:33:22.094  1252  1252 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.094  1252  1252 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.094  1252  1252 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.094  1252  1252 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.094  1252  1252 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.094  1252  1252 D SystemServerTiming: MakeDisplayReady took to complete: 1ms
05-15 01:33:22.094  1252  1252 I SystemServer: StartStorageManagerService
05-15 01:33:22.094  1252  1252 I SystemServiceManager: Starting com.android.server.StorageManagerService$Lifecycle
05-15 01:33:22.097  1252  1252 D SystemServerTiming: StartStorageManagerService took to complete: 3ms
05-15 01:33:22.097  1252  1252 I SystemServer: StartStorageStatsService
05-15 01:33:22.097  1252  1252 I SystemServiceManager: Starting com.android.server.usage.StorageStatsService$Lifecycle
05-15 01:33:22.098  1252  1306 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:22.098  1252  1306 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:22.098  1252  1306 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:22.098  1252  1306 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:22.098  1252  1306 D CryptdConnector: SND -> {1 cryptfs getfield SystemLocale}
05-15 01:33:22.101  1252  1308 D CryptdConnector: RCV <- {200 1 -1}
05-15 01:33:22.101  1252  1252 D SystemServerTiming: StartStorageStatsService took to complete: 4ms
05-15 01:33:22.101  1252  1252 I SystemServer: StartUiModeManager
05-15 01:33:22.101  1252  1252 I SystemServiceManager: Starting com.android.server.UiModeManagerService
05-15 01:33:22.102  1252  1306 W StorageManagerService: No primary storage mounted!
05-15 01:33:22.102  1252  1306 D VoldConnector: SND -> {1 asec list}
05-15 01:33:22.102  1252  1307 D VoldConnector: RCV <- {200 1 asec operation succeeded}
05-15 01:33:22.102  1252  1265 D SystemServerInitThreadPool: Started executing UiModeManager.onStart
05-15 01:33:22.102  1252  1252 D SystemServerTiming: StartUiModeManager took to complete: 1ms
05-15 01:33:22.102  1252  1306 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:22.102  1252  1252 I SystemServer: UpdatePackagesIfNeeded
05-15 01:33:22.103  1252  1252 D SystemServerTiming: UpdatePackagesIfNeeded took to complete: 1ms
05-15 01:33:22.103  1252  1252 I SystemServer: PerformFstrimIfNeeded
05-15 01:33:22.103  1252  1265 I ActivityManager: Config changes=200 {1.0 ?mcc?mnc [en_US] ldltr ?swdp ?wdp ?hdp ?density ?lsize ?long ?ldr ?wideColorGamut ?orien ?touch ?keyb/?/? ?nav/? s.2}
05-15 01:33:22.103  1252  1252 D SystemServerTiming: PerformFstrimIfNeeded took to complete: 0ms
05-15 01:33:22.103  1252  1252 I SystemServer: StartLockSettingsService
05-15 01:33:22.104  1252  1252 I SystemServiceManager: Starting com.android.server.locksettings.LockSettingsService$Lifecycle
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: Failure in UiModeManager.onStart: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityStackSupervisor.getDisplayOverrideConfiguration(ActivityStackSupervisor.java:488)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.performDisplayOverrideConfigUpdate(ActivityManagerService.java:20762)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateGlobalConfiguration(ActivityManagerService.java:20669)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfigurationLocked(ActivityManagerService.java:20547)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfiguration(ActivityManagerService.java:20486)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.sendConfigurationLocked(UiModeManagerService.java:478)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.lambda$-com_android_server_UiModeManagerService_9177(UiModeManagerService.java:236)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.$m$4(Unknown Source:4)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.run(Unknown Source:27)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.SystemServerInitThreadPool.lambda$-com_android_server_SystemServerInitThreadPool_2249(SystemServerInitThreadPool.java:64)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.$m$2(Unknown Source:8)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.run(Unknown Source:19)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:457)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1162)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:636)
05-15 01:33:22.110  1252  1265 E SystemServerInitThreadPool: 	at com.android.internal.util.ConcurrentUtils$1$1.run(ConcurrentUtils.java:59)
05-15 01:33:22.127  1252  1266 I UsageStatsService: User[0] Rollover scheduled @ 2018-05-16 01:33:22(1526434402104)
05-15 01:33:22.127  1252  1266 E AppIdleHistory: Unable to read app idle file for user 0
05-15 01:33:22.127  1252  1306 W StorageManagerService: No primary storage mounted!
05-15 01:33:22.127  1252  1306 D VoldConnector: SND -> {2 asec list}
05-15 01:33:22.127  1252  1307 D VoldConnector: RCV <- {200 2 asec operation succeeded}
05-15 01:33:22.129  1252  1252 D SystemServerTiming: StartLockSettingsService took to complete: 26ms
05-15 01:33:22.131  1252  1252 I OemLock : OemLock HAL not present on device
05-15 01:33:22.131  1252  1252 I SystemServer: StartDeviceIdleController
05-15 01:33:22.131  1252  1252 I SystemServiceManager: Starting com.android.server.DeviceIdleController
05-15 01:33:22.133  1252  1252 D SystemServerTiming: StartDeviceIdleController took to complete: 2ms
05-15 01:33:22.133  1252  1252 I SystemServer: StartDevicePolicyManager
05-15 01:33:22.133  1252  1252 I SystemServiceManager: Starting com.android.server.devicepolicy.DevicePolicyManagerService$Lifecycle
05-15 01:33:22.134  1252  1295 D SystemServerInitThreadPool: Finished executing Init OverlayManagerService
05-15 01:33:22.136  1252  1252 D SystemServerTiming: StartDevicePolicyManager took to complete: 3ms
05-15 01:33:22.136  1252  1252 I SystemServer: StartStatusBarManagerService
05-15 01:33:22.137  1252  1252 D SystemServerTiming: StartStatusBarManagerService took to complete: 1ms
05-15 01:33:22.137  1252  1252 I SystemServer: StartClipboardService
05-15 01:33:22.137  1252  1252 I SystemServiceManager: Starting com.android.server.clipboard.ClipboardService
05-15 01:33:22.138  1252  1252 D SystemServerTiming: StartClipboardService took to complete: 1ms
05-15 01:33:22.138  1252  1252 I SystemServer: StartNetworkManagementService
05-15 01:33:22.140  1252  1314 I NetworkManagement: onDaemonConnected()
05-15 01:33:22.140  1252  1252 D SystemServerTiming: StartNetworkManagementService took to complete: 2ms
05-15 01:33:22.140  1252  1252 I SystemServer: StartTextServicesManager
05-15 01:33:22.140  1252  1252 I SystemServiceManager: Starting com.android.server.TextServicesManagerService$Lifecycle
05-15 01:33:22.144  1252  1252 D SystemServerTiming: StartTextServicesManager took to complete: 4ms
05-15 01:33:22.144  1252  1252 I SystemServer: StartNetworkScoreService
05-15 01:33:22.144  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-8 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.144  1298  1298 D SensorHub: Channel activate-> handle: 8, enabled:0, err: 0
05-15 01:33:22.145  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-11 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.145  1298  1298 D SensorHub: Channel activate-> handle: 11, enabled:0, err: 0
05-15 01:33:22.145  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-12 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.145  1298  1298 D SensorHub: Channel activate-> handle: 12, enabled:0, err: 0
05-15 01:33:22.145  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-13 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.145  1298  1298 D SensorHub: Channel activate-> handle: 13, enabled:0, err: 0
05-15 01:33:22.145  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-14 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.145  1298  1298 D SensorHub: Channel activate-> handle: 14, enabled:0, err: 0
05-15 01:33:22.145  1252  1252 D SystemServerTiming: StartNetworkScoreService took to complete: 1ms
05-15 01:33:22.145  1252  1252 I SystemServer: StartNetworkStatsService
05-15 01:33:22.146  1298  1315 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-15 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.146  1298  1315 D SensorHub: Channel activate-> handle: 15, enabled:0, err: 0
05-15 01:33:22.146  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-17 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.146  1298  1298 D SensorHub: Channel activate-> handle: 17, enabled:0, err: 0
05-15 01:33:22.146  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-18 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.146  1298  1298 D SensorHub: Channel activate-> handle: 18, enabled:0, err: 0
05-15 01:33:22.146  1298  1298 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-21 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:22.146  1298  1298 D SensorHub: Channel activate-> handle: 21, enabled:0, err: 0
05-15 01:33:22.147  1252  1317 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:22.147  1252  1296 D SystemServerTimingAsync: StartSensorService took to complete: 112ms
05-15 01:33:22.147  1252  1296 D SystemServerInitThreadPool: Finished executing StartSensorService
05-15 01:33:22.147  1252  1318 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:22.149  1252  1252 W SystemServer: ***********************************************
05-15 01:33:22.149  1252  1252 E SystemServer: BOOT FAILURE starting NetworkStats Service
05-15 01:33:22.149  1252  1252 E SystemServer: java.lang.NullPointerException: missing AlarmManager
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.server.net.NetworkStatsService.<init>(NetworkStatsService.java:309)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:289)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.149  1252  1252 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.150  1252  1252 D SystemServerTiming: StartNetworkStatsService took to complete: 4ms
05-15 01:33:22.150  1252  1252 I SystemServer: StartNetworkPolicyManagerService
05-15 01:33:22.151  1252  1252 W SystemServer: ***********************************************
05-15 01:33:22.151  1252  1252 E SystemServer: BOOT FAILURE starting NetworkPolicy Service
05-15 01:33:22.151  1252  1252 E SystemServer: java.lang.NullPointerException: missing networkStats
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:501)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:487)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1096)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.151  1252  1252 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.151  1252  1252 D SystemServerTiming: StartNetworkPolicyManagerService took to complete: 1ms
05-15 01:33:22.151  1252  1252 I SystemServer: StartWifi
05-15 01:33:22.153  1252  1252 I SystemServiceManager: Starting com.android.server.wifi.WifiService
05-15 01:33:22.187  1202  1219 D CommandListener: Clearing all IP addresses on wlan0
05-15 01:33:22.187  1252  1325 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:22.192  1252  1252 D SystemServerTiming: StartWifi took to complete: 41ms
05-15 01:33:22.192  1252  1252 I SystemServer: StartWifiScanning
05-15 01:33:22.193  1252  1252 I SystemServiceManager: Starting com.android.server.wifi.scanner.WifiScanningService
05-15 01:33:22.194  1252  1252 D SystemServerTiming: StartWifiScanning took to complete: 2ms
05-15 01:33:22.195  1252  1252 I SystemServer: StartWifiRtt
05-15 01:33:22.195  1252  1252 I SystemServiceManager: Starting com.android.server.wifi.RttService
05-15 01:33:22.196  1252  1252 D SystemServerTiming: StartWifiRtt took to complete: 1ms
05-15 01:33:22.196  1252  1252 I SystemServer: No Wi-Fi Aware Service (Aware support Not Present)
05-15 01:33:22.196  1252  1252 I SystemServer: StartWifiP2P
05-15 01:33:22.196  1252  1252 I SystemServiceManager: Starting com.android.server.wifi.p2p.WifiP2pService
05-15 01:33:22.199  1252  1252 D SystemServerTiming: StartWifiP2P took to complete: 3ms
05-15 01:33:22.199  1252  1252 I SystemServer: StartEthernet
05-15 01:33:22.200  1252  1252 I SystemServiceManager: Starting com.android.server.ethernet.EthernetService
05-15 01:33:22.202  1252  1252 D SystemServerTiming: StartEthernet took to complete: 3ms
05-15 01:33:22.202  1252  1252 I SystemServer: StartConnectivityService
05-15 01:33:22.205  1252  1252 D ConnectivityService: ConnectivityService starting up
05-15 01:33:22.206  1252  1252 W SystemServer: ***********************************************
05-15 01:33:22.206  1252  1252 E SystemServer: BOOT FAILURE starting Connectivity Service
05-15 01:33:22.206  1252  1252 E SystemServer: java.lang.NullPointerException: missing INetworkStatsService
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:722)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:690)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1151)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.206  1252  1252 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.206  1252  1252 D SystemServerTiming: StartConnectivityService took to complete: 4ms
05-15 01:33:22.206  1252  1252 I SystemServer: StartNsdService
05-15 01:33:22.207  1252  1252 D NsdService: Network service discovery is enabled
05-15 01:33:22.208  1252  1252 D SystemServerTiming: StartNsdService took to complete: 2ms
05-15 01:33:22.208  1252  1252 I SystemServer: StartUpdateLockService
05-15 01:33:22.209  1252  1252 D SystemServerTiming: StartUpdateLockService took to complete: 1ms
05-15 01:33:22.209  1252  1252 I SystemServer: WaitForAsecScan
05-15 01:33:22.209  1252  1252 D SystemServerTiming: WaitForAsecScan took to complete: 0ms
05-15 01:33:22.209  1252  1252 I SystemServer: StartNotificationManager
05-15 01:33:22.209  1252  1252 I SystemServiceManager: Starting com.android.server.notification.NotificationManagerService
05-15 01:33:22.218  1252  1292 D SystemServerTimingAsync: AppDataPrepare took to complete: 236ms
05-15 01:33:22.218  1252  1292 I PackageManager: Deferred reconcileAppsData finished 73 packages
05-15 01:33:22.218  1252  1292 D SystemServerInitThreadPool: Finished executing prepareAppData
05-15 01:33:22.229  1252  1252 D ConditionProviders.SCP: new ScheduleConditionProvider()
05-15 01:33:22.229  1252  1252 I ConditionProviders:  Allowing condition provider org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:22.229  1252  1252 I NotificationListeners:  Allowing notification listener org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:22.230  1252  1252 I ConditionProviders:  Allowing condition provider com.android.camera2
05-15 01:33:22.230  1252  1252 D ZenLog  : set_zen_mode: off,init
05-15 01:33:22.238   526   526 D lights  : set_light_notification colorRGB=00000000, onMS=0, offMS=0
05-15 01:33:22.240  1252  1252 E System  : ******************************************
05-15 01:33:22.240  1252  1252 E System  : ************ Failure starting system services
05-15 01:33:22.240  1252  1252 E System  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:22.240  1252  1252 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:22.240  1252  1252 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.240  1252  1252 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.240  1252  1252 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.240  1252  1252 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.240  1252  1252 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.240  1252  1252 D SystemServerTiming: StartNotificationManager took to complete: 31ms
05-15 01:33:22.240  1252  1252 E Zygote  : System zygote died with exception
05-15 01:33:22.240  1252  1252 E Zygote  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:22.240  1252  1252 E Zygote  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:22.240  1252  1252 E Zygote  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.240  1252  1252 E Zygote  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.240  1252  1252 E Zygote  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.240  1252  1252 E Zygote  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.240  1252  1252 E Zygote  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.240  1252  1252 D AndroidRuntime: Shutting down VM
05-15 01:33:22.240  1252  1252 E AndroidRuntime: *** FATAL EXCEPTION IN SYSTEM PROCESS: main
05-15 01:33:22.240  1252  1252 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:22.240  1252  1252 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:22.241  1252  1252 I Process : Sending signal. PID: 1252 SIG: 9
05-15 01:33:22.259   752   770 I hinetmanager_vcom: open device result 2
05-15 01:33:22.259   752   770 E hinetmanager_vcom: open device failed, timeout
05-15 01:33:22.292   536   536 I lowmemorykiller: ActivityManager disconnected
05-15 01:33:22.292   536   536 I lowmemorykiller: Closing Activity Manager data connection
05-15 01:33:22.293  1198  1198 E Zygote  : Exit zygote because system server (1252) has terminated
05-15 01:33:22.293   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:22.293   346   346 E         : 
05-15 01:33:22.293  1198  1198 F libc    : Fatal signal 6 (SIGABRT), code 0 in tid 1198 (main), pid 1198 (main)
05-15 01:33:22.297   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:22.297   346   346 E         : 
05-15 01:33:22.297   511  1338 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 1 line
05-15 01:33:22.297   511  1339 I chatty  : uid=1041(audioserver) audio@2.0-servi expire 1 line
05-15 01:33:22.297   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 5 lines
05-15 01:33:22.298  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 4 lines
05-15 01:33:22.300  1199  1342 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 2 lines
05-15 01:33:22.300  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:22.300   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 1 line
05-15 01:33:22.300   511  1188 I chatty  : uid=1041(audioserver) HwBinder:511_4 expire 1 line
05-15 01:33:22.300  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:22.300  1199  1342 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:22.300   511  1188 I chatty  : uid=1041(audioserver) HwBinder:511_4 expire 8 lines
05-15 01:33:22.301   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 2 lines
05-15 01:33:22.301  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 3 lines
05-15 01:33:22.301   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 3 lines
05-15 01:33:22.301  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 4 lines
05-15 01:33:22.301   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 2 lines
05-15 01:33:22.302  1199  1199 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 2 lines
05-15 01:33:22.302   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 expire 2 lines
05-15 01:33:22.302  1199  1344 I chatty  : uid=1041(audioserver) /system/bin/audioserver expire 1 line
05-15 01:33:22.302   511   904 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:22.302   511   904 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:22.302   511  1188 I audio_hw_primary: update config period size 960
05-15 01:33:22.302   511   904 D dsp_soc : set source 0 succ
05-15 01:33:22.303   511  1188 I audio_hw_primary: change channel_mask form 80000007 to AUDIO_CHANNEL_IN_STEREO
05-15 01:33:22.303   511   904 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:22.303  1199  1346 I AudioFlinger: AudioFlinger's thread 0xe6f835c0 tid=1346 ready to run
05-15 01:33:22.303   511  1188 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:22.303   511  1188 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:22.303   511   904 I audio_hw_primary: update config period size 960
05-15 01:33:22.303   511  1188 D dsp_soc : set source 0 succ
05-15 01:33:22.303   511  1188 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:22.303  1199  1348 I AudioFlinger: AudioFlinger's thread 0xe6f83980 tid=1348 ready to run
05-15 01:33:22.303   511   904 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:22.303   511   904 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:22.304   511   904 D dsp_soc : set source 0 succ
05-15 01:33:22.304   511   904 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:22.306  1199  1199 I bt_a2dp_hw: adev_open:  adev_open in A2dp_hw module
05-15 01:33:22.306  1199  1199 I AudioFlinger: loadHwModule() Loaded a2dp audio interface, handle 18
05-15 01:33:22.307   511   904 D vndksupport: Loading /vendor/lib64/hw/audio.usb.default.so from current namespace instead of sphal namespace.
05-15 01:33:22.307  1199  1199 I AudioFlinger: loadHwModule() Loaded usb audio interface, handle 26
05-15 01:33:22.307   511   904 D vndksupport: Loading /vendor/lib64/hw/audio.r_submix.default.so from current namespace instead of sphal namespace.
05-15 01:33:22.307   511   904 I r_submix: adev_open(name=audio_hw_if)
05-15 01:33:22.307   511   904 I r_submix: adev_init_check()
05-15 01:33:22.307   511   904 W DeviceHAL: Device 0x7589a14380 set_master_mute: Function not implemented
05-15 01:33:22.307  1199  1199 I AudioFlinger: loadHwModule() Loaded r_submix audio interface, handle 34
05-15 01:33:22.308   511   904 D r_submix: adev_open_input_stream(addr=0)
05-15 01:33:22.308   511   904 D r_submix: submix_audio_device_create_pipe_l(addr=0, idx=9)
05-15 01:33:22.308   511   904 D r_submix:   now using address 0 for route 9
05-15 01:33:22.308  1199  1353 I AudioFlinger: AudioFlinger's thread 0xe6f83140 tid=1353 ready to run
05-15 01:33:22.308   511   904 D r_submix: adev_close_input_stream()
05-15 01:33:22.308  1199  1199 W APM_AudioPolicyManager: Output device 00010000 unreachable
05-15 01:33:22.308   511   904 D r_submix: submix_audio_device_release_pipe_l(idx=9) addr=0
05-15 01:33:22.308   511   904 D r_submix: submix_audio_device_destroy_pipe_l(): pipe destroyed
05-15 01:33:22.308  1199  1199 E EffectsConfig: Failed to parse /vendor/etc/audio_effects.xml: Tinyxml2 error (3): /vendor/etc/audio_effects.xml (null)
05-15 01:33:22.308  1199  1199 W AudioPolicyEffects: Failed to load XML effect configuration, fallback to .conf
05-15 01:33:22.310   511   904 I soundtrigger_hw: stdev_get_properties
05-15 01:33:22.310  1199  1199 I SoundTriggerHalHidl: getProperties res implementor The Android Open Source Project
05-15 01:33:22.310  1199  1199 I SoundTriggerHalHidl: getProperties ret 0
05-15 01:33:22.310  1199  1199 I SoundTriggerHwService: loaded default module Volantis OK Google , handle 1
05-15 01:33:22.313  1349  1349 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-15 01:33:22.314   751   751 I /system/bin/tombstoned: received crash request for pid 1198
05-15 01:33:22.314  1349  1349 I crash_dump64: performing dump of process 1198 (target tid = 1198)
05-15 01:33:22.314  1349  1349 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-15 01:33:22.315  1349  1349 F DEBUG   : LineageOS Version: 'unknown'
05-15 01:33:22.315  1349  1349 F DEBUG   : Build fingerprint: 'Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys'
05-15 01:33:22.315  1349  1349 F DEBUG   : Revision: '0'
05-15 01:33:22.315  1349  1349 F DEBUG   : ABI: 'arm64'
05-15 01:33:22.315  1349  1349 F DEBUG   : pid: 1198, tid: 1198, name: main  >>> zygote64 <<<
05-15 01:33:22.315  1349  1349 F DEBUG   : signal 6 (SIGABRT), code 0 (SI_USER), fault addr --------
05-15 01:33:22.315  1349  1349 F DEBUG   :     x0   0000000000000000  x1   0000000000000009  x2   0000000000000005  x3   0000000000000003
05-15 01:33:22.315  1349  1349 F DEBUG   :     x4   0000000040100401  x5   a802a00080404000  x6   0000000000000000  x7   7f7f7f7f7f7f7f7f
05-15 01:33:22.315  1349  1349 F DEBUG   :     x8   0000000000000081  x9   a4ddcbd023c9d8fc  x10  0000007fe1a6de40  x11  0000000000000038
05-15 01:33:22.315  1349  1349 F DEBUG   :     x12  000000000000000b  x13  ffffffffffffffff  x14  ff00000000000000  x15  ffffffffffffffff
05-15 01:33:22.315  1349  1349 F DEBUG   :     x16  000000784862f300  x17  0000007845eaf55c  x18  0000000070215150  x19  000000784949fa50
05-15 01:33:22.315  1349  1349 F DEBUG   :     x20  00000078485db1e6  x21  00000078485db64a  x22  00000078485db6a6  x23  00000000000004e4
05-15 01:33:22.315  1349  1349 F DEBUG   :     x24  00000078485db68e  x25  00000078485db669  x26  000000784949fa40  x27  0000000000000002
05-15 01:33:22.315  1349  1349 F DEBUG   :     x28  0000007848634000  x29  0000007fe1a6e410  x30  000000784859500c
05-15 01:33:22.315  1349  1349 F DEBUG   :     sp   0000007fe1a6e3b0  pc   0000007845eaf564  pstate 0000000060000000
05-15 01:33:22.550  1349  1349 F DEBUG   : 
05-15 01:33:22.550  1349  1349 F DEBUG   : backtrace:
05-15 01:33:22.550  1349  1349 F DEBUG   :     #00 pc 000000000006a564  /system/lib64/libc.so (kill+8)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #01 pc 0000000000176008  /system/lib64/libandroid_runtime.so ((anonymous namespace)::SigChldHandler(int)+280)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #02 pc 00000000000005f0  [vdso:0000007849334000]
05-15 01:33:22.550  1349  1349 F DEBUG   :     #03 pc 0000000000069ea0  /system/lib64/libc.so (__ppoll+4)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #04 pc 00000000000265e4  /system/lib64/libc.so (poll+88)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #05 pc 000000000002e9a8  /system/lib64/libjavacore.so (Linux_poll(_JNIEnv*, _jobject*, _jobjectArray*, int)+800)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #06 pc 000000000030bad0  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.Linux.fcntlVoid [DEDUPED]+160)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #07 pc 0000000000300a74  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.BlockGuardOs.poll+228)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #08 pc 00000000002b67a4  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (android.system.Os.poll+84)
05-15 01:33:22.550  1349  1349 F DEBUG   :     #09 pc 000000000164e488  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteServer.runSelectLoop+664)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #10 pc 0000000001652ed8  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteInit.main+2728)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #11 pc 000000000054744c  /system/lib64/libart.so (art_quick_invoke_static_stub+604)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #12 pc 00000000000dc7b0  /system/lib64/libart.so (art::ArtMethod::Invoke(art::Thread*, unsigned int*, unsigned int, art::JValue*, char const*)+260)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #13 pc 000000000046bb70  /system/lib64/libart.so (art::InvokeWithArgArray(art::ScopedObjectAccessAlreadyRunnable const&, art::ArtMethod*, art::ArgArray*, art::JValue*, char const*)+100)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #14 pc 000000000046b79c  /system/lib64/libart.so (art::InvokeWithVarArgs(art::ScopedObjectAccessAlreadyRunnable const&, _jobject*, _jmethodID*, std::__va_list)+420)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #15 pc 0000000000372a54  /system/lib64/libart.so (art::JNI::CallStaticVoidMethodV(_JNIEnv*, _jclass*, _jmethodID*, std::__va_list)+620)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #16 pc 00000000000a6fb8  /system/lib64/libandroid_runtime.so (_JNIEnv::CallStaticVoidMethod(_jclass*, _jmethodID*, ...)+120)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #17 pc 00000000000a9728  /system/lib64/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+832)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #18 pc 0000000000002440  /system/bin/app_process64 (main+1328)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #19 pc 00000000000a14d4  /system/lib64/libc.so (__libc_init+88)
05-15 01:33:22.555  1349  1349 F DEBUG   :     #20 pc 0000000000001e70  /system/bin/app_process64 (_start_main+80)
05-15 01:33:22.685  1349  1349 E crash_dump64: unable to connect to activity manager: No such file or directory
05-15 01:33:22.685   751   751 E /system/bin/tombstoned: Tombstone written to: /data/tombstones/tombstone_00
05-15 01:33:22.783   511  1188 I r_submix: adev_close()
05-15 01:33:22.783   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 0,  out_device: 0x2
05-15 01:33:22.783   511   904 I audio_hw_primary: adev_close
05-15 01:33:22.783   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 4,  out_device: 0x2
05-15 01:33:22.783   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 5,  out_device: 0x2
05-15 01:33:22.783   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 6,  out_device: 0x2
05-15 01:33:22.783   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 7,  out_device: 0x2
05-15 01:33:22.783   511   904 I audio_hw_primary: destroy_offload_standby_thread
05-15 01:33:22.783   511  1338 I audio_hw_primary: offload_standby_loop: wait standby_cond succ
05-15 01:33:23.000   511  1166 E audio_hw_primary: direct_standby_loop: adev->outputs[OUTPUT_DIRECT] is NULL
05-15 01:33:23.000   511  1166 I audio_hw_primary: direct_standby_loop: standby loop exit...
05-15 01:33:23.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 4,  out_device: 0x2
05-15 01:33:23.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 5,  out_device: 0x2
05-15 01:33:23.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 6,  out_device: 0x2
05-15 01:33:23.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 7,  out_device: 0x2
05-15 01:33:23.000   511  1034 E typec_headset_hal: typec_headset_uninit:already null so no need to free
05-15 01:33:23.000   511  1034 D dsp_interface: dsp_close:
05-15 01:33:23.000   511  1034 I dsp_soc_ctl: dsp_soc_ctl_close++
05-15 01:33:23.000   511  1034 I dsp_soc_ctl: close /dev/hifi_misc.
05-15 01:33:23.000   511  1034 I dsp_soc_ctl: dsp_soc_ctl_close--
05-15 01:33:23.001   511  1034 I MAX98925_SPK: maxim smartpa close
05-15 01:33:24.030  1366  1366 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:24.031  1365  1365 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:24.032  1365  1365 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:24.032  1365  1365 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:24.033  1365  1365 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:24.033  1366  1366 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:24.035  1366  1366 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:25.000   511  1338 E audio_hw_primary: offload_standby_loop: adev->outputs[OUTPUT_OFFLOAD] is NULL
05-15 01:33:25.000   511  1338 I audio_hw_primary: offload_standby_loop: standby loop exit...
05-15 01:33:25.000   511   904 I audio_hw_primary: destroy_direct_standby_thread
05-15 01:33:25.000   511  1339 I audio_hw_primary: direct_standby_loop: wait standby_cond succ
05-15 01:33:26.141  1376  1376 I Netd    : Netd 1.0 starting
05-15 01:33:26.141  1376  1376 D TetherController: Setting IP forward enable = 0
05-15 01:33:26.161  1377  1377 I wificond: wificond is starting up...
05-15 01:33:26.180  1378  1378 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:26.180  1378  1378 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:26.180  1378  1378 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:26.180  1378  1378 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:26.180  1378  1378 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:26.183  1378  1378 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:26.183  1378  1378 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:26.183  1378  1378 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:26.188  1376  1376 I Netd    : Creating child chains: 14.2ms
05-15 01:33:26.188  1376  1376 I Netd    : Setting up OEM hooks: 0.2ms
05-15 01:33:26.192  1376  1376 I Netd    : Setting up FirewallController hooks: 3.4ms
05-15 01:33:26.194  1376  1376 I Netd    : Setting up NatController hooks: 2.6ms
05-15 01:33:26.196  1376  1376 I Netd    : Setting up BandwidthController hooks: 2.0ms
05-15 01:33:26.196  1376  1376 I Netd    : Setting up IdletimerController hooks: 0.0ms
05-15 01:33:26.199  1374  1374 W cameraserver: type=1400 audit(0.0:146): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2092 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:26.199  1374  1374 W cameraserver: type=1400 audit(0.0:147): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2295 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:26.200  1376  1376 I Netd    : Disabling bandwidth control: 3.2ms
05-15 01:33:26.201  1376  1376 E Netd    : cannot find interface dummy0
05-15 01:33:26.201  1376  1376 I Netd    : Initializing RouteController: 1.5ms
05-15 01:33:26.202  1376  1376 E Netd    : Unable to create netlink socket: Protocol not supported
05-15 01:33:26.202  1376  1376 W Netd    : Unable to open qlog quota socket, check if xt_quota2 can send via UeventHandler
05-15 01:33:26.202  1376  1376 D MDnsDS  : MDnsSdListener::Hander starting up
05-15 01:33:26.202  1376  1389 D MDnsDS  : MDnsSdListener starting to monitor
05-15 01:33:26.202  1376  1389 D MDnsDS  : Going to poll with pollCount 1
05-15 01:33:26.203  1376  1376 I Netd    : Registering NetdNativeService: 0.7ms
05-15 01:33:26.203  1376  1376 I Netd    : Starting CommandListener: 0.1ms
05-15 01:33:26.205  1376  1376 I Netd    : Registering NetdHwService: 1.7ms
05-15 01:33:26.205  1376  1376 I Netd    : Netd started in 63ms
05-15 01:33:26.207  1374  1374 I cameraserver: ServiceManager: 0xef6979a0
05-15 01:33:26.207  1374  1374 I CameraService: CameraService started (pid=1374)
05-15 01:33:26.207  1374  1374 I CameraService: CameraService process starting
05-15 01:33:26.208  1374  1374 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:26.208  1374  1374 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:26.210  1374  1374 E vndksupport: Could not load /vendor/lib/hw/android.hardware.camera.provider@2.4-impl.so from sphal namespace: dlopen failed: library "android.hardware.camera.device@1.0.so" not found.
05-15 01:33:26.210  1374  1374 E /system/bin/cameraserver: Failed to dlopen android.hardware.camera.provider@2.4-impl.so: unknown error
05-15 01:33:26.212  1375  1375 I mediaserver: ServiceManager: 0xe7197a40
05-15 01:33:26.212  1375  1375 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:26.242  1373  1373 I FastMixerState: sMaxFastTracks = 8
05-15 01:33:26.245  1373  1373 I audioserver: ServiceManager: 0xf1d97940
05-15 01:33:26.245  1373  1373 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:26.247  1373  1373 I AudioFlinger: Using default 3000 mSec as standby time.
05-15 01:33:26.248  1373  1373 E APM::Serializer: deserialize: Could not parse /odm/etc/audio_policy_configuration.xml document.
05-15 01:33:26.252   511  1034 D vndksupport: Loading /vendor/lib64/hw/audio.primary.hisi.so from current namespace instead of sphal namespace.
05-15 01:33:26.253   511  1034 I audio_hw_primary: adev_open:
05-15 01:33:26.253   511  1034 I audio_hw_primary: offload mode is enable
05-15 01:33:26.277   346   346 E         : pid 511, opration oeminfo_read OK
05-15 01:33:26.277   346   346 E         : 
05-15 01:33:26.277   511  1034 I audio_config: get_vendor_info: vendor_country_info = all/cn
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:KNIGHT
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get product_name succ, product_name = KNIGHT
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:audio_custom
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get cust_name succ, cust_name = audio_custom
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:max98925
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get spk_pa_name succ, spk_pa_name = max98925
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:hi363x
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get soc_name succ, soc_name = hi363x
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:hi6402
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get codec_name succ, codec_name = hi6402
05-15 01:33:26.277   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get mic_name not succ, set mic_name = none as default
05-15 01:33:26.277   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get hs_pa_name not succ, set hs_pa_name = none as default
05-15 01:33:26.277   511  1034 V audio_common: get value success, value:true
05-15 01:33:26.277   511  1034 I audio_config: get_audio_configs: get modem_sio_master succ, modem_sio_master = 1
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:max98925
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get ear_pa_name succ, ear_pa_name = max98925
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:true
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get vqm function enable succ, vqm function enable = 1
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:true
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get bwe function support succ, bwe function support = 1
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 W audio_config: get_audio_configs: get swb function support not succ, set swb function support = 0 as default
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:false
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get multi mic function enable succ, multi_mic_enable = 0
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:true
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get dual_smartpa_support function support succ, dual_smartpa_support function support = true
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:0.0
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get dual_smartpa_verison = 0.0 succ.
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:false
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get voice_anc_support function support succ, voice_anc_support function support = flase
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 W audio_config: get_audio_configs: get visualizer_support fail, set visualizer_support as false
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:true
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get asr feature enable succ, asr_enable = 1
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:ok
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get soundtrigger feature enable succ, soundtrigger_enable = 1
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 W audio_config: get_audio_configs: get spk_num not succ, set spk_num = 1 as default
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:speaker
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get speaker_test_content succ, speaker_test_content = speaker
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:1
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get smartpa_info pa_num succ, pa_num = 1
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:0
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get smartpa_info algo_in succ, algo_in = 0
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:0001
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get smartpa_info pa_type succ, pa_type = 1
05-15 01:33:26.278   511  1034 V audio_common: get value success, value:false
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get audio sar function support succ, sar_support = 0
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: use default max stream volume
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 W audio_config: get_audio_ir_configs: get analog earpiece function enable not succ, set analog_earpiece  enable = 0 as default
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 I audio_config: get_audio_configs: get codec stub not succ, set codec stub = 0 as default
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 I audio_config: get_karaoke_mic_configs:karaoke mic configuration support = NA
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.278   511  1034 I audio_config: get_smartpa_latency_configs: smartpa latency use default 0
05-15 01:33:26.278   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 W audio_config: get_audio_hifi_info_configs: get extern headset hifi function enable not succ, set ext_hs_hifi_enable = 0 as default
05-15 01:33:26.279   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 W audio_config: get_audio_hifi_info_configs: get support_dynamic_rate not succ, set support_dynamic_rate = 0 as default
05-15 01:33:26.279   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 W audio_config: get_audio_hifi_info_configs: get support_Hperform_Lpower not succ, set support_Hperform_Lpower = 0 as default
05-15 01:33:26.279   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 W audio_config: get_audio_hifi_info_configs: get digital_voice_wakeup_enable not succ, set digital_voice_wakeup_enable = 0 as default
05-15 01:33:26.279   511  1034 W audio_common: open dts file failed! May not need in this case
05-15 01:33:26.279   511  1034 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:26.279   511  1407 E audio_hw_primary: UEVENT  init fail
05-15 01:33:26.279   511  1034 E audio_config: get_para_config_file_print_err:get audio/devicemask/typec_headset_devicemask_KNIGHT.xml failed.
05-15 01:33:26.279   511  1034 I audio_hw_primary: codec_init: paths_xml is /odm/etc/audio/hi6402/mixer_paths_KNIGHT.xml
05-15 01:33:26.295  1372  1372 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:26.298  1372  1372 I zygote64: option[0]=-Xzygote
05-15 01:33:26.298  1372  1372 I zygote64: option[1]=-Xusetombstonedtraces
05-15 01:33:26.298  1372  1372 I zygote64: option[2]=exit
05-15 01:33:26.298  1372  1372 I zygote64: option[3]=vfprintf
05-15 01:33:26.298  1372  1372 I zygote64: option[4]=sensitiveThread
05-15 01:33:26.298  1372  1372 I zygote64: option[5]=-verbose:gc
05-15 01:33:26.298  1372  1372 I zygote64: option[6]=-Xms8m
05-15 01:33:26.298  1372  1372 I zygote64: option[7]=-Xmx512m
05-15 01:33:26.299  1372  1372 I zygote64: option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:26.299  1372  1372 I zygote64: option[9]=-XX:HeapMinFree=2m
05-15 01:33:26.299  1372  1372 I zygote64: option[10]=-XX:HeapMaxFree=8m
05-15 01:33:26.299  1372  1372 I zygote64: option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:26.299  1372  1372 I zygote64: option[12]=-Xusejit:true
05-15 01:33:26.299  1372  1372 I zygote64: option[13]=-Xjitsaveprofilinginfo
05-15 01:33:26.299  1372  1372 I zygote64: option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:26.299  1372  1372 I zygote64: option[15]=-Xlockprofthreshold:500
05-15 01:33:26.299  1372  1372 I zygote64: option[16]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[17]=--runtime-arg
05-15 01:33:26.299  1372  1372 I zygote64: option[18]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[19]=-Xms64m
05-15 01:33:26.299  1372  1372 I zygote64: option[20]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[21]=--runtime-arg
05-15 01:33:26.299  1372  1372 I zygote64: option[22]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[23]=-Xmx64m
05-15 01:33:26.299  1372  1372 I zygote64: option[24]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:26.299  1372  1372 I zygote64: option[26]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:26.299  1372  1372 I zygote64: option[28]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:26.299  1372  1372 I zygote64: option[30]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[31]=--runtime-arg
05-15 01:33:26.299  1372  1372 I zygote64: option[32]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[33]=-Xms64m
05-15 01:33:26.299  1372  1372 I zygote64: option[34]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[35]=--runtime-arg
05-15 01:33:26.299  1372  1372 I zygote64: option[36]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[37]=-Xmx512m
05-15 01:33:26.299  1372  1372 I zygote64: option[38]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[39]=-j4
05-15 01:33:26.299  1372  1372 I zygote64: option[40]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[41]=-j4
05-15 01:33:26.299  1372  1372 I zygote64: option[42]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[43]=--instruction-set-variant=generic
05-15 01:33:26.299  1372  1372 I zygote64: option[44]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[45]=--instruction-set-variant=generic
05-15 01:33:26.299  1372  1372 I zygote64: option[46]=-Ximage-compiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[47]=--instruction-set-features=default
05-15 01:33:26.299  1372  1372 I zygote64: option[48]=-Xcompiler-option
05-15 01:33:26.299  1372  1372 I zygote64: option[49]=--instruction-set-features=default
05-15 01:33:26.299  1372  1372 I zygote64: option[50]=-Duser.locale=en-US
05-15 01:33:26.299  1372  1372 I zygote64: option[51]=--cpu-abilist=arm64-v8a
05-15 01:33:26.299  1372  1372 I zygote64: option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:26.340   511  1034 E audio_route: Control 'S4 IF CLK EN' already exists in path 'media-speaker-earpiece'
05-15 01:33:26.340   511  1034 E audio_route: Control 'HPDAC_I2V SWITCH' already exists in path 'media-speaker-headset'
05-15 01:33:26.340   511  1034 E audio_route: Control 'HPDAC_I2V SWITCH' already exists in path 'media-speaker-headphone'
05-15 01:33:26.340   511  1034 E audio_route: Control 'S4 IF CLK EN' already exists in path 'communication-speaker-earpiece'
05-15 01:33:26.340   511  1034 E audio_route: Control 'S4 IF CLK EN' already exists in path 'media-fm-speaker-earpiece'
05-15 01:33:26.340   511  1034 E audio_route: Control 'S4 IF CLK EN' already exists in path 'dup-call-m0-speaker-earpiece'
05-15 01:33:26.341   511  1034 E audio_route: Control 'S4 IF CLK EN' already exists in path 'dup-call-wb-m0-speaker-earpiece'
05-15 01:33:26.341   511  1034 E audio_route: unknown enum value string S2L for ctl APR MUX
05-15 01:33:26.341   511  1034 E audio_route: unknown enum value string S2L for ctl APR MUX
05-15 01:33:26.342   511  1034 I audio_hw_primary: codec_init: pop_seq_xml is /odm/etc/audio/hi6402/pop_seq_KNIGHT.xml
05-15 01:33:26.342   511  1034 I audio_pop: UP
05-15 01:33:26.342   511  1034 I audio_pop: down
05-15 01:33:26.342   511  1034 I audio_pop: 0:up name match mixer state:S1 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 1:up name match mixer state:S1 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 2:up name match mixer state:S2 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 3:up name match mixer state:S2 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 4:up name match mixer state:S3 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 5:up name match mixer state:S3 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 6:up name match mixer state:S4 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 7:up name match mixer state:S4 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 8:up name match mixer state:SP IL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 9:up name match mixer state:SP IR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 0:down match mixer state:S1 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 1:down match mixer state:S1 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 2:down match mixer state:S2 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 3:down match mixer state:S2 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 4:down match mixer state:S3 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 5:down match mixer state:S3 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 6:down match mixer state:S4 OL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 7:down match mixer state:S4 OR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 8:down match mixer state:SP IL SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_pop: 9:down match mixer state:SP IR SWITCH SWITCH
05-15 01:33:26.342   511  1034 I audio_hw_primary: codec_init: volumes_xml is /odm/etc/audio/hi6402/mixer_volumes_KNIGHT_normal.xml
05-15 01:33:26.363   511  1034 I typec_headset_hal: typec_headset_init:filename 
05-15 01:33:26.363   511  1034 I typec_headset_hal: typec_headset_init: doesn't exist
05-15 01:33:26.363   511  1034 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:26.363   511  1034 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:26.363   511  1034 I audio_hw_primary: visualizer_init: visualizer do not supported
05-15 01:33:26.363   511  1034 D cust_interface: cust_open:
05-15 01:33:26.363   511  1034 I cust_interface: cust_open: audio cust file name is libaudio_custom.so
05-15 01:33:26.363   511  1034 D audio_custom: dev_init:
05-15 01:33:26.363   511  1034 W audio_custom: dev_init: can't find cvaa mute flag string, just set false.
05-15 01:33:26.363   511  1034 W audio_custom: dev_init: can't find cvaa mono flag string, just set false.
05-15 01:33:26.363   511  1034 I spk_dev_interface: spk_dev_open: smartpa lib name is libmax98925.so
05-15 01:33:26.363   511  1034 I spk_dev_interface: smartpa_param_init: smartpa algo running on codec dsp, init param
05-15 01:33:26.363   511  1034 I spk_dev_interface: Cannot get symbols _dev_get_R0, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols _dev_set_calibration_value, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols _dev_get_F0, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols _dev_mute, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols _dev_algo_bypass, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols _dev_pa_reg_dump, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: Cannot get symbols dev_get_parameters, use default
05-15 01:33:26.364   511  1034 E spk_dev_interface: Cannot get symbols dev_set_reg_parameters, use default
05-15 01:33:26.364   511  1034 I spk_dev_interface: load_earpa: earpa lib name is libmax98925.so
05-15 01:33:26.364   511  1034 I spk_dev_interface: load_earpa: ear and spk are the same smartpa libmax98925.so
05-15 01:33:26.364   511  1034 E spk_dev_interface: load_hs_pa:get hs_pa lib name error, use default
05-15 01:33:26.364   511  1034 W spk_dev_interface: load_hs_pa:Unknown device name, use default
05-15 01:33:26.369   511  1034 I MAX98925_SPK: open MAX98925_SPK driver successfully return 21
05-15 01:33:26.370   511  1034 I MAX98925_SPK: MAX98925 SPK set dai clock success
05-15 01:33:26.371   511  1034 D dsp_interface: dsp_open:product_name = KNIGHT
05-15 01:33:26.371   511  1034 I dsp_soc : soc_dsp_open: product_name = KNIGHT, dsp_name = hi363x
05-15 01:33:26.371   511  1034 I dsp_soc_ctl: dsp_soc_ctl_open++
05-15 01:33:26.371   511  1034 I dsp_soc_ctl: open /dev/hifi_misc.
05-15 01:33:26.371   511  1034 I dsp_soc_ctl: dsp_soc_ctl_open--
05-15 01:33:26.371   511  1034 I dsp_common: dsp_common_open: product_name = KNIGHT, dsp_name = hi6402
05-15 01:33:26.371   511  1034 V audio_common: get value success, value:maxim|mad
05-15 01:33:26.371   511  1034 I dsp_common: get_dsp_algo_config: get get_config_value succ, algo_config = 0x1
05-15 01:33:26.371   511  1034 I dsp_maxim_ctl: maxim_register register succ
05-15 01:33:26.371   511  1034 I dsp_common: dsp_common_open 0x4 algo disable 
05-15 01:33:26.371   511  1034 I dsp_common: dsp_common_open 0x8 algo disable 
05-15 01:33:26.371   511  1034 I dsp_common: dsp_common_open 0x10 algo disable 
05-15 01:33:26.371   511  1034 D dsp_interface: dsp_init:
05-15 01:33:26.371   511  1034 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:26.371   511  1034 I dsp_codec_ctl: get_screen_rotate: spk_rcv_stereo_support match, return true
05-15 01:33:26.371   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:26.371   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:26.371   511  1034 V dsp_soc_para_ctl: dsp_nv_init:begin
05-15 01:33:26.371   511  1034 V dsp_soc_para_ctl: ap_param_init: dsp_nv_size: 206408, dsp_nv_param: 0x758bba2c00
05-15 01:33:26.371   511  1034 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8bba2c00(low) 0x75(high), result = 0
05-15 01:33:26.371   511  1034 V dsp_soc_para_ctl: clear_hifi_nv: copy to dsp DDR, dsp_nv_size: 206408, dsp_nv_param: 0x0x758bba2c00, copy2dsp_result:0
05-15 01:33:26.371   511  1034 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:26.371   511  1034 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/dts/dts_KNIGHT_normal.xml
05-15 01:33:26.372   511  1034 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:26.372   511  1034 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/mbdrc/mbdrc_KNIGHT_normal.xml
05-15 01:33:26.373   511  1034 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:26.373   511  1034 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/modem/modem_KNIGHT_normal.xml
05-15 01:33:26.382   511  1034 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:26.382   511  1034 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/sws/sws_KNIGHT_normal.xml
05-15 01:33:26.384   511  1034 I dsp_soc_para_ctl: get_sws_3d_param_name:get audio/sws/sws_3d_KNIGHT_normal.cfg failed.
05-15 01:33:26.384   511  1034 I dsp_soc_para_ctl: get_sws_3d_param_name: filename is 
05-15 01:33:26.384   511  1034 I dsp_soc_para_ctl: get_sws_tws_param_name:get audio/sws/sws_tws_KNIGHT_normal.cfg failed.
05-15 01:33:26.384   511  1034 I dsp_soc_para_ctl: get_sws_tws_param_name: filename is 
05-15 01:33:26.384   511  1034 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8bba2c00(low) 0x75(high), result = 0
05-15 01:33:26.384   511  1034 V dsp_soc_para_ctl: copy_nv_to_hifi: copy to dsp DDR except flag, dsp_nv_size: 206408, dsp_nv_param: 0x0x758bba2c00, copy2dsp_result:0
05-15 01:33:26.384   511  1034 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8bba2c00(low) 0x75(high), result = 0
05-15 01:33:26.384   511  1034 V dsp_soc_para_ctl: copy_nv_to_hifi: copy to dsp DDR, dsp_nv_size: 206408, dsp_nv_param: 0x0x758bba2c00, copy2dsp_result:0
05-15 01:33:26.384   511  1034 V dsp_soc_para_ctl: copy_nv_to_hifi:end
05-15 01:33:26.384   511  1034 V dsp_soc_para_ctl: dsp_nv_init:end
05-15 01:33:26.384   511  1034 I dsp_common: dsp_common_init: initialize dsp module
05-15 01:33:26.384   511  1034 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:26.384   511  1034 D dsp_codec_ctl: image_num:6
05-15 01:33:26.384   511  1034 D dsp_codec_ctl: dsp_type:hi6402_2spk dsp_img_list[0]:hi6402
05-15 01:33:26.384   511  1034 D dsp_codec_ctl: dsp_type:hi6402_2spk dsp_img_list[1]:hi6402_2spk
05-15 01:33:26.384   511  1034 E dsp_codec_ctl: open dts file failed!
05-15 01:33:26.384   511  1034 I dsp_codec_ctl: get_smartpakit_dsp_image: use old smartpa img
05-15 01:33:26.384   511  1034 D dsp_codec_ctl: dsp_type:hi6402_2spk, dsp_name:hi6402, dsp_img_name:hifi_6402_2spk.img
05-15 01:33:26.394  1372  1372 D Zygote  : begin preload
05-15 01:33:26.394  1372  1372 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:26.394  1372  1372 I Zygote  : Preloading ICU data...
05-15 01:33:26.398  1372  1372 D Zygote64Timing: BeginIcuCachePinning took to complete: 4ms
05-15 01:33:26.398  1372  1372 I Zygote  : Preloading classes...
05-15 01:33:26.466  1372  1372 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:26.472  1372  1372 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:26.475  1372  1372 I zygote64: Thread[1,tid=1372,Native,Thread*=0x7d278bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:26.476  1372  1372 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:26.476  1372  1372 I zygote64: Thread[1,tid=1372,Native,Thread*=0x7d278bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:26.476  1372  1372 I zygote64: Thread[1,tid=1372,Native,Thread*=0x7d278bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:26.511  1372  1372 I Zygote  : ...preloaded 4715 classes in 113ms.
05-15 01:33:26.512  1372  1372 I zygote64: VMRuntime.preloadDexCaches starting
05-15 01:33:26.540  1372  1372 I zygote64: VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:26.540  1372  1372 I zygote64: VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:26.540  1372  1372 I zygote64: VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:26.540  1372  1372 I zygote64: VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:26.540  1372  1372 I zygote64: VMRuntime.preloadDexCaches finished
05-15 01:33:26.540  1372  1372 D Zygote64Timing: PreloadClasses took to complete: 142ms
05-15 01:33:26.555  1372  1372 I Zygote  : Preloading resources...
05-15 01:33:26.559  1372  1372 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:26.567  1372  1372 I Zygote  : ...preloaded 64 resources in 11ms.
05-15 01:33:26.568  1372  1372 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:26.569  1372  1372 I Zygote  : ...preloaded 41 resources in 2ms.
05-15 01:33:26.569  1372  1372 D Zygote64Timing: PreloadResources took to complete: 29ms
05-15 01:33:26.584  1372  1372 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:26.594  1372  1372 I Zygote  : Preloading shared libraries...
05-15 01:33:26.600  1372  1372 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:26.601  1372  1372 I Zygote  : Installed AndroidKeyStoreProvider in 0ms.
05-15 01:33:26.605  1372  1372 I Zygote  : Warmed up JCA providers in 5ms.
05-15 01:33:26.605  1372  1372 D Zygote  : end preload
05-15 01:33:26.605  1372  1372 D Zygote64Timing: ZygotePreload took to complete: 211ms
05-15 01:33:26.614  1372  1372 I zygote64: Explicit concurrent copying GC freed 29303(2MB) AllocSpace objects, 25(476KB) LOS objects, 80% free, 1524KB/7MB, paused 30us total 9.357ms
05-15 01:33:26.622  1372  1372 I zygote64: Explicit concurrent copying GC freed 5435(198KB) AllocSpace objects, 0(0B) LOS objects, 81% free, 1357KB/7MB, paused 21us total 5.912ms
05-15 01:33:26.622  1372  1372 D Zygote64Timing: PostZygoteInitGC took to complete: 17ms
05-15 01:33:26.622  1372  1372 D Zygote64Timing: ZygoteInit took to complete: 228ms
05-15 01:33:26.742  1372  1372 I zygote64: Global filter of size 170 installed
05-15 01:33:26.764  1372  1372 I Zygote  : System server process 1415 has been created
05-15 01:33:26.764  1372  1372 E Zygote  : couldn't write 1415 to /dev/memcg/system/tasks
05-15 01:33:26.766  1372  1372 I Zygote  : Accepting command socket connections
05-15 01:33:26.771  1415  1415 I chatty  : uid=1000 system_server expire 145 lines
05-15 01:33:26.786  1415  1415 I SystemServer: InitBeforeStartServices
05-15 01:33:26.786  1415  1415 I SystemServer: Entered the Android system server!
05-15 01:33:26.849   733   733 W Binder:733_1: type=1400 audit(0.0:148): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:26.849   733   733 W Binder:733_1: type=1400 audit(0.0:149): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:26.855  1415  1415 D SystemServerTiming: InitBeforeStartServices took to complete: 69ms
05-15 01:33:26.855  1415  1415 I SystemServer: StartServices
05-15 01:33:26.855  1415  1415 I SystemServer: Reading configuration...
05-15 01:33:26.855  1415  1415 I SystemServer: ReadingSystemConfig
05-15 01:33:26.855  1415  1415 D SystemServerTiming: ReadingSystemConfig took to complete: 0ms
05-15 01:33:26.855  1415  1415 I SystemServer: StartInstaller
05-15 01:33:26.855  1415  1415 I SystemServiceManager: Starting com.android.server.pm.Installer
05-15 01:33:26.855  1415  1428 D SystemServerInitThreadPool: Started executing ReadingSystemConfig
05-15 01:33:26.857  1415  1415 D SystemServerTiming: StartInstaller took to complete: 2ms
05-15 01:33:26.857  1415  1415 I SystemServer: DeviceIdentifiersPolicyService
05-15 01:33:26.857  1415  1415 I SystemServiceManager: Starting com.android.server.os.DeviceIdentifiersPolicyService
05-15 01:33:26.857  1415  1415 D SystemServerTiming: DeviceIdentifiersPolicyService took to complete: 0ms
05-15 01:33:26.857  1415  1415 I SystemServer: StartActivityManager
05-15 01:33:26.857  1415  1415 I SystemServiceManager: Starting com.android.server.am.ActivityManagerService$Lifecycle
05-15 01:33:26.864  1415  1428 D SystemServerInitThreadPool: Finished executing ReadingSystemConfig
05-15 01:33:26.865  1415  1415 I ActivityManager: Memory class: 384
05-15 01:33:26.865  1415  1430 I ServiceThread: Enabled StrictMode logging for ActivityManager looper.
05-15 01:33:26.866  1415  1431 I ServiceThread: Enabled StrictMode logging for android.ui looper.
05-15 01:33:26.874  1415  1415 D BatteryStatsImpl: Reading daily items from /data/system/batterystats-daily.xml
05-15 01:33:26.875  1415  1433 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:26.876  1415  1433 E BatteryExternalStatsWorker: no controller energy info supplied for telephony
05-15 01:33:26.877  1415  1433 E KernelUidCpuFreqTimeReader: Failed to read /proc/uid_time_in_state: java.io.FileNotFoundException: /proc/uid_time_in_state (No such file or directory)
05-15 01:33:26.910  1415  1415 I AppOps  : No existing app ops /data/system/appops.xml; starting empty
05-15 01:33:26.912  1415  1415 I IntentFirewall: Read new rules (A:0 B:0 S:0)
05-15 01:33:26.913  1415  1437 I ServiceThread: Enabled StrictMode logging for android.display looper.
05-15 01:33:26.917  1415  1415 D AppOps  : AppOpsService published
05-15 01:33:26.917  1415  1415 D SystemServerTiming: StartActivityManager took to complete: 60ms
05-15 01:33:26.917  1415  1415 I SystemServer: StartPowerManager
05-15 01:33:26.917  1415  1415 I SystemServiceManager: Starting com.android.server.power.PowerManagerService
05-15 01:33:26.918  1415  1439 I ServiceThread: Enabled StrictMode logging for PowerManagerService looper.
05-15 01:33:26.919  1415  1415 D SystemServerTiming: StartPowerManager took to complete: 2ms
05-15 01:33:26.919  1415  1415 I SystemServer: InitPowerManagement
05-15 01:33:26.920  1415  1415 D SystemServerTiming: InitPowerManagement took to complete: 0ms
05-15 01:33:26.920  1415  1415 I SystemServer: StartRecoverySystemService
05-15 01:33:26.920  1415  1415 I SystemServiceManager: Starting com.android.server.RecoverySystemService
05-15 01:33:26.920  1415  1415 D SystemServerTiming: StartRecoverySystemService took to complete: 1ms
05-15 01:33:26.920  1415  1415 V RescueParty: Disabled because of active USB connection
05-15 01:33:26.920  1415  1415 I SystemServer: StartLightsService
05-15 01:33:26.920  1415  1415 I SystemServiceManager: Starting com.android.server.lights.LightsService
05-15 01:33:26.920  1415  1415 D SystemServerTiming: StartLightsService took to complete: 0ms
05-15 01:33:26.921  1415  1415 I SystemServer: StartDisplayManager
05-15 01:33:26.921  1415  1415 I SystemServiceManager: Starting com.android.server.display.DisplayManagerService
05-15 01:33:26.921  1415  1415 D SystemServerTiming: StartDisplayManager took to complete: 1ms
05-15 01:33:26.921  1415  1415 I SystemServer: WaitForDisplay
05-15 01:33:26.922  1415  1415 I SystemServiceManager: Starting phase 100
05-15 01:33:26.923  1415  1437 I DisplayManagerService: Display device added: DisplayDeviceInfo{"Built-in Screen": uniqueId="local:0", 1080 x 1920, modeId 1, defaultModeId 1, supportedModes [{id=1, width=1080, height=1920, fps=60.000004}], colorMode 0, supportedColorModes [0], HdrCapabilities android.view.Display$HdrCapabilities@1d6308, density 480, 365.76 x 366.676 dpi, appVsyncOff 2000000, presDeadline 13666666, touch INTERNAL, rotation 0, type BUILT_IN, state UNKNOWN, FLAG_DEFAULT_DISPLAY, FLAG_ROTATES_WITH_CONTENT, FLAG_SECURE, FLAG_SUPPORTS_PROTECTED_BUFFERS}
05-15 01:33:26.925   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:26.927  1415  1415 D SystemServerTiming: WaitForDisplay took to complete: 6ms
05-15 01:33:26.927  1415  1437 I DisplayManagerService: Display device changed state: "Built-in Screen", ON
05-15 01:33:26.927  1415  1415 I SystemServer: StartPackageManagerService
05-15 01:33:26.931  1415  1415 D SELinuxMMAC: Using policy file /system/etc/selinux/plat_mac_permissions.xml
05-15 01:33:26.932  1415  1415 D SELinuxMMAC: Using policy file /vendor/etc/selinux/nonplat_mac_permissions.xml
05-15 01:33:26.963  1415  1415 W PackageManager: Failed to parse /system/framework/arm: Missing base APK in /system/framework/arm
05-15 01:33:26.963  1415  1415 W PackageManager: Failed to parse /system/framework/arm64: Missing base APK in /system/framework/arm64
05-15 01:33:26.963  1415  1415 W PackageManager: Failed to parse /system/framework/oat: Missing base APK in /system/framework/oat
05-15 01:33:27.008  1415  1415 I PackageManager: Finished scanning system apps. Time: 48 ms, packageCount: 94 , timePerPackage: 0 , cached: 94
05-15 01:33:27.009  1415  1415 I PackageManager: Finished scanning non-system apps. Time: 0 ms, packageCount: 0 , timePerPackage: 0 , cached: 0
05-15 01:33:27.010  1415  1415 I PackageManager: Time to scan packages: 0.05 seconds
05-15 01:33:27.011  1415  1415 V PackageManager: reconcileAppsData for null u0 0x3 migrateAppData=true
05-15 01:33:27.040  1415  1415 V PackageManager: reconcileAppsData finished 21 packages
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:27.041  1415  1455 D SystemServerInitThreadPool: Started executing prepareAppData
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:27.041  1415  1415 V PackageManager: Disabling com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to disable com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:27.041  1415  1415 V PackageManager: Enabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to enable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:27.041  1415  1415 V PackageManager: Enabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:27.041  1415  1415 W PackageManager: Unable to enable com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:27.042   733   760 W installd: Ignoring /data/data/com.android.webview/lib with unexpected GID 0 instead of 10038
05-15 01:33:27.043   733   760 W installd: Ignoring /data/data/com.svox.pico/lib with unexpected GID 0 instead of 10045
05-15 01:33:27.045  1415  1455 D SystemServerTimingAsync: AppDataFixup took to complete: 4ms
05-15 01:33:27.066  1415  1415 D PackageManager: Ephemeral resolver not found with new action; try old one
05-15 01:33:27.066  1415  1415 D PackageManager: Ephemeral resolver NOT found; no matching intent filters
05-15 01:33:27.066  1415  1415 D PackageManager: Ephemeral installer not found with new action; try old one
05-15 01:33:27.066  1415  1415 D PackageManager: Clear ephemeral installer activity
05-15 01:33:27.091  1415  1415 D SystemServerTiming: StartPackageManagerService took to complete: 164ms
05-15 01:33:27.091  1415  1415 I SystemServer: StartOtaDexOptService
05-15 01:33:27.092  1415  1415 D OTADexopt: No upgrade, skipping A/B artifacts check.
05-15 01:33:27.092  1415  1415 D SystemServerTiming: StartOtaDexOptService took to complete: 1ms
05-15 01:33:27.092  1415  1415 I SystemServer: StartUserManagerService
05-15 01:33:27.092  1415  1415 I SystemServiceManager: Starting com.android.server.pm.UserManagerService$LifeCycle
05-15 01:33:27.092  1415  1415 D SystemServerTiming: StartUserManagerService took to complete: 0ms
05-15 01:33:27.092  1415  1415 I SystemServer: InitAttributerCache
05-15 01:33:27.092  1415  1415 D SystemServerTiming: InitAttributerCache took to complete: 0ms
05-15 01:33:27.093  1415  1415 I SystemServer: SetSystemProcess
05-15 01:33:27.096   536   536 I lowmemorykiller: ActivityManager connected
05-15 01:33:27.097  1415  1415 D SystemServerTiming: SetSystemProcess took to complete: 4ms
05-15 01:33:27.097  1415  1457 I ServiceThread: Enabled StrictMode logging for android.anim looper.
05-15 01:33:27.097  1415  1415 I SystemServer: StartOverlayManagerService
05-15 01:33:27.098  1415  1415 I SystemServer: StartSubstratumService
05-15 01:33:27.098  1415  1458 D SystemServerInitThreadPool: Started executing Init OverlayManagerService
05-15 01:33:27.099  1415  1415 D SystemServerTiming: StartSubstratumService took to complete: 1ms
05-15 01:33:27.099  1415  1415 I SystemServer: StartDropBoxManager
05-15 01:33:27.099  1415  1459 D SystemServerInitThreadPool: Started executing StartSensorService
05-15 01:33:27.099  1415  1415 I SystemServiceManager: Starting com.android.server.DropBoxManagerService
05-15 01:33:27.099  1415  1459 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:27.100  1415  1415 D SystemServerTiming: StartDropBoxManager took to complete: 1ms
05-15 01:33:27.100  1415  1415 I SystemServer: StartBatteryService
05-15 01:33:27.100  1415  1415 I SystemServiceManager: Starting com.android.server.BatteryService
05-15 01:33:27.101  1298  1315 E /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: ISensors::poll() re-entry. I do not know what to do except killing myself.
05-15 01:33:27.107  1415  1415 D SystemServerTiming: StartBatteryService took to complete: 7ms
05-15 01:33:27.107  1415  1415 I SystemServer: StartUsageService
05-15 01:33:27.108  1415  1415 I SystemServiceManager: Starting com.android.server.usage.UsageStatsService
05-15 01:33:27.108  1415  1427 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:27.112  1415  1415 D SystemServerTiming: StartUsageService took to complete: 5ms
05-15 01:33:27.112  1415  1415 I SystemServer: StartWebViewUpdateService
05-15 01:33:27.112  1415  1415 I SystemServiceManager: Starting com.android.server.webkit.WebViewUpdateService
05-15 01:33:27.113  1415  1415 D SystemServerTiming: StartWebViewUpdateService took to complete: 1ms
05-15 01:33:27.114  1415  1415 I SystemServer: StartKeyAttestationApplicationIdProviderService
05-15 01:33:27.114  1415  1428 D SystemServerInitThreadPool: Started executing SecondaryZygotePreload
05-15 01:33:27.114  1415  1428 I SystemServer: SecondaryZygotePreload
05-15 01:33:27.115  1415  1415 D SystemServerTiming: StartKeyAttestationApplicationIdProviderService took to complete: 1ms
05-15 01:33:27.115  1415  1415 I SystemServer: StartKeyChainSystemService
05-15 01:33:27.116  1415  1415 I SystemServiceManager: Starting com.android.server.security.KeyChainSystemService
05-15 01:33:27.116  1415  1415 D SystemServerTiming: StartKeyChainSystemService took to complete: 1ms
05-15 01:33:27.116  1415  1415 I SystemServer: StartSchedulingPolicyService
05-15 01:33:27.116  1415  1415 D SystemServerTiming: StartSchedulingPolicyService took to complete: 0ms
05-15 01:33:27.116  1415  1415 I SystemServer: StartTelecomLoaderService
05-15 01:33:27.116  1415  1415 I SystemServiceManager: Starting com.android.server.telecom.TelecomLoaderService
05-15 01:33:27.117  1415  1415 D SystemServerTiming: StartTelecomLoaderService took to complete: 0ms
05-15 01:33:27.117  1415  1415 I SystemServer: StartTelephonyRegistry
05-15 01:33:27.119  1415  1415 D SystemServerTiming: StartTelephonyRegistry took to complete: 1ms
05-15 01:33:27.119  1415  1415 I SystemServer: StartEntropyMixer
05-15 01:33:27.120  1415  1415 I EntropyMixer: Writing entropy...
05-15 01:33:27.123  1461  1461 I chatty  : uid=1000(system) /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service expire 62 lines
05-15 01:33:27.125  1415  1428 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:27.126  1415  1415 D SystemServerTiming: StartEntropyMixer took to complete: 6ms
05-15 01:33:27.126  1415  1415 I SystemServer: StartAccountManagerService
05-15 01:33:27.126  1415  1415 I SystemServiceManager: Starting com.android.server.accounts.AccountManagerService$Lifecycle
05-15 01:33:27.129  1415  1415 D SystemServerTiming: StartAccountManagerService took to complete: 3ms
05-15 01:33:27.129  1415  1415 I SystemServer: StartContentService
05-15 01:33:27.129  1415  1415 I SystemServiceManager: Starting com.android.server.content.ContentService$Lifecycle
05-15 01:33:27.130  1415  1415 D SystemServerTiming: StartContentService took to complete: 1ms
05-15 01:33:27.130  1415  1415 I SystemServer: InstallSystemProviders
05-15 01:33:27.146  1415  1415 I SettingsState: No settings state /data/system/users/0/settings_ssaid.xml
05-15 01:33:27.146  1415  1428 E SystemServer: Unable to preload default resources
05-15 01:33:27.146  1415  1428 D SystemServerTimingAsync: SecondaryZygotePreload took to complete: 32ms
05-15 01:33:27.146  1415  1428 D SystemServerInitThreadPool: Finished executing SecondaryZygotePreload
05-15 01:33:27.148  1415  1415 D SystemServerTiming: InstallSystemProviders took to complete: 18ms
05-15 01:33:27.148  1415  1415 I SystemServer: StartVibratorService
05-15 01:33:27.152  1415  1415 D SystemServerTiming: StartVibratorService took to complete: 4ms
05-15 01:33:27.152  1415  1415 I SystemServer: StartConsumerIrService
05-15 01:33:27.153  1415  1415 E System  : ******************************************
05-15 01:33:27.154  1415  1415 E System  : ************ Failure starting core service
05-15 01:33:27.154  1415  1415 E System  : java.lang.RuntimeException: IR HAL present, but FEATURE_CONSUMER_IR is not set!
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.server.ConsumerIrService.<init>(ConsumerIrService.java:54)
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:831)
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.154  1415  1415 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.154  1415  1415 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.154  1415  1415 I SystemServer: StartInputMethodManagerLifecycle
05-15 01:33:27.154  1415  1415 I SystemServiceManager: Starting com.android.server.InputMethodManagerService$Lifecycle
05-15 01:33:27.157  1415  1415 D SystemServerTiming: StartInputMethodManagerLifecycle took to complete: 4ms
05-15 01:33:27.157  1415  1415 I SystemServer: StartAccessibilityManagerService
05-15 01:33:27.159   733   733 W Binder:733_5: type=1400 audit(0.0:150): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:27.159   733   733 W Binder:733_5: type=1400 audit(0.0:153): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:27.159  1415  1415 D SystemServerTiming: StartAccessibilityManagerService took to complete: 1ms
05-15 01:33:27.159  1415  1415 I SystemServer: MakeDisplayReady
05-15 01:33:27.159  1415  1415 W SystemServer: ***********************************************
05-15 01:33:27.159  1415  1415 E SystemServer: BOOT FAILURE making display ready
05-15 01:33:27.159  1415  1415 E SystemServer: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.wm.WindowManagerService.displayReady()' on a null object reference
05-15 01:33:27.159  1415  1415 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:947)
05-15 01:33:27.159  1415  1415 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.159  1415  1415 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.159  1415  1415 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.159  1415  1415 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.159  1415  1415 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.159  1415  1415 D SystemServerTiming: MakeDisplayReady took to complete: 0ms
05-15 01:33:27.159  1415  1415 I SystemServer: StartStorageManagerService
05-15 01:33:27.159  1415  1415 I SystemServiceManager: Starting com.android.server.StorageManagerService$Lifecycle
05-15 01:33:27.163  1415  1415 D SystemServerTiming: StartStorageManagerService took to complete: 4ms
05-15 01:33:27.163  1415  1415 I SystemServer: StartStorageStatsService
05-15 01:33:27.163  1415  1469 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:27.163  1415  1415 I SystemServiceManager: Starting com.android.server.usage.StorageStatsService$Lifecycle
05-15 01:33:27.163  1415  1469 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:27.164  1415  1469 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:27.164  1415  1469 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:27.164  1415  1469 D CryptdConnector: SND -> {1 cryptfs getfield SystemLocale}
05-15 01:33:27.166  1415  1415 D SystemServerTiming: StartStorageStatsService took to complete: 3ms
05-15 01:33:27.166  1415  1415 I SystemServer: StartUiModeManager
05-15 01:33:27.166  1415  1415 I SystemServiceManager: Starting com.android.server.UiModeManagerService
05-15 01:33:27.167  1415  1471 D CryptdConnector: RCV <- {200 1 -1}
05-15 01:33:27.168  1415  1469 W StorageManagerService: No primary storage mounted!
05-15 01:33:27.168  1415  1469 D VoldConnector: SND -> {1 asec list}
05-15 01:33:27.168  1415  1470 D VoldConnector: RCV <- {200 1 asec operation succeeded}
05-15 01:33:27.168  1415  1469 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:27.191  1415  1469 W StorageManagerService: No primary storage mounted!
05-15 01:33:27.191  1415  1469 D VoldConnector: SND -> {2 asec list}
05-15 01:33:27.191  1415  1428 D SystemServerInitThreadPool: Started executing UiModeManager.onStart
05-15 01:33:27.191  1415  1428 I ActivityManager: Config changes=200 {1.0 ?mcc?mnc [en_US] ldltr ?swdp ?wdp ?hdp ?density ?lsize ?long ?ldr ?wideColorGamut ?orien ?touch ?keyb/?/? ?nav/? s.2}
05-15 01:33:27.193  1415  1429 I UsageStatsService: User[0] Rollover scheduled @ 2018-05-16 01:33:27(1526434407191)
05-15 01:33:27.193  1415  1429 E AppIdleHistory: Unable to read app idle file for user 0
05-15 01:33:27.193  1415  1470 D VoldConnector: RCV <- {200 2 asec operation succeeded}
05-15 01:33:27.194  1415  1415 D SystemServerTiming: StartUiModeManager took to complete: 28ms
05-15 01:33:27.194  1415  1415 I SystemServer: UpdatePackagesIfNeeded
05-15 01:33:27.194  1415  1415 D SystemServerTiming: UpdatePackagesIfNeeded took to complete: 0ms
05-15 01:33:27.194  1415  1415 I SystemServer: PerformFstrimIfNeeded
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: Failure in UiModeManager.onStart: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityStackSupervisor.getDisplayOverrideConfiguration(ActivityStackSupervisor.java:488)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.performDisplayOverrideConfigUpdate(ActivityManagerService.java:20762)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateGlobalConfiguration(ActivityManagerService.java:20669)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfigurationLocked(ActivityManagerService.java:20547)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfiguration(ActivityManagerService.java:20486)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.sendConfigurationLocked(UiModeManagerService.java:478)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.lambda$-com_android_server_UiModeManagerService_9177(UiModeManagerService.java:236)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.$m$4(Unknown Source:4)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.run(Unknown Source:27)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.SystemServerInitThreadPool.lambda$-com_android_server_SystemServerInitThreadPool_2249(SystemServerInitThreadPool.java:64)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.$m$2(Unknown Source:8)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.run(Unknown Source:19)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:457)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1162)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:636)
05-15 01:33:27.195  1415  1428 E SystemServerInitThreadPool: 	at com.android.internal.util.ConcurrentUtils$1$1.run(ConcurrentUtils.java:59)
05-15 01:33:27.195  1415  1415 D SystemServerTiming: PerformFstrimIfNeeded took to complete: 0ms
05-15 01:33:27.195  1415  1415 I SystemServer: StartLockSettingsService
05-15 01:33:27.195  1415  1415 I SystemServiceManager: Starting com.android.server.locksettings.LockSettingsService$Lifecycle
05-15 01:33:27.198  1415  1458 D SystemServerInitThreadPool: Finished executing Init OverlayManagerService
05-15 01:33:27.200  1415  1415 D SystemServerTiming: StartLockSettingsService took to complete: 5ms
05-15 01:33:27.201  1415  1415 I OemLock : OemLock HAL not present on device
05-15 01:33:27.201  1415  1415 I SystemServer: StartDeviceIdleController
05-15 01:33:27.201  1415  1415 I SystemServiceManager: Starting com.android.server.DeviceIdleController
05-15 01:33:27.203  1415  1415 D SystemServerTiming: StartDeviceIdleController took to complete: 2ms
05-15 01:33:27.203  1415  1415 I SystemServer: StartDevicePolicyManager
05-15 01:33:27.203  1415  1415 I SystemServiceManager: Starting com.android.server.devicepolicy.DevicePolicyManagerService$Lifecycle
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-8 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 8, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-11 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 11, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-12 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 12, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-13 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 13, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-14 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 14, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-15 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 15, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-17 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 17, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-18 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 18, enabled:0, err: 0
05-15 01:33:27.205  1461  1461 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-21 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:27.205  1461  1461 D SensorHub: Channel activate-> handle: 21, enabled:0, err: 0
05-15 01:33:27.206  1415  1479 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:27.206  1415  1459 D SystemServerTimingAsync: StartSensorService took to complete: 107ms
05-15 01:33:27.206  1415  1459 D SystemServerInitThreadPool: Finished executing StartSensorService
05-15 01:33:27.206  1415  1415 D SystemServerTiming: StartDevicePolicyManager took to complete: 3ms
05-15 01:33:27.206  1415  1480 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:27.206  1415  1415 I SystemServer: StartStatusBarManagerService
05-15 01:33:27.207  1415  1415 D SystemServerTiming: StartStatusBarManagerService took to complete: 1ms
05-15 01:33:27.207  1415  1415 I SystemServer: StartClipboardService
05-15 01:33:27.207  1415  1415 I SystemServiceManager: Starting com.android.server.clipboard.ClipboardService
05-15 01:33:27.208  1415  1415 D SystemServerTiming: StartClipboardService took to complete: 1ms
05-15 01:33:27.208  1415  1415 I SystemServer: StartNetworkManagementService
05-15 01:33:27.210  1415  1481 I NetworkManagement: onDaemonConnected()
05-15 01:33:27.210  1415  1415 D SystemServerTiming: StartNetworkManagementService took to complete: 2ms
05-15 01:33:27.210  1415  1415 I SystemServer: StartTextServicesManager
05-15 01:33:27.211  1415  1415 I SystemServiceManager: Starting com.android.server.TextServicesManagerService$Lifecycle
05-15 01:33:27.215  1415  1415 D SystemServerTiming: StartTextServicesManager took to complete: 4ms
05-15 01:33:27.215  1415  1415 I SystemServer: StartNetworkScoreService
05-15 01:33:27.216  1415  1415 D SystemServerTiming: StartNetworkScoreService took to complete: 1ms
05-15 01:33:27.216  1415  1415 I SystemServer: StartNetworkStatsService
05-15 01:33:27.220  1415  1415 W SystemServer: ***********************************************
05-15 01:33:27.220  1415  1415 E SystemServer: BOOT FAILURE starting NetworkStats Service
05-15 01:33:27.220  1415  1415 E SystemServer: java.lang.NullPointerException: missing AlarmManager
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.server.net.NetworkStatsService.<init>(NetworkStatsService.java:309)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:289)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.220  1415  1415 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.220  1415  1415 D SystemServerTiming: StartNetworkStatsService took to complete: 4ms
05-15 01:33:27.220  1415  1415 I SystemServer: StartNetworkPolicyManagerService
05-15 01:33:27.221  1415  1415 W SystemServer: ***********************************************
05-15 01:33:27.222  1415  1415 E SystemServer: BOOT FAILURE starting NetworkPolicy Service
05-15 01:33:27.222  1415  1415 E SystemServer: java.lang.NullPointerException: missing networkStats
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:501)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:487)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1096)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.222  1415  1415 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.222  1415  1415 D SystemServerTiming: StartNetworkPolicyManagerService took to complete: 2ms
05-15 01:33:27.222  1415  1415 I SystemServer: StartWifi
05-15 01:33:27.223  1415  1415 I SystemServiceManager: Starting com.android.server.wifi.WifiService
05-15 01:33:27.259  1376  1393 D CommandListener: Clearing all IP addresses on wlan0
05-15 01:33:27.259  1415  1488 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:27.265  1415  1415 D SystemServerTiming: StartWifi took to complete: 43ms
05-15 01:33:27.265  1415  1415 I SystemServer: StartWifiScanning
05-15 01:33:27.265  1415  1415 I SystemServiceManager: Starting com.android.server.wifi.scanner.WifiScanningService
05-15 01:33:27.267  1415  1415 D SystemServerTiming: StartWifiScanning took to complete: 2ms
05-15 01:33:27.267  1415  1415 I SystemServer: StartWifiRtt
05-15 01:33:27.268  1415  1415 I SystemServiceManager: Starting com.android.server.wifi.RttService
05-15 01:33:27.268  1415  1415 D SystemServerTiming: StartWifiRtt took to complete: 1ms
05-15 01:33:27.268  1415  1415 I SystemServer: No Wi-Fi Aware Service (Aware support Not Present)
05-15 01:33:27.268  1415  1415 I SystemServer: StartWifiP2P
05-15 01:33:27.268  1415  1415 I SystemServiceManager: Starting com.android.server.wifi.p2p.WifiP2pService
05-15 01:33:27.272  1415  1415 D SystemServerTiming: StartWifiP2P took to complete: 4ms
05-15 01:33:27.272  1415  1415 I SystemServer: StartEthernet
05-15 01:33:27.272  1415  1415 I SystemServiceManager: Starting com.android.server.ethernet.EthernetService
05-15 01:33:27.275  1415  1415 D SystemServerTiming: StartEthernet took to complete: 3ms
05-15 01:33:27.275  1415  1415 I SystemServer: StartConnectivityService
05-15 01:33:27.278  1415  1415 D ConnectivityService: ConnectivityService starting up
05-15 01:33:27.278  1415  1415 W SystemServer: ***********************************************
05-15 01:33:27.279  1415  1415 E SystemServer: BOOT FAILURE starting Connectivity Service
05-15 01:33:27.279  1415  1415 E SystemServer: java.lang.NullPointerException: missing INetworkStatsService
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:722)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:690)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1151)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.279  1415  1415 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.279  1415  1415 D SystemServerTiming: StartConnectivityService took to complete: 4ms
05-15 01:33:27.279  1415  1415 I SystemServer: StartNsdService
05-15 01:33:27.280  1415  1415 D NsdService: Network service discovery is enabled
05-15 01:33:27.281  1415  1415 D SystemServerTiming: StartNsdService took to complete: 2ms
05-15 01:33:27.281  1415  1415 I SystemServer: StartUpdateLockService
05-15 01:33:27.281  1415  1415 D SystemServerTiming: StartUpdateLockService took to complete: 0ms
05-15 01:33:27.281  1415  1415 I SystemServer: WaitForAsecScan
05-15 01:33:27.282  1415  1415 D SystemServerTiming: WaitForAsecScan took to complete: 0ms
05-15 01:33:27.282  1415  1415 I SystemServer: StartNotificationManager
05-15 01:33:27.282  1415  1455 D SystemServerTimingAsync: AppDataPrepare took to complete: 237ms
05-15 01:33:27.282  1415  1455 I PackageManager: Deferred reconcileAppsData finished 73 packages
05-15 01:33:27.282  1415  1455 D SystemServerInitThreadPool: Finished executing prepareAppData
05-15 01:33:27.282  1415  1415 I SystemServiceManager: Starting com.android.server.notification.NotificationManagerService
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: codec_adsp_send_sync_cmd:ioctl ret=0
05-15 01:33:27.294   511  1034 D dsp_maxim_ctl: maxim_init:
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_screen_rotate: spk_rcv_stereo_support match, return true
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:27.294   511  1034 I dsp_codec_para_ctl: speaker id:2
05-15 01:33:27.294   511  1034 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:27.294   511  1034 I dsp_codec_para_ctl: receiver id:0
05-15 01:33:27.294   511  1034 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:27.298   511  1034 I dsp_codec_para_ctl: match_devicebox: maxim parameters match SPEAKER
05-15 01:33:27.298   511  1034 I dsp_codec_para_ctl: parse_vendor: maxim parameters match vendor GEER
05-15 01:33:27.298   511  1034 I dsp_codec_para_ctl: match_devicebox: maxim parameters match RECEIVER
05-15 01:33:27.298   511  1034 I dsp_codec_para_ctl: parse_vendor: maxim parameters match vendor DEFAULT
05-15 01:33:27.299   511  1034 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:27.299   511  1034 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:27.300  1415  1415 D ConditionProviders.SCP: new ScheduleConditionProvider()
05-15 01:33:27.301  1415  1415 I ConditionProviders:  Allowing condition provider org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:27.301  1415  1415 I NotificationListeners:  Allowing notification listener org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:27.302  1415  1415 I ConditionProviders:  Allowing condition provider com.android.camera2
05-15 01:33:27.302  1415  1415 D ZenLog  : set_zen_mode: off,init
05-15 01:33:27.303   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:27.303   346   346 E         : 
05-15 01:33:27.303   511  1034 I dsp_codec_para_ctl: get_nv_data_stereo_smartpa : nv_value 6.263091,30.175679 , get RDC value rdc_L 6.263091 rdc_R 30.175679
05-15 01:33:27.303   511  1034 I dsp_codec_para_ctl: get_index_for_RDC_ID index 16
05-15 01:33:27.303   511  1034 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:27.306   511  1034 I dsp_maxim_ctl: [maxim_param_adjust_range_get] get stereo adjust_range value is 4.000000 9.000000 20.000000 40.000000.
05-15 01:33:27.307   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:27.307   346   346 E         : 
05-15 01:33:27.307   511  1034 I spk_dev_interface: spk_set_calibration_value: set calibration value rdc_l: 6.263091
05-15 01:33:27.307   511  1034 I audio_maintain_tools: asd_open: DLOPEN successful for libasd.so
05-15 01:33:27.307   511  1034 I asd     : [asd_dev_open] enter 
05-15 01:33:27.307   511  1034 I asd     : load_dmd_sharelib: dmd_sharelib has loaded, skip!
05-15 01:33:27.307   511  1034 I asd     : [asd_dev_open] exit 
05-15 01:33:27.307   511  1034 I audio_hw_primary: create_offload_standby_thread
05-15 01:33:27.307   511  1034 I audio_hw_primary: create_direct_standby_thread
05-15 01:33:27.307   511  1500 I audio_hw_primary: offload_standby_loop: standby loop start...
05-15 01:33:27.307   511  1501 I audio_hw_primary: direct_standby_loop: standby loop start...
05-15 01:33:27.307   511  1034 I audio_hw_primary: not support multi mic
05-15 01:33:27.308   511  1034 W DeviceHAL: Device 0x758ba2f000 get_master_volume: Function not implemented
05-15 01:33:27.308   511  1034 W DeviceHAL: Device 0x758ba2f000 get_master_mute: Function not implemented
05-15 01:33:27.308   511  1034 W DeviceHAL: Device 0x758ba2f000 set_master_volume: Function not implemented
05-15 01:33:27.308   511  1034 W DeviceHAL: Device 0x758ba2f000 set_master_mute: Function not implemented
05-15 01:33:27.308  1373  1373 I AudioFlinger: loadHwModule() Loaded primary audio interface, handle 10
05-15 01:33:27.308  1373  1373 I AudioFlinger: openOutput() this 0xf1dbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 2
05-15 01:33:27.309  1373  1373 I AudioFlinger: HAL output buffer size 960 frames, normal sink buffer size 960 frames
05-15 01:33:27.310  1373  1373 I BufferProvider: found effect "Multichannel Downmix To Stereo" from The Android Open Source Project
05-15 01:33:27.310  1373  1504 I AudioFlinger: AudioFlinger's thread 0xf1627f40 tid=1504 ready to run
05-15 01:33:27.310  1373  1504 W AudioFlinger: no wake lock to update, system not ready yet
05-15 01:33:27.310   526   526 D lights  : set_light_notification colorRGB=00000000, onMS=0, offMS=0
05-15 01:33:27.310  1373  1373 I AudioFlinger: Using module 10 as the primary audio interface
05-15 01:33:27.310   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 0,  out_device: 0
05-15 01:33:27.310   511  1034 I audio_hw_primary: set mode from 0 to 0
05-15 01:33:27.310  1373  1373 W AudioFlinger: moveEffects() bad srcOutput 0
05-15 01:33:27.311  1373  1504 W AudioFlinger: no wake lock to update, system not ready yet
05-15 01:33:27.311   511  1034 I audio_hw_primary: out_set_parameters_no_lock device:0x2, out type:0
05-15 01:33:27.311   511  1034 D dsp_interface: dsp_set_device: call_m0_standby = 1, device = 0x2, device_mask = 0x00000000
05-15 01:33:27.311   511  1034 E dsp_soc : soc_dsp_set_usb_power_resume: usbaudio power resume failed ioctl:-1 sr_status:0
05-15 01:33:27.311   511  1034 E dsp_interface: dsp_set_usb_power_resume: fail
05-15 01:33:27.311   511  1034 D dsp_soc : set device [2] [0] [succ]
05-15 01:33:27.311   511  1034 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:27.311   511  1034 I audio_hw_primary: select_devices++ mode[0]
05-15 01:33:27.311   511  1034 I audio_hw_primary: select_devices--
05-15 01:33:27.311   511  1361 I audio_hw_primary: adev_set_voice_volume volume: 0.
05-15 01:33:27.312  1373  1373 I AudioFlinger: openOutput() this 0xf1dbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 100
05-15 01:33:27.312   511  1034 E audio_hw_primary: adev open output stream, unsupported flags:0x100
05-15 01:33:27.312   511  1034 W DeviceHAL: Device 0x758ba2f000 open_output_stream: Invalid argument
05-15 01:33:27.312  1373  1373 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -22
05-15 01:33:27.312  1373  1373 W APM_AudioPolicyManager: Cannot open output stream for device 00000002 on hw module primary
05-15 01:33:27.312  1373  1373 I AudioFlinger: openOutput() this 0xf1dbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 8
05-15 01:33:27.312   511  1034 E audio_hw_primary: adev open output stream, unsupported flags:0x8
05-15 01:33:27.312   511  1034 W DeviceHAL: Device 0x758ba2f000 open_output_stream: Invalid argument
05-15 01:33:27.312  1373  1373 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -22
05-15 01:33:27.312  1373  1373 W APM_AudioPolicyManager: Cannot open output stream for device 00000002 on hw module primary
05-15 01:33:27.312  1373  1373 I AudioFlinger: openOutput() this 0xf1dbd000, module 10 Device 10000, SamplingRate 48000, Format 0x000001, Channels 3, flags 0
05-15 01:33:27.312   511  1034 E audio_hw_primary: adev->outputs[0x0] already existed
05-15 01:33:27.312   511  1034 W DeviceHAL: Device 0x758ba2f000 open_output_stream: Device or resource busy
05-15 01:33:27.312  1373  1373 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -61
05-15 01:33:27.312  1373  1373 W APM_AudioPolicyManager: Cannot open output stream for device 00010000 on hw module primary
05-15 01:33:27.312   511  1034 I audio_hw_primary: update config period size 960
05-15 01:33:27.312   511  1034 I audio_hw_primary: change channel_mask form 80000007 to AUDIO_CHANNEL_IN_STEREO
05-15 01:33:27.312  1415  1415 E System  : ******************************************
05-15 01:33:27.312  1415  1415 E System  : ************ Failure starting system services
05-15 01:33:27.312  1415  1415 E System  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:27.312  1415  1415 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:27.312  1415  1415 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.312  1415  1415 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.312  1415  1415 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.312  1415  1415 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.312  1415  1415 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.313  1415  1415 D SystemServerTiming: StartNotificationManager took to complete: 31ms
05-15 01:33:27.313  1415  1415 E Zygote  : System zygote died with exception
05-15 01:33:27.313  1415  1415 E Zygote  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:27.313  1415  1415 E Zygote  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:27.313  1415  1415 E Zygote  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.313  1415  1415 E Zygote  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.313  1415  1415 E Zygote  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.313  1415  1415 E Zygote  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.313  1415  1415 E Zygote  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.313  1415  1415 D AndroidRuntime: Shutting down VM
05-15 01:33:27.313  1415  1415 E AndroidRuntime: *** FATAL EXCEPTION IN SYSTEM PROCESS: main
05-15 01:33:27.313  1415  1415 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:27.313  1415  1415 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:27.313  1373  1506 I AudioFlinger: AudioFlinger's thread 0xf1203840 tid=1506 ready to run
05-15 01:33:27.313   511  1034 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:27.313   511  1034 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:27.313   511  1034 D dsp_soc : set source 0 succ
05-15 01:33:27.313   511  1034 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:27.313   511  1361 I audio_hw_primary: update config period size 960
05-15 01:33:27.313   511  1361 I audio_hw_primary: change channel_mask form 80000007 to AUDIO_CHANNEL_IN_STEREO
05-15 01:33:27.313  1415  1415 I Process : Sending signal. PID: 1415 SIG: 9
05-15 01:33:27.314  1373  1508 I AudioFlinger: AudioFlinger's thread 0xf1203900 tid=1508 ready to run
05-15 01:33:27.314   511  1361 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:27.314   511  1361 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:27.314   511  1034 I audio_hw_primary: update config period size 960
05-15 01:33:27.314   511  1361 D dsp_soc : set source 0 succ
05-15 01:33:27.314   511  1361 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:27.315  1373  1510 I AudioFlinger: AudioFlinger's thread 0xf1203280 tid=1510 ready to run
05-15 01:33:27.315   511  1034 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:27.315   511  1034 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:27.315   511  1034 D dsp_soc : set source 0 succ
05-15 01:33:27.315   511  1034 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:27.317  1373  1373 I bt_a2dp_hw: adev_open:  adev_open in A2dp_hw module
05-15 01:33:27.317  1373  1373 I AudioFlinger: loadHwModule() Loaded a2dp audio interface, handle 18
05-15 01:33:27.318   511  1034 D vndksupport: Loading /vendor/lib64/hw/audio.usb.default.so from current namespace instead of sphal namespace.
05-15 01:33:27.318  1373  1373 I AudioFlinger: loadHwModule() Loaded usb audio interface, handle 26
05-15 01:33:27.318   511  1034 D vndksupport: Loading /vendor/lib64/hw/audio.r_submix.default.so from current namespace instead of sphal namespace.
05-15 01:33:27.318   511  1034 I r_submix: adev_open(name=audio_hw_if)
05-15 01:33:27.318   511  1034 I r_submix: adev_init_check()
05-15 01:33:27.319   511  1034 W DeviceHAL: Device 0x758bb35400 set_master_mute: Function not implemented
05-15 01:33:27.319  1373  1373 I AudioFlinger: loadHwModule() Loaded r_submix audio interface, handle 34
05-15 01:33:27.319   511  1034 D r_submix: adev_open_input_stream(addr=0)
05-15 01:33:27.319   511  1034 D r_submix: submix_audio_device_create_pipe_l(addr=0, idx=9)
05-15 01:33:27.319   511  1034 D r_submix:   now using address 0 for route 9
05-15 01:33:27.319  1373  1514 I AudioFlinger: AudioFlinger's thread 0xf1203f80 tid=1514 ready to run
05-15 01:33:27.319   511  1034 D r_submix: adev_close_input_stream()
05-15 01:33:27.319   511  1034 D r_submix: submix_audio_device_release_pipe_l(idx=9) addr=0
05-15 01:33:27.319   511  1034 D r_submix: submix_audio_device_destroy_pipe_l(): pipe destroyed
05-15 01:33:27.319  1373  1373 W APM_AudioPolicyManager: Output device 00010000 unreachable
05-15 01:33:27.319  1373  1373 E EffectsConfig: Failed to parse /vendor/etc/audio_effects.xml: Tinyxml2 error (3): /vendor/etc/audio_effects.xml (null)
05-15 01:33:27.319  1373  1373 W AudioPolicyEffects: Failed to load XML effect configuration, fallback to .conf
05-15 01:33:27.321   511  1034 I soundtrigger_hw: stdev_get_properties
05-15 01:33:27.321  1373  1373 I SoundTriggerHalHidl: getProperties res implementor The Android Open Source Project
05-15 01:33:27.321  1373  1373 I SoundTriggerHalHidl: getProperties ret 0
05-15 01:33:27.321  1373  1373 I SoundTriggerHwService: loaded default module Volantis OK Google , handle 1
05-15 01:33:27.362   536   536 I lowmemorykiller: ActivityManager disconnected
05-15 01:33:27.362   536   536 I lowmemorykiller: Closing Activity Manager data connection
05-15 01:33:27.362   384   384 I chatty  : uid=1000(system) /system/bin/servicemanager expire 22 lines
05-15 01:33:27.363  1372  1372 E Zygote  : Exit zygote because system server (1415) has terminated
05-15 01:33:27.363   384   384 I ServiceManager: service 'procstats' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'meminfo' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'gfxinfo' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'dbinfo' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'cpuinfo' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'permission' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'processinfo' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'otadexopt' died
05-15 01:33:27.363  1372  1372 F libc    : Fatal signal 6 (SIGABRT), code 0 in tid 1372 (main), pid 1372 (main)
05-15 01:33:27.363   384   384 I ServiceManager: service 'package_native' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'package' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'overlay' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'dropbox' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'battery' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'usagestats' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'webviewupdate' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'sec_key_att_app_id_provider' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'scheduling_policy' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'telephony.registry' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'account' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'content' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'settings' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'sensorservice' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'device_identifiers' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'batterystats' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'appops' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'power' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'recovery' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'display' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'user' died
05-15 01:33:27.363   384   384 I ServiceManager: service 'activity' died
05-15 01:33:27.383  1518  1518 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-15 01:33:27.383   751   751 I /system/bin/tombstoned: received crash request for pid 1372
05-15 01:33:27.384  1518  1518 I crash_dump64: performing dump of process 1372 (target tid = 1372)
05-15 01:33:27.384  1518  1518 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-15 01:33:27.384  1518  1518 F DEBUG   : LineageOS Version: 'unknown'
05-15 01:33:27.384  1518  1518 F DEBUG   : Build fingerprint: 'Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys'
05-15 01:33:27.384  1518  1518 F DEBUG   : Revision: '0'
05-15 01:33:27.384  1518  1518 F DEBUG   : ABI: 'arm64'
05-15 01:33:27.384  1518  1518 F DEBUG   : pid: 1372, tid: 1372, name: main  >>> zygote64 <<<
05-15 01:33:27.384  1518  1518 F DEBUG   : signal 6 (SIGABRT), code 0 (SI_USER), fault addr --------
05-15 01:33:27.384  1518  1518 F DEBUG   :     x0   0000000000000000  x1   0000000000000009  x2   0000000000000005  x3   0000000000000003
05-15 01:33:27.384  1518  1518 F DEBUG   :     x4   0000000040100401  x5   a802a00080404000  x6   0000000000000000  x7   7f7f7f7f7f7f7f7f
05-15 01:33:27.384  1518  1518 F DEBUG   :     x8   0000000000000081  x9   f5744751a921f802  x10  0000007fe9d86be0  x11  0000000000000038
05-15 01:33:27.384  1518  1518 F DEBUG   :     x12  000000000000000b  x13  ffffffffffffffff  x14  ff00000000000000  x15  ffffffffffffffff
05-15 01:33:27.384  1518  1518 F DEBUG   :     x16  0000007dab06e300  x17  0000007daa4cc55c  x18  0000000070215150  x19  0000007dac460a50
05-15 01:33:27.384  1518  1518 F DEBUG   :     x20  0000007dab01a1e6  x21  0000007dab01a64a  x22  0000007dab01a6a6  x23  0000000000000587
05-15 01:33:27.384  1518  1518 F DEBUG   :     x24  0000007dab01a68e  x25  0000007dab01a669  x26  0000007dac460a40  x27  000000000000000b
05-15 01:33:27.384  1518  1518 F DEBUG   :     x28  0000007dab073000  x29  0000007fe9d871b0  x30  0000007daafd400c
05-15 01:33:27.384  1518  1518 F DEBUG   :     sp   0000007fe9d87150  pc   0000007daa4cc564  pstate 0000000060000000
05-15 01:33:27.619  1518  1518 F DEBUG   : 
05-15 01:33:27.619  1518  1518 F DEBUG   : backtrace:
05-15 01:33:27.619  1518  1518 F DEBUG   :     #00 pc 000000000006a564  /system/lib64/libc.so (kill+8)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #01 pc 0000000000176008  /system/lib64/libandroid_runtime.so ((anonymous namespace)::SigChldHandler(int)+280)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #02 pc 00000000000005f0  [vdso:0000007dac2f5000]
05-15 01:33:27.619  1518  1518 F DEBUG   :     #03 pc 0000000000069ea0  /system/lib64/libc.so (__ppoll+4)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #04 pc 00000000000265e4  /system/lib64/libc.so (poll+88)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #05 pc 000000000002e9a8  /system/lib64/libjavacore.so (Linux_poll(_JNIEnv*, _jobject*, _jobjectArray*, int)+800)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #06 pc 000000000030bad0  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.Linux.fcntlVoid [DEDUPED]+160)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #07 pc 0000000000300a74  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.BlockGuardOs.poll+228)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #08 pc 00000000002b67a4  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (android.system.Os.poll+84)
05-15 01:33:27.619  1518  1518 F DEBUG   :     #09 pc 000000000164e488  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteServer.runSelectLoop+664)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #10 pc 0000000001652ed8  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteInit.main+2728)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #11 pc 000000000054744c  /system/lib64/libart.so (art_quick_invoke_static_stub+604)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #12 pc 00000000000dc7b0  /system/lib64/libart.so (art::ArtMethod::Invoke(art::Thread*, unsigned int*, unsigned int, art::JValue*, char const*)+260)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #13 pc 000000000046bb70  /system/lib64/libart.so (art::InvokeWithArgArray(art::ScopedObjectAccessAlreadyRunnable const&, art::ArtMethod*, art::ArgArray*, art::JValue*, char const*)+100)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #14 pc 000000000046b79c  /system/lib64/libart.so (art::InvokeWithVarArgs(art::ScopedObjectAccessAlreadyRunnable const&, _jobject*, _jmethodID*, std::__va_list)+420)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #15 pc 0000000000372a54  /system/lib64/libart.so (art::JNI::CallStaticVoidMethodV(_JNIEnv*, _jclass*, _jmethodID*, std::__va_list)+620)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #16 pc 00000000000a6fb8  /system/lib64/libandroid_runtime.so (_JNIEnv::CallStaticVoidMethod(_jclass*, _jmethodID*, ...)+120)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #17 pc 00000000000a9728  /system/lib64/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+832)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #18 pc 0000000000002440  /system/bin/app_process64 (main+1328)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #19 pc 00000000000a14d4  /system/lib64/libc.so (__libc_init+88)
05-15 01:33:27.625  1518  1518 F DEBUG   :     #20 pc 0000000000001e70  /system/bin/app_process64 (_start_main+80)
05-15 01:33:27.758  1518  1518 E crash_dump64: unable to connect to activity manager: No such file or directory
05-15 01:33:27.759   751   751 E /system/bin/tombstoned: Tombstone written to: /data/tombstones/tombstone_01
05-15 01:33:27.825   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 0,  out_device: 0x2
05-15 01:33:27.825   511  1034 I audio_hw_primary: adev_close
05-15 01:33:27.825   384   384 I ServiceManager: service 'media.audio_flinger' died
05-15 01:33:27.825   384   384 I ServiceManager: service 'media.audio_policy' died
05-15 01:33:27.825   384   384 I ServiceManager: service 'media.sound_trigger_hw' died
05-15 01:33:27.825   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 4,  out_device: 0x2
05-15 01:33:27.825   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 5,  out_device: 0x2
05-15 01:33:27.825   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 6,  out_device: 0x2
05-15 01:33:27.825   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 7,  out_device: 0x2
05-15 01:33:27.825   511  1034 I audio_hw_primary: destroy_offload_standby_thread
05-15 01:33:27.825   511  1500 I audio_hw_primary: offload_standby_loop: wait standby_cond succ
05-15 01:33:27.830   384   384 I ServiceManager: service 'media.camera' died
05-15 01:33:27.836   384   384 I ServiceManager: service 'media.player' died
05-15 01:33:27.836   384   384 I ServiceManager: service 'media.resource_manager' died
05-15 01:33:27.841   384   384 I ServiceManager: service 'netd' died
05-15 01:33:27.846   384   384 I ServiceManager: service 'wificond' died
05-15 01:33:28.000   511  1339 E audio_hw_primary: direct_standby_loop: adev->outputs[OUTPUT_DIRECT] is NULL
05-15 01:33:28.000   511  1339 I audio_hw_primary: direct_standby_loop: standby loop exit...
05-15 01:33:28.000   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 4,  out_device: 0x2
05-15 01:33:28.000   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 5,  out_device: 0x2
05-15 01:33:28.000   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 6,  out_device: 0x2
05-15 01:33:28.000   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 7,  out_device: 0x2
05-15 01:33:28.000   511   904 E typec_headset_hal: typec_headset_uninit:already null so no need to free
05-15 01:33:28.000   511   904 D dsp_interface: dsp_close:
05-15 01:33:28.000   511   904 I dsp_soc_ctl: dsp_soc_ctl_close++
05-15 01:33:28.000   511   904 I dsp_soc_ctl: close /dev/hifi_misc.
05-15 01:33:28.000   511   904 I dsp_soc_ctl: dsp_soc_ctl_close--
05-15 01:33:28.000   511   904 I MAX98925_SPK: maxim smartpa close
05-15 01:33:29.031  1529  1529 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:29.032  1528  1528 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:29.033  1528  1528 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:29.033  1528  1528 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:29.033  1528  1528 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:29.034  1529  1529 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:29.035  1529  1529 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:30.000   511  1500 E audio_hw_primary: offload_standby_loop: adev->outputs[OUTPUT_OFFLOAD] is NULL
05-15 01:33:30.000   511  1500 I audio_hw_primary: offload_standby_loop: standby loop exit...
05-15 01:33:30.000   511  1034 I audio_hw_primary: destroy_direct_standby_thread
05-15 01:33:30.000   511  1501 I audio_hw_primary: direct_standby_loop: wait standby_cond succ
05-15 01:33:31.170  1539  1539 I Netd    : Netd 1.0 starting
05-15 01:33:31.170  1539  1539 D TetherController: Setting IP forward enable = 0
05-15 01:33:31.177  1540  1540 I wificond: wificond is starting up...
05-15 01:33:31.193  1536  1536 I FastMixerState: sMaxFastTracks = 8
05-15 01:33:31.193  1541  1541 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:31.193  1541  1541 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:31.193  1541  1541 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:31.193  1541  1541 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:31.193  1541  1541 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:31.195  1536  1536 I audioserver: ServiceManager: 0xe7c97940
05-15 01:33:31.195  1536  1536 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:31.198  1541  1541 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:31.199  1539  1539 I Netd    : Creating child chains: 14.8ms
05-15 01:33:31.199  1539  1539 I Netd    : Setting up OEM hooks: 0.1ms
05-15 01:33:31.199  1541  1541 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:31.199  1541  1541 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:31.199  1536  1536 I AudioFlinger: Using default 3000 mSec as standby time.
05-15 01:33:31.202  1536  1536 E APM::Serializer: deserialize: Could not parse /odm/etc/audio_policy_configuration.xml document.
05-15 01:33:31.203  1539  1539 I Netd    : Setting up FirewallController hooks: 4.7ms
05-15 01:33:31.205  1539  1539 I Netd    : Setting up NatController hooks: 2.0ms
05-15 01:33:31.208  1539  1539 I Netd    : Setting up BandwidthController hooks: 2.1ms
05-15 01:33:31.208  1539  1539 I Netd    : Setting up IdletimerController hooks: 0.1ms
05-15 01:33:31.209   511   904 D vndksupport: Loading /vendor/lib64/hw/audio.primary.hisi.so from current namespace instead of sphal namespace.
05-15 01:33:31.210   511   904 I audio_hw_primary: adev_open:
05-15 01:33:31.210   511   904 I audio_hw_primary: offload mode is enable
05-15 01:33:31.211  1539  1539 I Netd    : Disabling bandwidth control: 3.1ms
05-15 01:33:31.212  1539  1539 E Netd    : cannot find interface dummy0
05-15 01:33:31.213  1539  1539 I Netd    : Initializing RouteController: 1.8ms
05-15 01:33:31.213  1539  1539 E Netd    : Unable to create netlink socket: Protocol not supported
05-15 01:33:31.213  1539  1539 W Netd    : Unable to open qlog quota socket, check if xt_quota2 can send via UeventHandler
05-15 01:33:31.214  1539  1539 D MDnsDS  : MDnsSdListener::Hander starting up
05-15 01:33:31.215  1539  1559 D MDnsDS  : MDnsSdListener starting to monitor
05-15 01:33:31.215  1539  1559 D MDnsDS  : Going to poll with pollCount 1
05-15 01:33:31.217  1539  1539 I Netd    : Registering NetdNativeService: 1.0ms
05-15 01:33:31.217  1539  1539 I Netd    : Starting CommandListener: 0.1ms
05-15 01:33:31.218  1539  1539 I Netd    : Registering NetdHwService: 1.5ms
05-15 01:33:31.218  1539  1539 I Netd    : Netd started in 48ms
05-15 01:33:31.219  1537  1537 W cameraserver: type=1400 audit(0.0:154): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2092 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:31.219  1537  1537 W cameraserver: type=1400 audit(0.0:155): avc: denied { read } for name="hw" dev="mmcblk0p52" ino=2295 scontext=u:r:cameraserver:s0 tcontext=u:object_r:system_file:s0 tclass=dir permissive=0
05-15 01:33:31.221  1537  1537 I cameraserver: ServiceManager: 0xf3f179a0
05-15 01:33:31.221  1537  1537 I CameraService: CameraService started (pid=1537)
05-15 01:33:31.221  1537  1537 I CameraService: CameraService process starting
05-15 01:33:31.221  1537  1537 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:31.221  1537  1537 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:31.224  1537  1537 E vndksupport: Could not load /vendor/lib/hw/android.hardware.camera.provider@2.4-impl.so from sphal namespace: dlopen failed: library "android.hardware.camera.device@1.0.so" not found.
05-15 01:33:31.224  1537  1537 E /system/bin/cameraserver: Failed to dlopen android.hardware.camera.provider@2.4-impl.so: unknown error
05-15 01:33:31.234   346   346 E         : pid 511, opration oeminfo_read OK
05-15 01:33:31.234   346   346 E         : 
05-15 01:33:31.234   511   904 I audio_config: get_vendor_info: vendor_country_info = all/cn
05-15 01:33:31.234   511   904 V audio_common: get value success, value:KNIGHT
05-15 01:33:31.234   511   904 I audio_config: get_audio_configs: get product_name succ, product_name = KNIGHT
05-15 01:33:31.234   511   904 V audio_common: get value success, value:audio_custom
05-15 01:33:31.234   511   904 I audio_config: get_audio_configs: get cust_name succ, cust_name = audio_custom
05-15 01:33:31.235   511   904 V audio_common: get value success, value:max98925
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get spk_pa_name succ, spk_pa_name = max98925
05-15 01:33:31.235   511   904 V audio_common: get value success, value:hi363x
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get soc_name succ, soc_name = hi363x
05-15 01:33:31.235   511   904 V audio_common: get value success, value:hi6402
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get codec_name succ, codec_name = hi6402
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get mic_name not succ, set mic_name = none as default
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get hs_pa_name not succ, set hs_pa_name = none as default
05-15 01:33:31.235   511   904 V audio_common: get value success, value:true
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get modem_sio_master succ, modem_sio_master = 1
05-15 01:33:31.235   511   904 V audio_common: get value success, value:max98925
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get ear_pa_name succ, ear_pa_name = max98925
05-15 01:33:31.235   511   904 V audio_common: get value success, value:true
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get vqm function enable succ, vqm function enable = 1
05-15 01:33:31.235   511   904 V audio_common: get value success, value:true
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get bwe function support succ, bwe function support = 1
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 W audio_config: get_audio_configs: get swb function support not succ, set swb function support = 0 as default
05-15 01:33:31.235   511   904 V audio_common: get value success, value:false
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get multi mic function enable succ, multi_mic_enable = 0
05-15 01:33:31.235   511   904 V audio_common: get value success, value:true
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get dual_smartpa_support function support succ, dual_smartpa_support function support = true
05-15 01:33:31.235   511   904 V audio_common: get value success, value:0.0
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get dual_smartpa_verison = 0.0 succ.
05-15 01:33:31.235   511   904 V audio_common: get value success, value:false
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get voice_anc_support function support succ, voice_anc_support function support = flase
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 W audio_config: get_audio_configs: get visualizer_support fail, set visualizer_support as false
05-15 01:33:31.235   511   904 V audio_common: get value success, value:true
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get asr feature enable succ, asr_enable = 1
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 V audio_common: get value success, value:ok
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get soundtrigger feature enable succ, soundtrigger_enable = 1
05-15 01:33:31.235   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.235   511   904 W audio_config: get_audio_configs: get spk_num not succ, set spk_num = 1 as default
05-15 01:33:31.235   511   904 V audio_common: get value success, value:speaker
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get speaker_test_content succ, speaker_test_content = speaker
05-15 01:33:31.235   511   904 V audio_common: get value success, value:1
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get smartpa_info pa_num succ, pa_num = 1
05-15 01:33:31.235   511   904 V audio_common: get value success, value:0
05-15 01:33:31.235   511   904 I audio_config: get_audio_configs: get smartpa_info algo_in succ, algo_in = 0
05-15 01:33:31.236   511   904 V audio_common: get value success, value:0001
05-15 01:33:31.236   511   904 I audio_config: get_audio_configs: get smartpa_info pa_type succ, pa_type = 1
05-15 01:33:31.236   511   904 V audio_common: get value success, value:false
05-15 01:33:31.236   511   904 I audio_config: get_audio_configs: get audio sar function support succ, sar_support = 0
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 I audio_config: get_audio_configs: use default max stream volume
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_config: get_audio_ir_configs: get analog earpiece function enable not succ, set analog_earpiece  enable = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 I audio_config: get_audio_configs: get codec stub not succ, set codec stub = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 I audio_config: get_karaoke_mic_configs:karaoke mic configuration support = NA
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 I audio_config: get_smartpa_latency_configs: smartpa latency use default 0
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_config: get_audio_hifi_info_configs: get extern headset hifi function enable not succ, set ext_hs_hifi_enable = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_config: get_audio_hifi_info_configs: get support_dynamic_rate not succ, set support_dynamic_rate = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_config: get_audio_hifi_info_configs: get support_Hperform_Lpower not succ, set support_Hperform_Lpower = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 W audio_config: get_audio_hifi_info_configs: get digital_voice_wakeup_enable not succ, set digital_voice_wakeup_enable = 0 as default
05-15 01:33:31.236   511   904 W audio_common: open dts file failed! May not need in this case
05-15 01:33:31.236   511   904 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:31.236   511  1569 E audio_hw_primary: UEVENT  init fail
05-15 01:33:31.236   511   904 E audio_config: get_para_config_file_print_err:get audio/devicemask/typec_headset_devicemask_KNIGHT.xml failed.
05-15 01:33:31.236   511   904 I audio_hw_primary: codec_init: paths_xml is /odm/etc/audio/hi6402/mixer_paths_KNIGHT.xml
05-15 01:33:31.266  1538  1538 I mediaserver: ServiceManager: 0xeb297a40
05-15 01:33:31.266  1538  1538 W BatteryNotifier: batterystats service unavailable!
05-15 01:33:31.293  1535  1535 D AndroidRuntime: >>>>>> START com.android.internal.os.ZygoteInit uid 0 <<<<<<
05-15 01:33:31.296  1535  1535 I zygote64: option[0]=-Xzygote
05-15 01:33:31.296  1535  1535 I zygote64: option[1]=-Xusetombstonedtraces
05-15 01:33:31.296  1535  1535 I zygote64: option[2]=exit
05-15 01:33:31.296  1535  1535 I zygote64: option[3]=vfprintf
05-15 01:33:31.296  1535  1535 I zygote64: option[4]=sensitiveThread
05-15 01:33:31.296  1535  1535 I zygote64: option[5]=-verbose:gc
05-15 01:33:31.296  1535  1535 I zygote64: option[6]=-Xms8m
05-15 01:33:31.296  1535  1535 I zygote64: option[7]=-Xmx512m
05-15 01:33:31.296  1535  1535 I zygote64: option[8]=-XX:HeapGrowthLimit=384m
05-15 01:33:31.296  1535  1535 I zygote64: option[9]=-XX:HeapMinFree=2m
05-15 01:33:31.296  1535  1535 I zygote64: option[10]=-XX:HeapMaxFree=8m
05-15 01:33:31.296  1535  1535 I zygote64: option[11]=-XX:HeapTargetUtilization=0.75
05-15 01:33:31.296  1535  1535 I zygote64: option[12]=-Xusejit:true
05-15 01:33:31.296  1535  1535 I zygote64: option[13]=-Xjitsaveprofilinginfo
05-15 01:33:31.296  1535  1535 I zygote64: option[14]=-agentlib:jdwp=transport=dt_android_adb,suspend=n,server=y
05-15 01:33:31.296  1535  1535 I zygote64: option[15]=-Xlockprofthreshold:500
05-15 01:33:31.296  1535  1535 I zygote64: option[16]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[17]=--runtime-arg
05-15 01:33:31.296  1535  1535 I zygote64: option[18]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[19]=-Xms64m
05-15 01:33:31.296  1535  1535 I zygote64: option[20]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[21]=--runtime-arg
05-15 01:33:31.296  1535  1535 I zygote64: option[22]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[23]=-Xmx64m
05-15 01:33:31.296  1535  1535 I zygote64: option[24]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[25]=--image-classes=/system/etc/preloaded-classes
05-15 01:33:31.296  1535  1535 I zygote64: option[26]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[27]=--compiled-classes=/system/etc/compiled-classes
05-15 01:33:31.296  1535  1535 I zygote64: option[28]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[29]=--dirty-image-objects=/system/etc/dirty-image-objects
05-15 01:33:31.296  1535  1535 I zygote64: option[30]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[31]=--runtime-arg
05-15 01:33:31.296  1535  1535 I zygote64: option[32]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[33]=-Xms64m
05-15 01:33:31.296  1535  1535 I zygote64: option[34]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[35]=--runtime-arg
05-15 01:33:31.296  1535  1535 I zygote64: option[36]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[37]=-Xmx512m
05-15 01:33:31.296  1535  1535 I zygote64: option[38]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[39]=-j4
05-15 01:33:31.296  1535  1535 I zygote64: option[40]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[41]=-j4
05-15 01:33:31.296  1535  1535 I zygote64: option[42]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[43]=--instruction-set-variant=generic
05-15 01:33:31.296  1535  1535 I zygote64: option[44]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[45]=--instruction-set-variant=generic
05-15 01:33:31.296  1535  1535 I zygote64: option[46]=-Ximage-compiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[47]=--instruction-set-features=default
05-15 01:33:31.296  1535  1535 I zygote64: option[48]=-Xcompiler-option
05-15 01:33:31.296  1535  1535 I zygote64: option[49]=--instruction-set-features=default
05-15 01:33:31.296  1535  1535 I zygote64: option[50]=-Duser.locale=en-US
05-15 01:33:31.296  1535  1535 I zygote64: option[51]=--cpu-abilist=arm64-v8a
05-15 01:33:31.296  1535  1535 I zygote64: option[52]=-Xfingerprint:Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys
05-15 01:33:31.298   511   904 E audio_route: Control 'S4 IF CLK EN' already exists in path 'media-speaker-earpiece'
05-15 01:33:31.298  1535  1535 W zygote64: Incomplete boot detected. Pruning dalvik cache
05-15 01:33:31.298   511   904 E audio_route: Control 'HPDAC_I2V SWITCH' already exists in path 'media-speaker-headset'
05-15 01:33:31.298   511   904 E audio_route: Control 'HPDAC_I2V SWITCH' already exists in path 'media-speaker-headphone'
05-15 01:33:31.298   511   904 E audio_route: Control 'S4 IF CLK EN' already exists in path 'communication-speaker-earpiece'
05-15 01:33:31.298   511   904 E audio_route: Control 'S4 IF CLK EN' already exists in path 'media-fm-speaker-earpiece'
05-15 01:33:31.298   511   904 E audio_route: Control 'S4 IF CLK EN' already exists in path 'dup-call-m0-speaker-earpiece'
05-15 01:33:31.299   511   904 E audio_route: Control 'S4 IF CLK EN' already exists in path 'dup-call-wb-m0-speaker-earpiece'
05-15 01:33:31.299   511   904 E audio_route: unknown enum value string S2L for ctl APR MUX
05-15 01:33:31.299   511   904 I chatty  : uid=1041(audioserver) HwBinder:511_2 identical 5 lines
05-15 01:33:31.300   511   904 E audio_route: unknown enum value string S2L for ctl APR MUX
05-15 01:33:31.300   511   904 I audio_hw_primary: codec_init: pop_seq_xml is /odm/etc/audio/hi6402/pop_seq_KNIGHT.xml
05-15 01:33:31.300   511   904 I audio_pop: UP
05-15 01:33:31.300   511   904 I audio_pop: down
05-15 01:33:31.300   511   904 I audio_pop: 0:up name match mixer state:S1 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 1:up name match mixer state:S1 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 2:up name match mixer state:S2 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 3:up name match mixer state:S2 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 4:up name match mixer state:S3 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 5:up name match mixer state:S3 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 6:up name match mixer state:S4 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 7:up name match mixer state:S4 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 8:up name match mixer state:SP IL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 9:up name match mixer state:SP IR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 0:down match mixer state:S1 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 1:down match mixer state:S1 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 2:down match mixer state:S2 OL SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 3:down match mixer state:S2 OR SWITCH SWITCH
05-15 01:33:31.300   511   904 I audio_pop: 4:down match mixer state:S3 OL SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_pop: 5:down match mixer state:S3 OR SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_pop: 6:down match mixer state:S4 OL SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_pop: 7:down match mixer state:S4 OR SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_pop: 8:down match mixer state:SP IL SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_pop: 9:down match mixer state:SP IR SWITCH SWITCH
05-15 01:33:31.301   511   904 I audio_hw_primary: codec_init: volumes_xml is /odm/etc/audio/hi6402/mixer_volumes_KNIGHT_normal.xml
05-15 01:33:31.321   511   904 I typec_headset_hal: typec_headset_init:filename 
05-15 01:33:31.321   511   904 I typec_headset_hal: typec_headset_init: doesn't exist
05-15 01:33:31.321   511   904 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:31.321   511   904 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:31.321   511   904 I audio_hw_primary: visualizer_init: visualizer do not supported
05-15 01:33:31.321   511   904 D cust_interface: cust_open:
05-15 01:33:31.321   511   904 I cust_interface: cust_open: audio cust file name is libaudio_custom.so
05-15 01:33:31.322   511   904 D audio_custom: dev_init:
05-15 01:33:31.322   511   904 W audio_custom: dev_init: can't find cvaa mute flag string, just set false.
05-15 01:33:31.322   511   904 W audio_custom: dev_init: can't find cvaa mono flag string, just set false.
05-15 01:33:31.322   511   904 I spk_dev_interface: spk_dev_open: smartpa lib name is libmax98925.so
05-15 01:33:31.322   511   904 I spk_dev_interface: smartpa_param_init: smartpa algo running on codec dsp, init param
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_get_R0, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_set_calibration_value, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_get_F0, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_mute, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_algo_bypass, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols _dev_pa_reg_dump, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: Cannot get symbols dev_get_parameters, use default
05-15 01:33:31.322   511   904 E spk_dev_interface: Cannot get symbols dev_set_reg_parameters, use default
05-15 01:33:31.322   511   904 I spk_dev_interface: load_earpa: earpa lib name is libmax98925.so
05-15 01:33:31.322   511   904 I spk_dev_interface: load_earpa: ear and spk are the same smartpa libmax98925.so
05-15 01:33:31.322   511   904 E spk_dev_interface: load_hs_pa:get hs_pa lib name error, use default
05-15 01:33:31.322   511   904 W spk_dev_interface: load_hs_pa:Unknown device name, use default
05-15 01:33:31.328   511   904 I MAX98925_SPK: open MAX98925_SPK driver successfully return 18
05-15 01:33:31.329   511   904 I MAX98925_SPK: MAX98925 SPK set dai clock success
05-15 01:33:31.329   511   904 D dsp_interface: dsp_open:product_name = KNIGHT
05-15 01:33:31.329   511   904 I dsp_soc : soc_dsp_open: product_name = KNIGHT, dsp_name = hi363x
05-15 01:33:31.329   511   904 I dsp_soc_ctl: dsp_soc_ctl_open++
05-15 01:33:31.329   511   904 I dsp_soc_ctl: open /dev/hifi_misc.
05-15 01:33:31.329   511   904 I dsp_soc_ctl: dsp_soc_ctl_open--
05-15 01:33:31.329   511   904 I dsp_common: dsp_common_open: product_name = KNIGHT, dsp_name = hi6402
05-15 01:33:31.329   511   904 V audio_common: get value success, value:maxim|mad
05-15 01:33:31.329   511   904 I dsp_common: get_dsp_algo_config: get get_config_value succ, algo_config = 0x1
05-15 01:33:31.329   511   904 I dsp_maxim_ctl: maxim_register register succ
05-15 01:33:31.329   511   904 I dsp_common: dsp_common_open 0x4 algo disable 
05-15 01:33:31.329   511   904 I dsp_common: dsp_common_open 0x8 algo disable 
05-15 01:33:31.329   511   904 I dsp_common: dsp_common_open 0x10 algo disable 
05-15 01:33:31.329   511   904 D dsp_interface: dsp_init:
05-15 01:33:31.329   511   904 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:31.329   511   904 I dsp_codec_ctl: get_screen_rotate: spk_rcv_stereo_support match, return true
05-15 01:33:31.329   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:31.329   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:31.329   511   904 V dsp_soc_para_ctl: dsp_nv_init:begin
05-15 01:33:31.330   511   904 V dsp_soc_para_ctl: ap_param_init: dsp_nv_size: 206408, dsp_nv_param: 0x758c7baa80
05-15 01:33:31.330   511   904 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8c7baa80(low) 0x75(high), result = 0
05-15 01:33:31.330   511   904 V dsp_soc_para_ctl: clear_hifi_nv: copy to dsp DDR, dsp_nv_size: 206408, dsp_nv_param: 0x0x758c7baa80, copy2dsp_result:0
05-15 01:33:31.330   511   904 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:31.330   511   904 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/dts/dts_KNIGHT_normal.xml
05-15 01:33:31.330   511   904 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:31.330   511   904 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/mbdrc/mbdrc_KNIGHT_normal.xml
05-15 01:33:31.331   511   904 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:31.331   511   904 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/modem/modem_KNIGHT_normal.xml
05-15 01:33:31.341   511   904 I audio_config: get_ce_normal_para: ce_normal_para = normal
05-15 01:33:31.341   511   904 I dsp_soc_para_ctl: get_algo_param_name: filename is /odm/etc/audio/sws/sws_KNIGHT_normal.xml
05-15 01:33:31.342   511   904 I dsp_soc_para_ctl: get_sws_3d_param_name:get audio/sws/sws_3d_KNIGHT_normal.cfg failed.
05-15 01:33:31.342   511   904 I dsp_soc_para_ctl: get_sws_3d_param_name: filename is 
05-15 01:33:31.342   511   904 I dsp_soc_para_ctl: get_sws_tws_param_name:get audio/sws/sws_tws_KNIGHT_normal.cfg failed.
05-15 01:33:31.342   511   904 I dsp_soc_para_ctl: get_sws_tws_param_name: filename is 
05-15 01:33:31.342   511   904 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8c7baa80(low) 0x75(high), result = 0
05-15 01:33:31.342   511   904 V dsp_soc_para_ctl: copy_nv_to_hifi: copy to dsp DDR except flag, dsp_nv_size: 206408, dsp_nv_param: 0x0x758c7baa80, copy2dsp_result:0
05-15 01:33:31.342   511   904 D dsp_soc_ctl: copy_algo_param_to_hifi, param addr = 0x8c7baa80(low) 0x75(high), result = 0
05-15 01:33:31.342   511   904 V dsp_soc_para_ctl: copy_nv_to_hifi: copy to dsp DDR, dsp_nv_size: 206408, dsp_nv_param: 0x0x758c7baa80, copy2dsp_result:0
05-15 01:33:31.342   511   904 V dsp_soc_para_ctl: copy_nv_to_hifi:end
05-15 01:33:31.342   511   904 V dsp_soc_para_ctl: dsp_nv_init:end
05-15 01:33:31.342   511   904 I dsp_common: dsp_common_init: initialize dsp module
05-15 01:33:31.342   511   904 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:31.342   511   904 D dsp_codec_ctl: image_num:6
05-15 01:33:31.342   511   904 D dsp_codec_ctl: dsp_type:hi6402_2spk dsp_img_list[0]:hi6402
05-15 01:33:31.342   511   904 D dsp_codec_ctl: dsp_type:hi6402_2spk dsp_img_list[1]:hi6402_2spk
05-15 01:33:31.342   511   904 E dsp_codec_ctl: open dts file failed!
05-15 01:33:31.342   511   904 I dsp_codec_ctl: get_smartpakit_dsp_image: use old smartpa img
05-15 01:33:31.342   511   904 D dsp_codec_ctl: dsp_type:hi6402_2spk, dsp_name:hi6402, dsp_img_name:hifi_6402_2spk.img
05-15 01:33:31.365  1535  1535 I zygote64: Pruning dalvik-cache since we are relocating an image and will need to recompile
05-15 01:33:31.365  1535  1535 I zygote64: RelocateImage: /system/bin/patchoat --input-image-location=/system/framework/boot.art --output-image-file=/data/dalvik-cache/arm64/system@framework@boot.art --instruction-set=arm64 --base-offset-delta=8220672
05-15 01:33:31.740  1535  1535 D Zygote  : begin preload
05-15 01:33:31.740  1535  1535 I Zygote  : Installing ICU cache reference pinning...
05-15 01:33:31.740  1535  1535 I Zygote  : Preloading ICU data...
05-15 01:33:31.744  1535  1535 D Zygote64Timing: BeginIcuCachePinning took to complete: 5ms
05-15 01:33:31.744  1535  1535 I Zygote  : Preloading classes...
05-15 01:33:31.811  1535  1535 E ActivityRecognitionHardware: activity_recognition HAL is deprecated. class_init is effectively a no-op
05-15 01:33:31.817  1535  1535 W Zygote  : Class not found for preloading: android.icu.impl.number.Parse
05-15 01:33:31.820  1535  1535 I zygote64: Thread[1,tid=1535,Native,Thread*=0x70a86bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:31.820  1535  1535 D MtpDeviceJNI: register_android_mtp_MtpDevice
05-15 01:33:31.820  1535  1535 I zygote64: Thread[1,tid=1535,Native,Thread*=0x70a86bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:31.821  1535  1535 I zygote64: Thread[1,tid=1535,Native,Thread*=0x70a86bfa00,peer=0x12c01d18,"main"] recursive attempt to load library "/system/lib64/libmedia_jni.so"
05-15 01:33:31.855  1535  1535 I Zygote  : ...preloaded 4715 classes in 110ms.
05-15 01:33:31.855  1535  1535 I zygote64: VMRuntime.preloadDexCaches starting
05-15 01:33:31.883  1535  1535 I zygote64: VMRuntime.preloadDexCaches strings total=317139 before=10544 after=10544
05-15 01:33:31.883  1535  1535 I zygote64: VMRuntime.preloadDexCaches types total=26982 before=5654 after=5656
05-15 01:33:31.883  1535  1535 I zygote64: VMRuntime.preloadDexCaches fields total=128271 before=5535 after=5565
05-15 01:33:31.883  1535  1535 I zygote64: VMRuntime.preloadDexCaches methods total=226946 before=10193 after=10193
05-15 01:33:31.883  1535  1535 I zygote64: VMRuntime.preloadDexCaches finished
05-15 01:33:31.883  1535  1535 D Zygote64Timing: PreloadClasses took to complete: 139ms
05-15 01:33:31.898  1535  1535 I Zygote  : Preloading resources...
05-15 01:33:31.902  1535  1535 W Resources: Preloaded drawable resource #0x1080275 (android:drawable/dialog_background_material) that varies with configuration!!
05-15 01:33:31.910  1535  1535 I Zygote  : ...preloaded 64 resources in 12ms.
05-15 01:33:31.911  1535  1535 W Resources: Preloaded color resource #0x1060054 (android:color/btn_default_material_dark) that varies with configuration!!
05-15 01:33:31.912  1535  1535 I Zygote  : ...preloaded 41 resources in 3ms.
05-15 01:33:31.912  1535  1535 D Zygote64Timing: PreloadResources took to complete: 29ms
05-15 01:33:31.927  1535  1535 D libEGL  : loaded /vendor/lib64/egl/libGLES_mali.so
05-15 01:33:31.937  1535  1535 I Zygote  : Preloading shared libraries...
05-15 01:33:31.943  1535  1535 I Zygote  : Uninstalled ICU cache reference pinning...
05-15 01:33:31.944  1535  1535 I Zygote  : Installed AndroidKeyStoreProvider in 1ms.
05-15 01:33:31.948  1535  1535 I Zygote  : Warmed up JCA providers in 4ms.
05-15 01:33:31.948  1535  1535 D Zygote  : end preload
05-15 01:33:31.948  1535  1535 D Zygote64Timing: ZygotePreload took to complete: 209ms
05-15 01:33:31.958  1535  1535 I zygote64: Explicit concurrent copying GC freed 29303(2MB) AllocSpace objects, 25(476KB) LOS objects, 80% free, 1524KB/7MB, paused 30us total 9.400ms
05-15 01:33:31.965  1535  1535 I zygote64: Explicit concurrent copying GC freed 5435(198KB) AllocSpace objects, 0(0B) LOS objects, 81% free, 1357KB/7MB, paused 20us total 6.017ms
05-15 01:33:31.965  1535  1535 D Zygote64Timing: PostZygoteInitGC took to complete: 17ms
05-15 01:33:31.965  1535  1535 D Zygote64Timing: ZygoteInit took to complete: 226ms
05-15 01:33:32.022  1535  1535 I zygote64: Global filter of size 170 installed
05-15 01:33:32.043  1535  1535 I Zygote  : System server process 1580 has been created
05-15 01:33:32.043  1535  1535 E Zygote  : couldn't write 1580 to /dev/memcg/system/tasks
05-15 01:33:32.044  1535  1535 I Zygote  : Accepting command socket connections
05-15 01:33:32.051  1580  1580 I chatty  : uid=1000 system_server expire 149 lines
05-15 01:33:32.065  1580  1580 I SystemServer: InitBeforeStartServices
05-15 01:33:32.066  1580  1580 I SystemServer: Entered the Android system server!
05-15 01:33:32.134  1580  1580 D SystemServerTiming: InitBeforeStartServices took to complete: 69ms
05-15 01:33:32.134  1580  1580 I SystemServer: StartServices
05-15 01:33:32.134  1580  1580 I SystemServer: Reading configuration...
05-15 01:33:32.134  1580  1580 I SystemServer: ReadingSystemConfig
05-15 01:33:32.135  1580  1580 D SystemServerTiming: ReadingSystemConfig took to complete: 1ms
05-15 01:33:32.135  1580  1580 I SystemServer: StartInstaller
05-15 01:33:32.135  1580  1580 I SystemServiceManager: Starting com.android.server.pm.Installer
05-15 01:33:32.135  1580  1593 D SystemServerInitThreadPool: Started executing ReadingSystemConfig
05-15 01:33:32.139   733   733 W Binder:733_1: type=1400 audit(0.0:156): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:32.139   733   733 W Binder:733_1: type=1400 audit(0.0:157): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:32.142  1580  1580 D SystemServerTiming: StartInstaller took to complete: 7ms
05-15 01:33:32.142  1580  1580 I SystemServer: DeviceIdentifiersPolicyService
05-15 01:33:32.142  1580  1580 I SystemServiceManager: Starting com.android.server.os.DeviceIdentifiersPolicyService
05-15 01:33:32.143  1580  1580 D SystemServerTiming: DeviceIdentifiersPolicyService took to complete: 1ms
05-15 01:33:32.143  1580  1580 I SystemServer: StartActivityManager
05-15 01:33:32.143  1580  1580 I SystemServiceManager: Starting com.android.server.am.ActivityManagerService$Lifecycle
05-15 01:33:32.144  1580  1593 D SystemServerInitThreadPool: Finished executing ReadingSystemConfig
05-15 01:33:32.150  1580  1580 I ActivityManager: Memory class: 384
05-15 01:33:32.151  1580  1595 I ServiceThread: Enabled StrictMode logging for ActivityManager looper.
05-15 01:33:32.152  1580  1596 I ServiceThread: Enabled StrictMode logging for android.ui looper.
05-15 01:33:32.159  1580  1580 D BatteryStatsImpl: Reading daily items from /data/system/batterystats-daily.xml
05-15 01:33:32.161  1580  1598 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:32.162  1580  1598 E BatteryExternalStatsWorker: no controller energy info supplied for telephony
05-15 01:33:32.163  1580  1598 E KernelUidCpuFreqTimeReader: Failed to read /proc/uid_time_in_state: java.io.FileNotFoundException: /proc/uid_time_in_state (No such file or directory)
05-15 01:33:32.195  1580  1580 I AppOps  : No existing app ops /data/system/appops.xml; starting empty
05-15 01:33:32.196  1580  1580 I IntentFirewall: Read new rules (A:0 B:0 S:0)
05-15 01:33:32.197  1580  1602 I ServiceThread: Enabled StrictMode logging for android.display looper.
05-15 01:33:32.201  1580  1580 D AppOps  : AppOpsService published
05-15 01:33:32.201  1580  1580 D SystemServerTiming: StartActivityManager took to complete: 58ms
05-15 01:33:32.201  1580  1580 I SystemServer: StartPowerManager
05-15 01:33:32.201  1580  1580 I SystemServiceManager: Starting com.android.server.power.PowerManagerService
05-15 01:33:32.202  1580  1604 I ServiceThread: Enabled StrictMode logging for PowerManagerService looper.
05-15 01:33:32.203  1580  1580 D SystemServerTiming: StartPowerManager took to complete: 2ms
05-15 01:33:32.203  1580  1580 I SystemServer: InitPowerManagement
05-15 01:33:32.204  1580  1580 D SystemServerTiming: InitPowerManagement took to complete: 1ms
05-15 01:33:32.204  1580  1580 I SystemServer: StartRecoverySystemService
05-15 01:33:32.204  1580  1580 I SystemServiceManager: Starting com.android.server.RecoverySystemService
05-15 01:33:32.204  1580  1580 D SystemServerTiming: StartRecoverySystemService took to complete: 0ms
05-15 01:33:32.205  1580  1580 V RescueParty: Disabled because of active USB connection
05-15 01:33:32.205  1580  1580 I SystemServer: StartLightsService
05-15 01:33:32.205  1580  1580 I SystemServiceManager: Starting com.android.server.lights.LightsService
05-15 01:33:32.205  1580  1580 D SystemServerTiming: StartLightsService took to complete: 1ms
05-15 01:33:32.205  1580  1580 I SystemServer: StartDisplayManager
05-15 01:33:32.205  1580  1580 I SystemServiceManager: Starting com.android.server.display.DisplayManagerService
05-15 01:33:32.206  1580  1580 D SystemServerTiming: StartDisplayManager took to complete: 0ms
05-15 01:33:32.206  1580  1580 I SystemServer: WaitForDisplay
05-15 01:33:32.206  1580  1580 I SystemServiceManager: Starting phase 100
05-15 01:33:32.208  1580  1602 I DisplayManagerService: Display device added: DisplayDeviceInfo{"Built-in Screen": uniqueId="local:0", 1080 x 1920, modeId 1, defaultModeId 1, supportedModes [{id=1, width=1080, height=1920, fps=60.000004}], colorMode 0, supportedColorModes [0], HdrCapabilities android.view.Display$HdrCapabilities@1d6308, density 480, 365.76 x 366.676 dpi, appVsyncOff 2000000, presDeadline 13666666, touch INTERNAL, rotation 0, type BUILT_IN, state UNKNOWN, FLAG_DEFAULT_DISPLAY, FLAG_ROTATES_WITH_CONTENT, FLAG_SECURE, FLAG_SUPPORTS_PROTECTED_BUFFERS}
05-15 01:33:32.208   537   537 D SurfaceFlinger: Set power mode=2, type=0 flinger=0x7e7e65f000
05-15 01:33:32.209  1580  1580 D SystemServerTiming: WaitForDisplay took to complete: 3ms
05-15 01:33:32.209  1580  1602 I DisplayManagerService: Display device changed state: "Built-in Screen", ON
05-15 01:33:32.209  1580  1580 I SystemServer: StartPackageManagerService
05-15 01:33:32.214  1580  1580 D SELinuxMMAC: Using policy file /system/etc/selinux/plat_mac_permissions.xml
05-15 01:33:32.214  1580  1580 D SELinuxMMAC: Using policy file /vendor/etc/selinux/nonplat_mac_permissions.xml
05-15 01:33:32.246  1580  1580 W PackageManager: Failed to parse /system/framework/arm: Missing base APK in /system/framework/arm
05-15 01:33:32.246  1580  1580 W PackageManager: Failed to parse /system/framework/oat: Missing base APK in /system/framework/oat
05-15 01:33:32.246  1580  1580 W PackageManager: Failed to parse /system/framework/arm64: Missing base APK in /system/framework/arm64
05-15 01:33:32.256   511   904 I dsp_codec_ctl: codec_adsp_send_sync_cmd:ioctl ret=0
05-15 01:33:32.256   511   904 D dsp_maxim_ctl: maxim_init:
05-15 01:33:32.256   511   904 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_screen_rotate: spk_rcv_stereo_support match, return true
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_num: 1
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_smart_pa_num_stereo_status: get pa_type: 1
05-15 01:33:32.257   511   904 I dsp_codec_para_ctl: speaker id:2
05-15 01:33:32.257   511   904 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:32.257   511   904 I dsp_codec_para_ctl: receiver id:0
05-15 01:33:32.257   511   904 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:32.260   511   904 I dsp_codec_para_ctl: match_devicebox: maxim parameters match SPEAKER
05-15 01:33:32.261   511   904 I dsp_codec_para_ctl: parse_vendor: maxim parameters match vendor GEER
05-15 01:33:32.261   511   904 I dsp_codec_para_ctl: match_devicebox: maxim parameters match RECEIVER
05-15 01:33:32.261   511   904 I dsp_codec_para_ctl: parse_vendor: maxim parameters match vendor DEFAULT
05-15 01:33:32.262   511   904 I dsp_codec_ctl: get_spk_rec_stereo_status: dual_smartpa_support match, return true
05-15 01:33:32.262   511   904 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:32.266   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:32.266   346   346 E         : 
05-15 01:33:32.267   511   904 I dsp_codec_para_ctl: get_nv_data_stereo_smartpa : nv_value 6.263091,30.175679 , get RDC value rdc_L 6.263091 rdc_R 30.175679
05-15 01:33:32.267   511   904 I dsp_codec_para_ctl: get_index_for_RDC_ID index 16
05-15 01:33:32.267   511   904 I dsp_codec_para_ctl: get_algo_param_name: filename is /odm/etc/audio/maxim/maxim_KNIGHT_normal.xml
05-15 01:33:32.270   511   904 I dsp_maxim_ctl: [maxim_param_adjust_range_get] get stereo adjust_range value is 4.000000 9.000000 20.000000 40.000000.
05-15 01:33:32.271   346   346 E         : pid 511, opration nvm_read OK
05-15 01:33:32.271   346   346 E         : 
05-15 01:33:32.271   511   904 I spk_dev_interface: spk_set_calibration_value: set calibration value rdc_l: 6.263091
05-15 01:33:32.271   511   904 I audio_maintain_tools: asd_open: DLOPEN successful for libasd.so
05-15 01:33:32.271   511   904 I asd     : [asd_dev_open] enter 
05-15 01:33:32.271   511   904 I asd     : load_dmd_sharelib: dmd_sharelib has loaded, skip!
05-15 01:33:32.271   511   904 I asd     : [asd_dev_open] exit 
05-15 01:33:32.271   511   904 I audio_hw_primary: create_offload_standby_thread
05-15 01:33:32.271   511   904 I audio_hw_primary: create_direct_standby_thread
05-15 01:33:32.271   511  1616 I audio_hw_primary: offload_standby_loop: standby loop start...
05-15 01:33:32.271   511  1617 I audio_hw_primary: direct_standby_loop: standby loop start...
05-15 01:33:32.272   511   904 I audio_hw_primary: not support multi mic
05-15 01:33:32.272   511   904 W DeviceHAL: Device 0x758ba21000 get_master_volume: Function not implemented
05-15 01:33:32.272   511   904 W DeviceHAL: Device 0x758ba21000 get_master_mute: Function not implemented
05-15 01:33:32.272   511   904 W DeviceHAL: Device 0x758ba21000 set_master_volume: Function not implemented
05-15 01:33:32.272   511   904 W DeviceHAL: Device 0x758ba21000 set_master_mute: Function not implemented
05-15 01:33:32.272  1536  1536 I AudioFlinger: loadHwModule() Loaded primary audio interface, handle 10
05-15 01:33:32.272  1536  1536 I AudioFlinger: openOutput() this 0xe7cbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 2
05-15 01:33:32.273  1536  1536 I AudioFlinger: HAL output buffer size 960 frames, normal sink buffer size 960 frames
05-15 01:33:32.274  1536  1536 I BufferProvider: found effect "Multichannel Downmix To Stereo" from The Android Open Source Project
05-15 01:33:32.274  1536  1620 I AudioFlinger: AudioFlinger's thread 0xe7527dc0 tid=1620 ready to run
05-15 01:33:32.274  1536  1536 I AudioFlinger: Using module 10 as the primary audio interface
05-15 01:33:32.274  1536  1620 W AudioFlinger: no wake lock to update, system not ready yet
05-15 01:33:32.274   511   904 I audio_hw_primary: set mode from 0 to 0
05-15 01:33:32.274   511   904 I audio_hw_primary: do_out_standby standby: 1, stream_type: 0,  out_device: 0
05-15 01:33:32.275  1536  1536 W AudioFlinger: moveEffects() bad srcOutput 0
05-15 01:33:32.275  1536  1620 W AudioFlinger: no wake lock to update, system not ready yet
05-15 01:33:32.275   511   904 I audio_hw_primary: out_set_parameters_no_lock device:0x2, out type:0
05-15 01:33:32.275   511   904 D dsp_interface: dsp_set_device: call_m0_standby = 1, device = 0x2, device_mask = 0x00000000
05-15 01:33:32.275   511   904 E dsp_soc : soc_dsp_set_usb_power_resume: usbaudio power resume failed ioctl:-1 sr_status:0
05-15 01:33:32.275   511   904 E dsp_interface: dsp_set_usb_power_resume: fail
05-15 01:33:32.275   511   904 D dsp_soc : set device [2] [0] [succ]
05-15 01:33:32.275   511   904 I audio_hw_primary: call_get_sample_rate: sample_rate = 16000, tty_status = 0
05-15 01:33:32.275   511   904 I audio_hw_primary: select_devices++ mode[0]
05-15 01:33:32.275   511   904 I audio_hw_primary: select_devices--
05-15 01:33:32.276   511   904 I audio_hw_primary: adev_set_voice_volume volume: 0.
05-15 01:33:32.277  1536  1536 I AudioFlinger: openOutput() this 0xe7cbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 100
05-15 01:33:32.277   511   904 E audio_hw_primary: adev open output stream, unsupported flags:0x100
05-15 01:33:32.277   511   904 W DeviceHAL: Device 0x758ba21000 open_output_stream: Invalid argument
05-15 01:33:32.277  1536  1536 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -22
05-15 01:33:32.277  1536  1536 W APM_AudioPolicyManager: Cannot open output stream for device 00000002 on hw module primary
05-15 01:33:32.277  1536  1536 I AudioFlinger: openOutput() this 0xe7cbd000, module 10 Device 2, SamplingRate 48000, Format 0x000001, Channels 3, flags 8
05-15 01:33:32.277   511   904 E audio_hw_primary: adev open output stream, unsupported flags:0x8
05-15 01:33:32.277   511   904 W DeviceHAL: Device 0x758ba21000 open_output_stream: Invalid argument
05-15 01:33:32.277  1536  1536 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -22
05-15 01:33:32.277  1536  1536 W APM_AudioPolicyManager: Cannot open output stream for device 00000002 on hw module primary
05-15 01:33:32.277  1536  1536 I AudioFlinger: openOutput() this 0xe7cbd000, module 10 Device 10000, SamplingRate 48000, Format 0x000001, Channels 3, flags 0
05-15 01:33:32.277   511   904 E audio_hw_primary: adev->outputs[0x0] already existed
05-15 01:33:32.277   511   904 W DeviceHAL: Device 0x758ba21000 open_output_stream: Device or resource busy
05-15 01:33:32.278  1536  1536 I AudioHwDevice: openOutputStream(), HAL returned sampleRate 48000, Format 0x1, channelMask 0x3, status -61
05-15 01:33:32.278  1536  1536 W APM_AudioPolicyManager: Cannot open output stream for device 00010000 on hw module primary
05-15 01:33:32.278   511   904 I audio_hw_primary: update config period size 960
05-15 01:33:32.278   511   904 I audio_hw_primary: change channel_mask form 80000007 to AUDIO_CHANNEL_IN_STEREO
05-15 01:33:32.278  1536  1622 I AudioFlinger: AudioFlinger's thread 0xe7103480 tid=1622 ready to run
05-15 01:33:32.278   511   904 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:32.278   511   904 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:32.278   511   904 D dsp_soc : set source 0 succ
05-15 01:33:32.278   511   826 I audio_hw_primary: update config period size 960
05-15 01:33:32.278   511   904 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:32.278   511   826 I audio_hw_primary: change channel_mask form 80000007 to AUDIO_CHANNEL_IN_STEREO
05-15 01:33:32.279  1536  1624 I AudioFlinger: AudioFlinger's thread 0xe7103200 tid=1624 ready to run
05-15 01:33:32.279   511   826 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:32.279   511   826 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:32.279   511   826 D dsp_soc : set source 0 succ
05-15 01:33:32.279   511   904 I audio_hw_primary: update config period size 960
05-15 01:33:32.279   511   826 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:32.279  1536  1626 I AudioFlinger: AudioFlinger's thread 0xe71038c0 tid=1626 ready to run
05-15 01:33:32.280   511   904 I audio_hw_primary: do_in_standby standby: 1, in_device: 0
05-15 01:33:32.280   511   904 D dsp_interface: dsp_set_source:source = 0
05-15 01:33:32.280   511   904 D dsp_soc : set source 0 succ
05-15 01:33:32.280   511   904 I dsp_common: dsp_common_set_source:source = 0
05-15 01:33:32.282  1536  1536 I bt_a2dp_hw: adev_open:  adev_open in A2dp_hw module
05-15 01:33:32.283  1536  1536 I AudioFlinger: loadHwModule() Loaded a2dp audio interface, handle 18
05-15 01:33:32.283   511   904 D vndksupport: Loading /vendor/lib64/hw/audio.usb.default.so from current namespace instead of sphal namespace.
05-15 01:33:32.284  1536  1536 I AudioFlinger: loadHwModule() Loaded usb audio interface, handle 26
05-15 01:33:32.284   511   904 D vndksupport: Loading /vendor/lib64/hw/audio.r_submix.default.so from current namespace instead of sphal namespace.
05-15 01:33:32.284   511   904 I r_submix: adev_open(name=audio_hw_if)
05-15 01:33:32.285   511   904 I r_submix: adev_init_check()
05-15 01:33:32.285   511   904 W DeviceHAL: Device 0x7589a14b00 set_master_mute: Function not implemented
05-15 01:33:32.286  1536  1536 I AudioFlinger: loadHwModule() Loaded r_submix audio interface, handle 34
05-15 01:33:32.286   511   904 D r_submix: adev_open_input_stream(addr=0)
05-15 01:33:32.286   511   904 D r_submix: submix_audio_device_create_pipe_l(addr=0, idx=9)
05-15 01:33:32.286   511   904 D r_submix:   now using address 0 for route 9
05-15 01:33:32.286  1536  1634 I AudioFlinger: AudioFlinger's thread 0xe7103480 tid=1634 ready to run
05-15 01:33:32.286   511   904 D r_submix: adev_close_input_stream()
05-15 01:33:32.286   511   904 D r_submix: submix_audio_device_release_pipe_l(idx=9) addr=0
05-15 01:33:32.286   511   904 D r_submix: submix_audio_device_destroy_pipe_l(): pipe destroyed
05-15 01:33:32.286  1536  1536 W APM_AudioPolicyManager: Output device 00010000 unreachable
05-15 01:33:32.286  1536  1536 E EffectsConfig: Failed to parse /vendor/etc/audio_effects.xml: Tinyxml2 error (3): /vendor/etc/audio_effects.xml (null)
05-15 01:33:32.287  1536  1536 W AudioPolicyEffects: Failed to load XML effect configuration, fallback to .conf
05-15 01:33:32.288   511   826 I soundtrigger_hw: stdev_get_properties
05-15 01:33:32.288  1536  1536 I SoundTriggerHalHidl: getProperties res implementor The Android Open Source Project
05-15 01:33:32.289  1536  1536 I SoundTriggerHalHidl: getProperties ret 0
05-15 01:33:32.289  1536  1536 I SoundTriggerHwService: loaded default module Volantis OK Google , handle 1
05-15 01:33:32.293  1580  1580 I PackageManager: Finished scanning system apps. Time: 50 ms, packageCount: 94 , timePerPackage: 0 , cached: 94
05-15 01:33:32.293  1580  1580 I PackageManager: Finished scanning non-system apps. Time: 0 ms, packageCount: 0 , timePerPackage: 0 , cached: 0
05-15 01:33:32.295  1580  1580 I PackageManager: Time to scan packages: 0.052 seconds
05-15 01:33:32.297  1580  1580 V PackageManager: reconcileAppsData for null u0 0x3 migrateAppData=true
05-15 01:33:32.325  1580  1580 V PackageManager: reconcileAppsData finished 21 packages
05-15 01:33:32.326  1580  1636 D SystemServerInitThreadPool: Started executing prepareAppData
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateActivity
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$Receiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateServiceReceiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateActivity
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$Receiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$ActiveReceiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateService$SecretCodeReceiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.gms/com.google.android.gms.update.SystemUpdateServiceReceiver
05-15 01:33:32.326  1580  1580 V PackageManager: Disabling com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to disable com.google.android.setupwizard/com.google.android.setupwizard.time.DateTimeCheck
05-15 01:33:32.326  1580  1580 V PackageManager: Enabling com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to enable com.google.android.gsf/com.google.android.gsf.update.SystemUpdateService
05-15 01:33:32.326  1580  1580 V PackageManager: Enabling com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:32.326  1580  1580 W PackageManager: Unable to enable com.google.android.gms/com.google.android.gms.update.SystemUpdateService
05-15 01:33:32.327   733   760 W installd: Ignoring /data/data/com.android.webview/lib with unexpected GID 0 instead of 10038
05-15 01:33:32.327   733   760 W installd: Ignoring /data/data/com.svox.pico/lib with unexpected GID 0 instead of 10045
05-15 01:33:32.330  1580  1636 D SystemServerTimingAsync: AppDataFixup took to complete: 4ms
05-15 01:33:32.350  1580  1580 D PackageManager: Ephemeral resolver not found with new action; try old one
05-15 01:33:32.350  1580  1580 D PackageManager: Ephemeral resolver NOT found; no matching intent filters
05-15 01:33:32.351  1580  1580 D PackageManager: Ephemeral installer not found with new action; try old one
05-15 01:33:32.351  1580  1580 D PackageManager: Clear ephemeral installer activity
05-15 01:33:32.376  1580  1580 D SystemServerTiming: StartPackageManagerService took to complete: 167ms
05-15 01:33:32.376  1580  1580 I SystemServer: StartOtaDexOptService
05-15 01:33:32.377  1580  1580 D OTADexopt: No upgrade, skipping A/B artifacts check.
05-15 01:33:32.377  1580  1580 D SystemServerTiming: StartOtaDexOptService took to complete: 1ms
05-15 01:33:32.377  1580  1580 I SystemServer: StartUserManagerService
05-15 01:33:32.377  1580  1580 I SystemServiceManager: Starting com.android.server.pm.UserManagerService$LifeCycle
05-15 01:33:32.377  1580  1580 D SystemServerTiming: StartUserManagerService took to complete: 0ms
05-15 01:33:32.377  1580  1580 I SystemServer: InitAttributerCache
05-15 01:33:32.377  1580  1580 D SystemServerTiming: InitAttributerCache took to complete: 0ms
05-15 01:33:32.377  1580  1580 I SystemServer: SetSystemProcess
05-15 01:33:32.380   536   536 I lowmemorykiller: ActivityManager connected
05-15 01:33:32.380  1580  1580 D SystemServerTiming: SetSystemProcess took to complete: 3ms
05-15 01:33:32.381  1580  1638 I ServiceThread: Enabled StrictMode logging for android.anim looper.
05-15 01:33:32.381  1580  1580 I SystemServer: StartOverlayManagerService
05-15 01:33:32.382  1580  1580 I SystemServer: StartSubstratumService
05-15 01:33:32.382  1580  1639 D SystemServerInitThreadPool: Started executing Init OverlayManagerService
05-15 01:33:32.382  1580  1580 D SystemServerTiming: StartSubstratumService took to complete: 1ms
05-15 01:33:32.383  1580  1580 I SystemServer: StartDropBoxManager
05-15 01:33:32.383  1580  1640 D SystemServerInitThreadPool: Started executing StartSensorService
05-15 01:33:32.383  1580  1580 I SystemServiceManager: Starting com.android.server.DropBoxManagerService
05-15 01:33:32.383  1580  1640 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:32.383  1580  1580 D SystemServerTiming: StartDropBoxManager took to complete: 0ms
05-15 01:33:32.383  1580  1580 I SystemServer: StartBatteryService
05-15 01:33:32.383  1580  1580 I SystemServiceManager: Starting com.android.server.BatteryService
05-15 01:33:32.384  1461  1477 E /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: ISensors::poll() re-entry. I do not know what to do except killing myself.
05-15 01:33:32.389  1580  1580 D SystemServerTiming: StartBatteryService took to complete: 5ms
05-15 01:33:32.389  1580  1580 I SystemServer: StartUsageService
05-15 01:33:32.389  1580  1592 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:32.389  1580  1580 I SystemServiceManager: Starting com.android.server.usage.UsageStatsService
05-15 01:33:32.391  1580  1580 D SystemServerTiming: StartUsageService took to complete: 2ms
05-15 01:33:32.391  1580  1580 I SystemServer: StartWebViewUpdateService
05-15 01:33:32.391  1580  1580 I SystemServiceManager: Starting com.android.server.webkit.WebViewUpdateService
05-15 01:33:32.393  1580  1580 D SystemServerTiming: StartWebViewUpdateService took to complete: 2ms
05-15 01:33:32.394  1580  1580 I SystemServer: StartKeyAttestationApplicationIdProviderService
05-15 01:33:32.394  1580  1593 D SystemServerInitThreadPool: Started executing SecondaryZygotePreload
05-15 01:33:32.394  1580  1593 I SystemServer: SecondaryZygotePreload
05-15 01:33:32.395  1580  1580 D SystemServerTiming: StartKeyAttestationApplicationIdProviderService took to complete: 1ms
05-15 01:33:32.395  1580  1580 I SystemServer: StartKeyChainSystemService
05-15 01:33:32.395  1580  1580 I SystemServiceManager: Starting com.android.server.security.KeyChainSystemService
05-15 01:33:32.395  1580  1580 D SystemServerTiming: StartKeyChainSystemService took to complete: 0ms
05-15 01:33:32.395  1580  1580 I SystemServer: StartSchedulingPolicyService
05-15 01:33:32.396  1580  1580 D SystemServerTiming: StartSchedulingPolicyService took to complete: 1ms
05-15 01:33:32.396  1580  1580 I SystemServer: StartTelecomLoaderService
05-15 01:33:32.397  1580  1580 I SystemServiceManager: Starting com.android.server.telecom.TelecomLoaderService
05-15 01:33:32.397  1580  1580 D SystemServerTiming: StartTelecomLoaderService took to complete: 1ms
05-15 01:33:32.397  1580  1580 I SystemServer: StartTelephonyRegistry
05-15 01:33:32.400  1580  1580 D SystemServerTiming: StartTelephonyRegistry took to complete: 3ms
05-15 01:33:32.400  1580  1580 I SystemServer: StartEntropyMixer
05-15 01:33:32.402  1580  1580 I EntropyMixer: Writing entropy...
05-15 01:33:32.404  1580  1593 I chatty  : uid=1000 system_server expire 2 lines
05-15 01:33:32.407  1642  1642 I chatty  : uid=1000(system) sensors@1.0-ser expire 45 lines
05-15 01:33:32.408  1580  1580 D SystemServerTiming: StartEntropyMixer took to complete: 8ms
05-15 01:33:32.408  1580  1580 I SystemServer: StartAccountManagerService
05-15 01:33:32.408  1580  1580 I SystemServiceManager: Starting com.android.server.accounts.AccountManagerService$Lifecycle
05-15 01:33:32.411  1580  1580 D SystemServerTiming: StartAccountManagerService took to complete: 3ms
05-15 01:33:32.411  1580  1580 I SystemServer: StartContentService
05-15 01:33:32.411  1580  1580 I SystemServiceManager: Starting com.android.server.content.ContentService$Lifecycle
05-15 01:33:32.412  1580  1580 D SystemServerTiming: StartContentService took to complete: 1ms
05-15 01:33:32.412  1580  1580 I SystemServer: InstallSystemProviders
05-15 01:33:32.425  1580  1593 E SystemServer: Unable to preload default resources
05-15 01:33:32.425  1580  1593 D SystemServerTimingAsync: SecondaryZygotePreload took to complete: 31ms
05-15 01:33:32.425  1580  1593 D SystemServerInitThreadPool: Finished executing SecondaryZygotePreload
05-15 01:33:32.458  1580  1580 I SettingsState: No settings state /data/system/users/0/settings_ssaid.xml
05-15 01:33:32.463  1580  1580 D SystemServerTiming: InstallSystemProviders took to complete: 51ms
05-15 01:33:32.463  1580  1580 I SystemServer: StartVibratorService
05-15 01:33:32.466  1580  1580 D SystemServerTiming: StartVibratorService took to complete: 3ms
05-15 01:33:32.466  1580  1580 I SystemServer: StartConsumerIrService
05-15 01:33:32.467  1580  1580 E System  : ******************************************
05-15 01:33:32.467  1580  1580 E System  : ************ Failure starting core service
05-15 01:33:32.467  1580  1580 E System  : java.lang.RuntimeException: IR HAL present, but FEATURE_CONSUMER_IR is not set!
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.server.ConsumerIrService.<init>(ConsumerIrService.java:54)
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:831)
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:32.467  1580  1580 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:32.467  1580  1580 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:32.467  1580  1580 I SystemServer: StartInputMethodManagerLifecycle
05-15 01:33:32.467  1580  1580 I SystemServiceManager: Starting com.android.server.InputMethodManagerService$Lifecycle
05-15 01:33:32.469   733   733 W Binder:733_1: type=1400 audit(0.0:158): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:32.469   733   733 W Binder:733_1: type=1400 audit(0.0:161): avc: denied { quotaget } for scontext=u:r:installd:s0 tcontext=u:object_r:radio_data_file:s0 tclass=filesystem permissive=0
05-15 01:33:32.471  1580  1580 D SystemServerTiming: StartInputMethodManagerLifecycle took to complete: 4ms
05-15 01:33:32.471  1580  1580 I SystemServer: StartAccessibilityManagerService
05-15 01:33:32.473  1580  1580 D SystemServerTiming: StartAccessibilityManagerService took to complete: 1ms
05-15 01:33:32.473  1580  1580 I SystemServer: MakeDisplayReady
05-15 01:33:32.473  1580  1580 W SystemServer: ***********************************************
05-15 01:33:32.473  1580  1580 E SystemServer: BOOT FAILURE making display ready
05-15 01:33:32.473  1580  1580 E SystemServer: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.wm.WindowManagerService.displayReady()' on a null object reference
05-15 01:33:32.473  1580  1580 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:947)
05-15 01:33:32.473  1580  1580 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:32.473  1580  1580 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:32.473  1580  1580 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:32.473  1580  1580 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:32.473  1580  1580 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:32.473  1580  1580 D SystemServerTiming: MakeDisplayReady took to complete: 0ms
05-15 01:33:32.473  1580  1580 I SystemServer: StartStorageManagerService
05-15 01:33:32.474  1580  1580 I SystemServiceManager: Starting com.android.server.StorageManagerService$Lifecycle
05-15 01:33:32.477  1580  1580 D SystemServerTiming: StartStorageManagerService took to complete: 4ms
05-15 01:33:32.477  1580  1580 I SystemServer: StartStorageStatsService
05-15 01:33:32.477  1580  1580 I SystemServiceManager: Starting com.android.server.usage.StorageStatsService$Lifecycle
05-15 01:33:32.478  1580  1651 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:32.478  1580  1651 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:32.478  1580  1651 D StorageManagerService: Thinking about init, mSystemReady=false, mDaemonConnected=true
05-15 01:33:32.478  1580  1651 D StorageManagerService: Thinking about reset, mSystemReady=false, mDaemonConnected=true
05-15 01:33:32.479  1580  1651 D CryptdConnector: SND -> {1 cryptfs getfield SystemLocale}
05-15 01:33:32.479  1580  1639 D SystemServerInitThreadPool: Finished executing Init OverlayManagerService
05-15 01:33:32.481  1580  1580 D SystemServerTiming: StartStorageStatsService took to complete: 4ms
05-15 01:33:32.481  1580  1580 I SystemServer: StartUiModeManager
05-15 01:33:32.481  1580  1580 I SystemServiceManager: Starting com.android.server.UiModeManagerService
05-15 01:33:32.482  1580  1653 D CryptdConnector: RCV <- {200 1 -1}
05-15 01:33:32.484  1580  1651 W StorageManagerService: No primary storage mounted!
05-15 01:33:32.484  1580  1651 D VoldConnector: SND -> {1 asec list}
05-15 01:33:32.485  1580  1652 D VoldConnector: RCV <- {200 1 asec operation succeeded}
05-15 01:33:32.485  1580  1651 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:32.485  1580  1593 D SystemServerInitThreadPool: Started executing UiModeManager.onStart
05-15 01:33:32.486  1580  1593 I ActivityManager: Config changes=200 {1.0 ?mcc?mnc [en_US] ldltr ?swdp ?wdp ?hdp ?density ?lsize ?long ?ldr ?wideColorGamut ?orien ?touch ?keyb/?/? ?nav/? s.2}
05-15 01:33:32.486  1580  1580 D SystemServerTiming: StartUiModeManager took to complete: 5ms
05-15 01:33:32.486  1580  1580 I SystemServer: UpdatePackagesIfNeeded
05-15 01:33:32.487  1642  1658 I chatty  : uid=1000(system) HwBinder:1642_1 expire 15 lines
05-15 01:33:32.487  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-7 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 7, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-8 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 8, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-11 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 11, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-12 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 12, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-13 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 13, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-14 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 14, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-15 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 15, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-17 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 17, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-18 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 18, enabled:0, err: 0
05-15 01:33:32.488  1642  1658 I /vendor/bin/hw/vendor.huawei.hardware.sensors@1.0-service: activate-21 frameOpenedAls-0 enabled-0 cameraOpenedAls-0
05-15 01:33:32.488  1642  1658 D SensorHub: Channel activate-> handle: 21, enabled:0, err: 0
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: Failure in UiModeManager.onStart: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: java.lang.IllegalArgumentException: No display found with id: 0
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityStackSupervisor.getDisplayOverrideConfiguration(ActivityStackSupervisor.java:488)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.performDisplayOverrideConfigUpdate(ActivityManagerService.java:20762)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateGlobalConfiguration(ActivityManagerService.java:20669)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfigurationLocked(ActivityManagerService.java:20547)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.am.ActivityManagerService.updateConfiguration(ActivityManagerService.java:20486)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.sendConfigurationLocked(UiModeManagerService.java:478)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.UiModeManagerService.lambda$-com_android_server_UiModeManagerService_9177(UiModeManagerService.java:236)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.$m$4(Unknown Source:4)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$VaVGUZuNs2jqHMhhxPzwNl4zK-M.run(Unknown Source:27)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.SystemServerInitThreadPool.lambda$-com_android_server_SystemServerInitThreadPool_2249(SystemServerInitThreadPool.java:64)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.$m$2(Unknown Source:8)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.server.-$Lambda$Ganck_s9Kl5o2K6eVDoQTKLc-6g.run(Unknown Source:19)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:457)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1162)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:636)
05-15 01:33:32.489  1580  1593 E SystemServerInitThreadPool: 	at com.android.internal.util.ConcurrentUtils$1$1.run(ConcurrentUtils.java:59)
05-15 01:33:32.489  1580  1660 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:32.489  1580  1640 D SystemServerTimingAsync: StartSensorService took to complete: 106ms
05-15 01:33:32.489  1580  1640 D SystemServerInitThreadPool: Finished executing StartSensorService
05-15 01:33:32.489  1580  1661 I chatty  : uid=1000 system_server expire 1 line
05-15 01:33:32.508  1580  1651 W StorageManagerService: No primary storage mounted!
05-15 01:33:32.508  1580  1651 D VoldConnector: SND -> {2 asec list}
05-15 01:33:32.508  1580  1594 I UsageStatsService: User[0] Rollover scheduled @ 2018-05-16 01:33:32(1526434412486)
05-15 01:33:32.509  1580  1652 D VoldConnector: RCV <- {200 2 asec operation succeeded}
05-15 01:33:32.509  1580  1594 E AppIdleHistory: Unable to read app idle file for user 0
05-15 01:33:32.532  1662  1662 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/TelephonyProvider --class-loader-context=PCL[]
05-15 01:33:32.601  1662  1662 I dex2oat : dex2oat took 69.811ms (74.884ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=117KB (120728B) native alloc=2MB (2136352B) free=985KB (1009376B)
05-15 01:33:32.624  1668  1668 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/MmsService --class-loader-context=PCL[]
05-15 01:33:32.678  1668  1668 I dex2oat : dex2oat took 54.256ms (50.450ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=101KB (103616B) native alloc=1955KB (2002744B) free=1116KB (1142984B)
05-15 01:33:32.700  1673  1673 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/DefaultContainerService --class-loader-context=PCL[]
05-15 01:33:32.742  1673  1673 I dex2oat : dex2oat took 41.980ms (37.469ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=35KB (36512B) native alloc=1500KB (1536496B) free=1059KB (1084944B)
05-15 01:33:32.764  1680  1680 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/SettingsProvider --class-loader-context=PCL[]
05-15 01:33:32.847  1680  1680 I dex2oat : dex2oat took 83.104ms (129.477ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=295KB (302512B) native alloc=2MB (2494320B) free=1148KB (1175696B)
05-15 01:33:32.870  1685  1685 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Trebuchet --class-loader-context=PCL[]
05-15 01:33:33.000   511  1501 E audio_hw_primary: direct_standby_loop: adev->outputs[OUTPUT_DIRECT] is NULL
05-15 01:33:33.000   511  1501 I audio_hw_primary: direct_standby_loop: standby loop exit...
05-15 01:33:33.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 4,  out_device: 0x2
05-15 01:33:33.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 5,  out_device: 0x2
05-15 01:33:33.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 6,  out_device: 0x2
05-15 01:33:33.000   511  1034 I audio_hw_primary: do_out_standby standby: 1, stream_type: 7,  out_device: 0x2
05-15 01:33:33.000   511  1034 E typec_headset_hal: typec_headset_uninit:already null so no need to free
05-15 01:33:33.000   511  1034 D dsp_interface: dsp_close:
05-15 01:33:33.000   511  1034 I dsp_soc_ctl: dsp_soc_ctl_close++
05-15 01:33:33.000   511  1034 I dsp_soc_ctl: close /dev/hifi_misc.
05-15 01:33:33.000   511  1034 I dsp_soc_ctl: dsp_soc_ctl_close--
05-15 01:33:33.001   511  1034 I MAX98925_SPK: maxim smartpa close
05-15 01:33:33.001   511  1034 I r_submix: adev_close()
05-15 01:33:33.240  1685  1685 I dex2oat : dex2oat took 370.502ms (840.733ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=4MB (4835800B) native alloc=3MB (3611768B) free=1592KB (1631112B)
05-15 01:33:33.245  1580  1636 I chatty  : uid=1000 system_server expire 7 lines
05-15 01:33:33.263  1690  1690 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/InputDevices --class-loader-context=PCL[]
05-15 01:33:33.300  1690  1690 I dex2oat : dex2oat took 36.802ms (32.440ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=16KB (16984B) native alloc=1153KB (1181600B) free=1406KB (1439840B)
05-15 01:33:33.321  1695  1695 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/ExtShared --class-loader-context=PCL[]
05-15 01:33:33.358  1695  1695 I dex2oat : dex2oat took 37.621ms (33.963ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=64KB (65552B) native alloc=1634KB (1673360B) free=925KB (948080B)
05-15 01:33:33.381  1700  1700 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Telecom --class-loader-context=PCL[]
05-15 01:33:33.589  1700  1700 I dex2oat : dex2oat took 208.991ms (428.328ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=1846KB (1890488B) native alloc=2MB (2775144B) free=1385KB (1419160B)
05-15 01:33:33.614  1705  1705 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Dialer --class-loader-context=PCL[]
05-15 01:33:33.616  1705  1705 W dex2oat : Could not reserve sentinel fault page
05-15 01:33:33.971  1705  1710 W dex2oat : Class android.support.v4.content.ModernAsyncTask failed lock verification and will run slower.
05-15 01:33:33.972  1705  1710 W dex2oat : Common causes for lock verification issues are non-optimized dex code
05-15 01:33:33.972  1705  1710 W dex2oat : and incorrect proguard optimizations.
05-15 01:33:33.983  1705  1712 W dex2oat : Class android.support.v4.util.SimpleArrayMap failed lock verification and will run slower.
05-15 01:33:33.984  1705  1711 W dex2oat : Class android.support.v4.util.ArraySet failed lock verification and will run slower.
05-15 01:33:34.041  1714  1714 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:34.043   385   385 I chatty  : uid=1000(system) hwservicemanage expire 10 lines
05-15 01:33:34.044  1713  1713 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:34.045  1713  1713 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:34.045  1713  1713 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:34.045  1713  1713 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:34.046  1714  1714 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:34.048  1714  1714 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:34.072  1705  1711 W dex2oat : Class com.android.dialer.DialerPhoneNumber$RawInput failed lock verification and will run slower.
05-15 01:33:34.072  1705  1712 W dex2oat : Class com.android.dialer.DialerPhoneNumber failed lock verification and will run slower.
05-15 01:33:34.072  1705  1705 W dex2oat : Class com.android.dialer.DialerInternalPhoneNumber failed lock verification and will run slower.
05-15 01:33:34.113  1705  1710 W dex2oat : Class com.android.dialer.calldetails.CallDetailsEntries failed lock verification and will run slower.
05-15 01:33:34.113  1705  1711 W dex2oat : Class com.android.dialer.calldetails.CallDetailsEntries$CallDetailsEntry failed lock verification and will run slower.
05-15 01:33:34.115  1705  1705 W dex2oat : Class com.android.dialer.callintent.CallSpecificAppData failed lock verification and will run slower.
05-15 01:33:34.116  1705  1712 W dex2oat : Class com.android.dialer.common.concurrent.AsyncTaskExecutors failed lock verification and will run slower.
05-15 01:33:34.120  1705  1711 W dex2oat : Class com.android.dialer.dialercontact.SimDetails failed lock verification and will run slower.
05-15 01:33:34.120  1705  1712 W dex2oat : Class com.android.dialer.dialercontact.DialerContact failed lock verification and will run slower.
05-15 01:33:34.123  1705  1712 W dex2oat : Class com.android.dialer.enrichedcall.historyquery.proto.HistoryResult failed lock verification and will run slower.
05-15 01:33:34.191  1705  1712 W dex2oat : Class com.bumptech.glide.Glide failed lock verification and will run slower.
05-15 01:33:34.226  1705  1705 W dex2oat : Class com.google.internal.communications.voicemailtranscription.v1.TranscribeVoicemailRequest failed lock verification and will run slower.
05-15 01:33:34.226  1705  1710 W dex2oat : Class com.google.internal.communications.voicemailtranscription.v1.TranscribeVoicemailResponse failed lock verification and will run slower.
05-15 01:33:34.266  1705  1705 I dex2oat : dex2oat took 652.289ms (1.369s cpu) (threads: 4) arena alloc=0B (0B) java alloc=6MB (6600936B) native alloc=4MB (5173776B) free=1603KB (1641968B)
05-15 01:33:34.290  1717  1717 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ExtServices --class-loader-context=PCL[]
05-15 01:33:34.329  1717  1717 I dex2oat : dex2oat took 39.221ms (37.334ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=77KB (79072B) native alloc=1936KB (1983264B) free=1647KB (1686752B)
05-15 01:33:34.352  1722  1722 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/PackageInstaller --class-loader-context=PCL[]
05-15 01:33:34.621  1722  1722 I dex2oat : dex2oat took 269.372ms (590.458ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=3MB (3856288B) native alloc=2MB (2877040B) free=1798KB (1841552B)
05-15 01:33:34.644  1727  1727 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ProxyHandler --class-loader-context=PCL[]
05-15 01:33:34.687  1727  1727 I dex2oat : dex2oat took 43.016ms (35.568ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=67KB (69288B) native alloc=1925KB (1971472B) free=1146KB (1174256B)
05-15 01:33:34.708  1732  1732 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/LatinIME --class-loader-context=PCL[]
05-15 01:33:34.844  1732  1732 I dex2oat : dex2oat took 137.017ms (257.646ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=1305KB (1336856B) native alloc=2MB (2533440B) free=1621KB (1660864B)
05-15 01:33:34.858  1580  1592 W BatteryService: updateLightsLocked: mLineageBatteryLights is not yet ready; skipping
05-15 01:33:34.870  1739  1739 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Settings --class-loader-context=PCL[]
05-15 01:33:35.609  1739  1739 I dex2oat : dex2oat took 739.535ms (1.712s cpu) (threads: 4) arena alloc=0B (0B) java alloc=12MB (13218240B) native alloc=5MB (6221600B) free=2MB (2167008B)
05-15 01:33:35.632  1744  1744 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/LineageSettingsProvider --class-loader-context=PCL[]
05-15 01:33:35.634  1744  1744 W dex2oat : Could not reserve sentinel fault page
05-15 01:33:35.706  1744  1744 I dex2oat : dex2oat took 73.656ms (101.744ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=261KB (267536B) native alloc=2MB (2118944B) free=1002KB (1026784B)
05-15 01:33:35.727  1749  1749 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/TeleService --class-loader-context=PCL[]
05-15 01:33:35.968  1749  1749 I dex2oat : dex2oat took 241.500ms (500.670ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2949624B) native alloc=3MB (3218088B) free=1465KB (1500504B)
05-15 01:33:35.991  1756  1756 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Shell --class-loader-context=PCL[]
05-15 01:33:36.049  1756  1756 I dex2oat : dex2oat took 58.665ms (71.323ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=173KB (178008B) native alloc=2MB (2100712B) free=1532KB (1569304B)
05-15 01:33:36.070  1761  1761 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/FusedLocation --class-loader-context=PCL[/system/framework/com.android.location.provider.jar]
05-15 01:33:36.110  1761  1761 I dex2oat : dex2oat took 40.307ms (36.958ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=68KB (69704B) native alloc=2MB (2161776B) free=960KB (983952B)
05-15 01:33:36.132  1766  1766 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/SystemUI --class-loader-context=PCL[]
05-15 01:33:36.141  1767  1767 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:36.141  1767  1767 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:36.141  1767  1767 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:36.141  1767  1767 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:36.142  1767  1767 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:36.144  1767  1767 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:36.144  1767  1767 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:36.144  1767  1767 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:36.911  1766  1766 I dex2oat : dex2oat took 779.701ms (1.805s cpu) (threads: 4) arena alloc=0B (0B) java alloc=11MB (11743432B) native alloc=5MB (6160504B) free=2MB (2228104B)
05-15 01:33:36.936  1774  1774 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/OmniJaws --class-loader-context=PCL[]
05-15 01:33:36.995  1774  1774 I dex2oat : dex2oat took 59.572ms (55.598ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=171KB (175240B) native alloc=1994KB (2042056B) free=1589KB (1627960B)
05-15 01:33:37.017  1779  1779 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/HardwareOverlayPicker --class-loader-context=PCL[]
05-15 01:33:37.059  1779  1779 I dex2oat : dex2oat took 41.888ms (33.289ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=64KB (66240B) native alloc=1482KB (1518184B) free=1077KB (1103256B)
05-15 01:33:37.081  1784  1784 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/CalendarProvider --class-loader-context=PCL[/system/framework/android.test.mock.jar:/system/framework/android.test.runner.jar]
05-15 01:33:37.172  1784  1784 I dex2oat : dex2oat took 91.559ms (137.528ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=484KB (496456B) native alloc=2MB (2570472B) free=1585KB (1623832B)
05-15 01:33:37.195  1789  1789 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/MediaProvider --class-loader-context=PCL[]
05-15 01:33:37.258  1789  1789 I dex2oat : dex2oat took 63.588ms (68.865ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=162KB (166792B) native alloc=2MB (2103904B) free=1529KB (1566112B)
05-15 01:33:37.281  1794  1794 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/WallpaperCropper --class-loader-context=PCL[]
05-15 01:33:37.328  1794  1794 I dex2oat : dex2oat took 47.873ms (57.659ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=147KB (150632B) native alloc=2019KB (2067976B) free=1052KB (1077752B)
05-15 01:33:37.352  1799  1799 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/DocumentsUI --class-loader-context=PCL[]
05-15 01:33:37.625  1799  1799 I dex2oat : dex2oat took 273.366ms (569.739ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=3MB (3324544B) native alloc=3MB (3352888B) free=1845KB (1889992B)
05-15 01:33:37.649  1804  1804 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ExternalStorageProvider --class-loader-context=PCL[]
05-15 01:33:37.689  1804  1804 I dex2oat : dex2oat took 40.744ms (39.346ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=72KB (73752B) native alloc=1990KB (2038200B) free=1081KB (1107528B)
05-15 01:33:37.711  1809  1809 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/HTMLViewer --class-loader-context=PCL[]
05-15 01:33:37.712  1809  1809 W dex2oat : Could not reserve sentinel fault page
05-15 01:33:37.749  1809  1809 I dex2oat : dex2oat took 38.620ms (36.868ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=65KB (66760B) native alloc=1657KB (1697176B) free=1414KB (1448552B)
05-15 01:33:37.771  1814  1814 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/SubstratumService --class-loader-context=PCL[]
05-15 01:33:37.807  1814  1814 I dex2oat : dex2oat took 36.502ms (32.729ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=35KB (36336B) native alloc=1474KB (1509768B) free=1085KB (1111672B)
05-15 01:33:37.827  1819  1819 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/CompanionDeviceManager --class-loader-context=PCL[]
05-15 01:33:37.870  1819  1819 I dex2oat : dex2oat took 43.376ms (40.625ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=85KB (87856B) native alloc=1820KB (1864328B) free=1763KB (1805688B)
05-15 01:33:37.893  1826  1826 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/DownloadProvider --class-loader-context=PCL[]
05-15 01:33:37.971  1826  1826 I dex2oat : dex2oat took 78.530ms (113.537ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=406KB (416496B) native alloc=2MB (2497864B) free=1656KB (1696440B)
05-15 01:33:37.996  1831  1831 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/messaging --class-loader-context=PCL[]
05-15 01:33:38.501  1831  1831 I dex2oat : dex2oat took 504.992ms (1.075s cpu) (threads: 4) arena alloc=0B (0B) java alloc=5MB (6057560B) native alloc=4MB (4862480B) free=1395KB (1428976B)
05-15 01:33:38.524  1836  1836 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Terminal --class-loader-context=PCL[]
05-15 01:33:38.700  1836  1836 I dex2oat : dex2oat took 176.616ms (325.537ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=1247KB (1277944B) native alloc=2MB (2605160B) free=1551KB (1589144B)
05-15 01:33:38.727  1841  1841 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/LockClock --class-loader-context=PCL[]
05-15 01:33:38.820  1841  1841 I dex2oat : dex2oat took 92.904ms (136.354ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=480KB (492024B) native alloc=2MB (2276056B) free=1361KB (1393960B)
05-15 01:33:38.826  1580  1580 I chatty  : uid=1000 system_server expire 39 lines
05-15 01:33:38.843  1846  1846 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/DownloadProviderUi --class-loader-context=PCL[]
05-15 01:33:38.844  1846  1846 W dex2oat : Could not reserve sentinel fault page
05-15 01:33:38.881  1846  1846 I dex2oat : dex2oat took 39.086ms (36.669ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=80KB (82904B) native alloc=1795KB (1838960B) free=1788KB (1831056B)
05-15 01:33:38.903  1851  1851 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/PacProcessor --class-loader-context=PCL[]
05-15 01:33:38.941  1851  1851 I dex2oat : dex2oat took 38.584ms (34.074ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=51KB (52736B) native alloc=1643KB (1682544B) free=1428KB (1463184B)
05-15 01:33:38.963  1858  1858 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/OmniStyle --class-loader-context=PCL[]
05-15 01:33:39.021  1858  1858 I dex2oat : dex2oat took 58.293ms (65.717ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=230KB (236224B) native alloc=2MB (2157592B) free=964KB (988136B)
05-15 01:33:39.033  1864  1864 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:39.033  1863  1863 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:39.034  1863  1863 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:39.034  1863  1863 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:39.034  1863  1863 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:39.035  1864  1864 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:39.036  1864  1864 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:39.047  1865  1865 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Profiles --class-loader-context=PCL[]
05-15 01:33:39.125  1865  1865 I dex2oat : dex2oat took 79.118ms (108.636ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=297KB (304136B) native alloc=2MB (2122888B) free=998KB (1022840B)
05-15 01:33:39.148  1871  1871 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/CertInstaller --class-loader-context=PCL[]
05-15 01:33:39.194  1871  1871 I dex2oat : dex2oat took 46.555ms (47.751ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=167KB (171856B) native alloc=2MB (2134512B) free=1499KB (1535504B)
05-15 01:33:39.218  1876  1876 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/CarrierConfig --class-loader-context=PCL[]
05-15 01:33:39.260  1876  1876 I dex2oat : dex2oat took 42.505ms (34.134ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=22KB (23152B) native alloc=1315KB (1346944B) free=1244KB (1274496B)
05-15 01:33:39.284  1881  1881 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Contacts --class-loader-context=PCL[]
05-15 01:33:39.758  1881  1881 I dex2oat : dex2oat took 474.369ms (1.042s cpu) (threads: 4) arena alloc=0B (0B) java alloc=5MB (5849624B) native alloc=4MB (4474104B) free=1262KB (1293064B)
05-15 01:33:39.763  1580  1636 I chatty  : uid=1000 system_server expire 3 lines
05-15 01:33:39.782  1886  1886 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Camera2 --class-loader-context=PCL[]
05-15 01:33:40.042  1886  1886 I dex2oat : dex2oat took 259.885ms (505.941ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2333432B) native alloc=3MB (3278008B) free=1406KB (1440584B)
05-15 01:33:40.066  1893  1893 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Recorder --class-loader-context=PCL[]
05-15 01:33:40.288  1893  1893 I dex2oat : dex2oat took 222.735ms (445.056ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2592696B) native alloc=2MB (2590168B) free=2MB (2128424B)
05-15 01:33:40.310  1898  1898 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/EasterEgg --class-loader-context=PCL[]
05-15 01:33:40.393  1898  1898 I dex2oat : dex2oat took 83.457ms (123.469ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=355KB (363560B) native alloc=2MB (2323360B) free=1315KB (1346656B)
05-15 01:33:40.415  1903  1903 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/MtpDocumentsProvider --class-loader-context=PCL[]
05-15 01:33:40.467  1903  1903 I dex2oat : dex2oat took 51.685ms (50.977ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=88KB (91104B) native alloc=1953KB (2000136B) free=1118KB (1145592B)
05-15 01:33:40.489  1908  1908 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Stk --class-loader-context=PCL[]
05-15 01:33:40.535  1908  1908 I dex2oat : dex2oat took 46.910ms (55.864ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=172KB (176264B) native alloc=1931KB (1977480B) free=1652KB (1692536B)
05-15 01:33:40.557  1913  1913 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/BackupRestoreConfirmation --class-loader-context=PCL[]
05-15 01:33:40.602  1913  1913 I dex2oat : dex2oat took 44.928ms (37.633ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=64KB (66392B) native alloc=1800KB (1843704B) free=1271KB (1302024B)
05-15 01:33:40.624  1918  1918 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/WeatherProvider --class-loader-context=PCL[]
05-15 01:33:40.699  1918  1918 I dex2oat : dex2oat took 75.464ms (96.617ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=259KB (265896B) native alloc=2MB (2118056B) free=1515KB (1551960B)
05-15 01:33:40.722  1923  1923 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/GoogleClock --class-loader-context=PCL[]
05-15 01:33:41.047  1923  1923 I dex2oat : dex2oat took 325.641ms (779.805ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=4MB (4405856B) native alloc=3MB (3537568B) free=1153KB (1181024B)
05-15 01:33:41.069  1930  1930 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Provision --class-loader-context=PCL[]
05-15 01:33:41.105  1930  1930 I dex2oat : dex2oat took 37.136ms (33.209ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=16KB (17032B) native alloc=1214KB (1243712B) free=1345KB (1377728B)
05-15 01:33:41.127  1935  1935 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/StatementService --class-loader-context=PCL[]
05-15 01:33:41.142  1936  1936 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:41.142  1936  1936 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:41.142  1936  1936 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:41.142  1936  1936 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:41.142  1936  1936 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:41.144  1936  1936 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:41.145  1936  1936 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:41.145  1936  1936 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:41.174  1935  1935 I dex2oat : dex2oat took 47.438ms (46.536ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=68KB (69720B) native alloc=1995KB (2043432B) free=1588KB (1626584B)
05-15 01:33:41.196  1941  1941 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/SharedStorageBackup --class-loader-context=PCL[]
05-15 01:33:41.238  1941  1941 I dex2oat : dex2oat took 41.990ms (34.871ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=54KB (55856B) native alloc=1640KB (1680104B) free=919KB (941336B)
05-15 01:33:41.260  1946  1946 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/PrintSpooler --class-loader-context=PCL[]
05-15 01:33:41.364  1946  1946 I dex2oat : dex2oat took 104.129ms (175.992ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=655KB (671056B) native alloc=2MB (2518392B) free=1636KB (1675912B)
05-15 01:33:41.368  1580  1636 D SystemServerTimingAsync: AppDataPrepare took to complete: 9038ms
05-15 01:33:41.368  1580  1636 I PackageManager: Deferred reconcileAppsData finished 73 packages
05-15 01:33:41.368  1580  1636 D SystemServerInitThreadPool: Finished executing prepareAppData
05-15 01:33:41.386  1951  1951 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/BasicDreams --class-loader-context=PCL[]
05-15 01:33:41.429  1951  1951 I dex2oat : dex2oat took 43.312ms (37.084ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=70KB (71960B) native alloc=1853KB (1897640B) free=1730KB (1772376B)
05-15 01:33:41.455  1956  1956 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/webview --class-loader-context=PCL[]
05-15 01:33:41.692  1956  1956 I dex2oat : dex2oat took 237.469ms (496.976ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2806704B) native alloc=3MB (3180816B) free=1501KB (1537776B)
05-15 01:33:41.714  1961  1961 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/BuiltInPrintService --class-loader-context=PCL[]
05-15 01:33:41.715  1961  1961 W dex2oat : Could not reserve sentinel fault page
05-15 01:33:41.766  1961  1961 I dex2oat : dex2oat took 52.268ms (56.581ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=142KB (145696B) native alloc=2MB (2101288B) free=1531KB (1568728B)
05-15 01:33:41.787  1966  1966 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/CellBroadcastReceiver --class-loader-context=PCL[]
05-15 01:33:42.003  1966  1966 I dex2oat : dex2oat took 216.291ms (443.843ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2582944B) native alloc=2MB (2624832B) free=1532KB (1569472B)
05-15 01:33:42.025  1973  1973 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/OneTimeInitializer --class-loader-context=PCL[]
05-15 01:33:42.070  1973  1973 I dex2oat : dex2oat took 45.006ms (41.961ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=82KB (84952B) native alloc=1953KB (2000008B) free=1630KB (1670008B)
05-15 01:33:42.090  1978  1978 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/KeyChain --class-loader-context=PCL[]
05-15 01:33:42.130  1978  1978 I dex2oat : dex2oat took 40.165ms (43.594ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=104KB (107464B) native alloc=1944KB (1991128B) free=1639KB (1678888B)
05-15 01:33:42.150  1983  1983 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/PrintRecommendationService --class-loader-context=PCL[]
05-15 01:33:42.191  1983  1983 I dex2oat : dex2oat took 41.247ms (43.651ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=73KB (75456B) native alloc=1943KB (1990240B) free=1640KB (1679776B)
05-15 01:33:42.214  1988  1988 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Gallery2 --class-loader-context=PCL[]
05-15 01:33:42.648  1988  1988 I dex2oat : dex2oat took 434.597ms (940.746ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=5MB (5596328B) native alloc=3MB (4092480B) free=1635KB (1674688B)
05-15 01:33:42.671  1993  1993 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/CallLogBackup --class-loader-context=PCL[]
05-15 01:33:42.710  1993  1993 I dex2oat : dex2oat took 39.930ms (36.806ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=67KB (69336B) native alloc=1641KB (1680952B) free=1430KB (1464776B)
05-15 01:33:42.731  1998  1998 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/CarrierDefaultApp --class-loader-context=PCL[]
05-15 01:33:42.772  1998  1998 I dex2oat : dex2oat took 41.582ms (43.290ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=85KB (87128B) native alloc=1939KB (1986008B) free=1644KB (1684008B)
05-15 01:33:42.797  2003  2003 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/Eleven --class-loader-context=PCL[]
05-15 01:33:43.349  2003  2003 I dex2oat : dex2oat took 552.486ms (1.046s cpu) (threads: 4) arena alloc=0B (0B) java alloc=4MB (4561592B) native alloc=4MB (5224480B) free=2MB (2115552B)
05-15 01:33:43.372  2010  2010 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ManagedProvisioning --class-loader-context=PCL[]
05-15 01:33:43.453  2010  2010 I dex2oat : dex2oat took 81.895ms (117.731ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=700KB (717304B) native alloc=2MB (2140904B) free=1493KB (1529112B)
05-15 01:33:43.474  2015  2015 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/PhotoTable --class-loader-context=PCL[]
05-15 01:33:43.529  2015  2015 I dex2oat : dex2oat took 54.771ms (58.565ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=188KB (193352B) native alloc=2MB (2212736B) free=911KB (932992B)
05-15 01:33:43.549  2020  2020 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/WAPPushManager --class-loader-context=PCL[]
05-15 01:33:43.591  2020  2020 I dex2oat : dex2oat took 42.349ms (42.200ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=86KB (88432B) native alloc=1961KB (2008920B) free=1110KB (1136808B)
05-15 01:33:43.613  2025  2025 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/LiveWallpapersPicker --class-loader-context=PCL[]
05-15 01:33:43.851  2025  2025 I dex2oat : dex2oat took 238.435ms (482.888ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2881968B) native alloc=2MB (2596832B) free=1560KB (1597472B)
05-15 01:33:43.873  2030  2030 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/AudioFX --class-loader-context=PCL[]
05-15 01:33:44.042  2036  2036 I vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: main:27: We're the service for display engine hal.
05-15 01:33:44.047  2035  2035 D vndksupport: Loading /vendor/lib64/hw/hisupl.hi1102.default.so from current namespace instead of sphal namespace.
05-15 01:33:44.048  2035  2035 E HAL     : load: id=hisupl.hi1102 != hmi->id=hisupl
05-15 01:33:44.049  2035  2035 E HiSuplHAL_HiSuplInterface: supl hw_get_module hisupl failed: -22
05-15 01:33:44.049  2035  2035 E venodr.huawei.hardware.hisupl@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.hisupl@1.0::ISuplclienttoserverInterface/default.
05-15 01:33:44.049  2036  2036 I ServiceManagement: Removing namespace from process name vendor.huawei.hardware.hwdisplay.displayengine@1.0-service to displayengine@1.
05-15 01:33:44.050   385   385 I chatty  : uid=1000(system) hwservicemanage expire 1 line
05-15 01:33:44.051  2036  2036 E vendor.huawei.hardware.hwdisplay.displayengine@1.0-service: Could not register service vendor.huawei.hardware.hwdisplay.displayengine@1.0::IDisplayEngineWrapper/default (-2147483648).
05-15 01:33:44.085  2030  2030 I dex2oat : dex2oat took 211.751ms (403.739ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=1584KB (1622560B) native alloc=2MB (2956512B) free=1720KB (1762080B)
05-15 01:33:44.108  2040  2040 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/StorageManager --class-loader-context=PCL[]
05-15 01:33:44.336  2040  2040 I dex2oat : dex2oat took 229.115ms (476.711ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2742904B) native alloc=2MB (2845048B) free=1829KB (1873544B)
05-15 01:33:44.358  2045  2045 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/BookmarkProvider --class-loader-context=PCL[]
05-15 01:33:44.396  2045  2045 I dex2oat : dex2oat took 37.703ms (32.617ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=17KB (17512B) native alloc=1313KB (1345216B) free=1246KB (1276224B)
05-15 01:33:44.416  2050  2050 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/ExactCalculator --class-loader-context=PCL[]
05-15 01:33:44.525  2050  2050 I dex2oat : dex2oat took 108.843ms (190.685ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=670KB (686320B) native alloc=2MB (2329736B) free=1820KB (1864568B)
05-15 01:33:44.546  2055  2055 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ResurrectionOTA --class-loader-context=PCL[]
05-15 01:33:44.602  2055  2055 I dex2oat : dex2oat took 56.102ms (63.273ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=199KB (204184B) native alloc=2MB (2160000B) free=1474KB (1510016B)
05-15 01:33:44.606  1580  1580 I chatty  : uid=1000 system_server expire 5 lines
05-15 01:33:44.623  2060  2060 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/LineageParts --class-loader-context=PCL[]
05-15 01:33:44.888  2060  2060 I dex2oat : dex2oat took 265.451ms (579.669ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (3097448B) native alloc=2MB (3131264B) free=1550KB (1587328B)
05-15 01:33:44.910  2065  2065 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/VpnDialogs --class-loader-context=PCL[]
05-15 01:33:44.949  2065  2065 I dex2oat : dex2oat took 39.401ms (36.808ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=49KB (51064B) native alloc=1480KB (1516200B) free=1591KB (1629528B)
05-15 01:33:44.971  2070  2070 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Wallpapers --class-loader-context=PCL[]
05-15 01:33:45.256  2070  2070 I dex2oat : dex2oat took 285.464ms (643.493ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=3MB (3516592B) native alloc=3MB (3213552B) free=1981KB (2029328B)
05-15 01:33:45.279  2077  2077 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Email --class-loader-context=PCL[]
05-15 01:33:45.753  2077  2077 I dex2oat : dex2oat took 474.060ms (1.095s cpu) (threads: 4) arena alloc=0B (0B) java alloc=5MB (5866000B) native alloc=4MB (5046728B) free=1727KB (1769016B)
05-15 01:33:45.775  2082  2082 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/WallpaperBackup --class-loader-context=PCL[]
05-15 01:33:45.819  2082  2082 I dex2oat : dex2oat took 43.871ms (34.689ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=19KB (19568B) native alloc=1150KB (1178560B) free=1409KB (1442880B)
05-15 01:33:45.823  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/priv-app/BlockedNumberProvider/BlockedNumberProvider.apk pkg=com.android.providers.blockednumber isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:45.839  2087  2087 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/BlockedNumberProvider --class-loader-context=PCL[]
05-15 01:33:45.915  2087  2087 I dex2oat : dex2oat took 76.130ms (102.626ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=414KB (424480B) native alloc=2MB (2516864B) free=1126KB (1153152B)
05-15 01:33:45.919  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/app/UserDictionaryProvider/UserDictionaryProvider.apk pkg=com.android.providers.userdictionary isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:45.936  2092  2092 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/UserDictionaryProvider --class-loader-context=PCL[]
05-15 01:33:45.978  2092  2092 I dex2oat : dex2oat took 42.313ms (36.776ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=49KB (50728B) native alloc=1662KB (1702544B) free=897KB (918896B)
05-15 01:33:45.982  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/priv-app/EmergencyInfo/EmergencyInfo.apk pkg=com.android.emergency isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:45.998  2097  2097 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/EmergencyInfo --class-loader-context=PCL[]
05-15 01:33:46.158   385   385 W /system/bin/hwservicemanager: getTransport: Cannot find entry vendor.huawei.hardware.gnss@1.0::IHWGnss/default in either framework or device manifest.
05-15 01:33:46.161  2102  2102 E GnssHAL_GnssInterface: [gps_jni]Open /proc/device-tree/gps_power/broadcom_config,ic_type success!
05-15 01:33:46.162  2102  2102 D GnssHAL_GnssInterface: To get Gps IC type 4774
05-15 01:33:46.162  2102  2102 D GnssHAL_GnssInterface: [gps_jni]the gps_ic_type is gps4774
05-15 01:33:46.162  2102  2102 D GnssHAL_GnssInterface: [gps_jni]system do ToAdjustGpsMiddleware done!
05-15 01:33:46.162  2102  2102 D vndksupport: Loading /vendor/lib64/hw/gps4774.default.so from current namespace instead of sphal namespace.
05-15 01:33:46.167  2102  2102 E HAL     : load: id=gps4774 != hmi->id=gps
05-15 01:33:46.167  2102  2102 E GnssHAL_GnssInterface: gnss hw_get_module gps failed: -22
05-15 01:33:46.167  2102  2102 E vendor.huawei.hardware.gnss@1.0-service: Could not get passthrough implementation for vendor.huawei.hardware.gnss@1.0::IHWGnss/default.
05-15 01:33:46.233  2097  2097 I dex2oat : dex2oat took 234.783ms (460.521ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2759624B) native alloc=2MB (2428688B) free=1724KB (1765616B)
05-15 01:33:46.238  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/app/BluetoothMidiService/BluetoothMidiService.apk pkg=com.android.bluetoothmidiservice isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:46.255  2105  2105 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/BluetoothMidiService --class-loader-context=PCL[]
05-15 01:33:46.298  2105  2105 I dex2oat : dex2oat took 43.577ms (37.873ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=67KB (69152B) native alloc=1799KB (1842448B) free=1272KB (1303280B)
05-15 01:33:46.302  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/app/Bluetooth/Bluetooth.apk pkg=com.android.bluetooth isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[/system/framework/javax.obex.jar]
05-15 01:33:46.319  2110  2110 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Bluetooth --class-loader-context=PCL[/system/framework/javax.obex.jar]
05-15 01:33:46.649  2110  2110 I dex2oat : dex2oat took 331.079ms (675.331ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=2MB (2118080B) native alloc=3MB (3898008B) free=1825KB (1869160B)
05-15 01:33:46.656  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/app/Development/Development.apk pkg=com.android.development isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[/system/framework/android.test.mock.jar:/system/framework/android.test.runner.jar]
05-15 01:33:46.672  2115  2115 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/Development --class-loader-context=PCL[/system/framework/android.test.mock.jar:/system/framework/android.test.runner.jar]
05-15 01:33:46.735  2115  2115 I dex2oat : dex2oat took 63.547ms (77.622ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=461KB (472888B) native alloc=2MB (2194240B) free=1953KB (2000064B)
05-15 01:33:46.740  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/priv-app/ContactsProvider/ContactsProvider.apk pkg=com.android.providers.contacts isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:46.756  2120  2120 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/ContactsProvider --class-loader-context=PCL[]
05-15 01:33:46.884  2120  2120 I dex2oat : dex2oat took 128.283ms (212.402ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=610KB (624744B) native alloc=2MB (2562456B) free=1593KB (1631848B)
05-15 01:33:46.889  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/app/CaptivePortalLogin/CaptivePortalLogin.apk pkg=com.android.captiveportallogin isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:46.905  2125  2125 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/app/CaptivePortalLogin --class-loader-context=PCL[]
05-15 01:33:46.950  2125  2125 I dex2oat : dex2oat took 45.332ms (41.768ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=97KB (99560B) native alloc=1796KB (1839880B) free=1275KB (1305848B)
05-15 01:33:46.954  1580  1580 I PackageManager.DexOptimizer: Running dexopt (dexoptNeeded=1) on: /system/priv-app/QtiAudio/QtiAudio.apk pkg=me.phh.qti.audio isa=arm64 dexoptFlags=public target-filter=verify oatDir=null sharedLibraries=PCL[]
05-15 01:33:46.971  2130  2130 I dex2oat : /system/bin/dex2oat --input-vdex-fd=-1 --output-vdex-fd=17 --compiler-filter=verify -j4 --classpath-dir=/system/priv-app/QtiAudio --class-loader-context=PCL[]
05-15 01:33:47.008  2130  2130 I dex2oat : dex2oat took 37.947ms (37.023ms cpu) (threads: 4) arena alloc=0B (0B) java alloc=70KB (71704B) native alloc=1936KB (1983072B) free=1135KB (1162656B)
05-15 01:33:47.011  1580  1580 D SystemServerTiming: UpdatePackagesIfNeeded took to complete: 14525ms
05-15 01:33:47.011  1580  1580 I SystemServer: PerformFstrimIfNeeded
05-15 01:33:47.012  1580  1580 D SystemServerTiming: PerformFstrimIfNeeded took to complete: 1ms
05-15 01:33:47.012  1580  1580 I SystemServer: StartLockSettingsService
05-15 01:33:47.012  1580  1580 I SystemServiceManager: Starting com.android.server.locksettings.LockSettingsService$Lifecycle
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at android.content.Context.getSystemService(Context.java:3163)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.locksettings.LockSettingsStrongAuth.<init>(LockSettingsStrongAuth.java:74)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.locksettings.LockSettingsService$Injector.getStrongAuth(LockSettingsService.java:341)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.locksettings.LockSettingsService.<init>(LockSettingsService.java:399)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.locksettings.LockSettingsService.<init>(LockSettingsService.java:390)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.locksettings.LockSettingsService$Lifecycle.onStart(LockSettingsService.java:197)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:124)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:111)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1008)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.014  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.017  1580  1580 D SystemServerTiming: StartLockSettingsService took to complete: 5ms
05-15 01:33:47.017  1580  1580 I zygote64: Looking for service android.hardware.oemlock@1.0::IOemLock/default
05-15 01:33:47.018   385   385 W /system/bin/hwservicemanager: getTransport: Cannot find entry android.hardware.oemlock@1.0::IOemLock/default in either framework or device manifest.
05-15 01:33:47.018  1580  1580 E zygote64: service android.hardware.oemlock@1.0::IOemLock declares transport method EMPTY but framework expects hwbinder.
05-15 01:33:47.018  1580  1580 I OemLock : OemLock HAL not present on device
05-15 01:33:47.018  1580  1580 I SystemServer: StartDeviceIdleController
05-15 01:33:47.019  1580  1580 I SystemServiceManager: Starting com.android.server.DeviceIdleController
05-15 01:33:47.020  1580  1580 D SystemServerTiming: StartDeviceIdleController took to complete: 2ms
05-15 01:33:47.020  1580  1580 I SystemServer: StartDevicePolicyManager
05-15 01:33:47.020  1580  1580 I SystemServiceManager: Starting com.android.server.devicepolicy.DevicePolicyManagerService$Lifecycle
05-15 01:33:47.023  1580  1580 D SystemServerTiming: StartDevicePolicyManager took to complete: 3ms
05-15 01:33:47.023  1580  1580 I SystemServer: StartStatusBarManagerService
05-15 01:33:47.024  1580  1580 D SystemServerTiming: StartStatusBarManagerService took to complete: 1ms
05-15 01:33:47.024  1580  1580 I SystemServer: StartClipboardService
05-15 01:33:47.024  1580  1580 I SystemServiceManager: Starting com.android.server.clipboard.ClipboardService
05-15 01:33:47.025  1580  1580 D SystemServerTiming: StartClipboardService took to complete: 1ms
05-15 01:33:47.025  1580  1580 I SystemServer: StartNetworkManagementService
05-15 01:33:47.026  1580  2135 I NetworkManagement: onDaemonConnected()
05-15 01:33:47.027  1580  1580 D SystemServerTiming: StartNetworkManagementService took to complete: 2ms
05-15 01:33:47.027  1580  1580 I SystemServer: StartTextServicesManager
05-15 01:33:47.027  1580  1580 I SystemServiceManager: Starting com.android.server.TextServicesManagerService$Lifecycle
05-15 01:33:47.031  1580  1580 D SystemServerTiming: StartTextServicesManager took to complete: 4ms
05-15 01:33:47.031  1580  1580 I SystemServer: StartNetworkScoreService
05-15 01:33:47.032  1580  1580 D SystemServerTiming: StartNetworkScoreService took to complete: 0ms
05-15 01:33:47.032  1580  1580 I SystemServer: StartNetworkStatsService
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:284)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.032  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.035  1580  1580 W SystemServer: ***********************************************
05-15 01:33:47.035  1580  1580 E SystemServer: BOOT FAILURE starting NetworkStats Service
05-15 01:33:47.035  1580  1580 E SystemServer: java.lang.NullPointerException: missing AlarmManager
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.server.net.NetworkStatsService.<init>(NetworkStatsService.java:309)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.server.net.NetworkStatsService.create(NetworkStatsService.java:289)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1087)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.035  1580  1580 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.035  1580  1580 D SystemServerTiming: StartNetworkStatsService took to complete: 4ms
05-15 01:33:47.035  1580  1580 I SystemServer: StartNetworkPolicyManagerService
05-15 01:33:47.036  1580  1580 W SystemServer: ***********************************************
05-15 01:33:47.037  1580  1580 E SystemServer: BOOT FAILURE starting NetworkPolicy Service
05-15 01:33:47.037  1580  1580 E SystemServer: java.lang.NullPointerException: missing networkStats
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:501)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.server.net.NetworkPolicyManagerService.<init>(NetworkPolicyManagerService.java:487)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1096)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.037  1580  1580 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.037  1580  1580 D SystemServerTiming: StartNetworkPolicyManagerService took to complete: 2ms
05-15 01:33:47.037  1580  1580 I SystemServer: StartWifi
05-15 01:33:47.038  1580  1580 I SystemServiceManager: Starting com.android.server.wifi.WifiService
05-15 01:33:47.047  1580  1580 D WifiApConfigStore: 2G band allowed channels are:1,6,11
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiConfigStore.<init>(WifiConfigStore.java:147)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiInjector.<init>(WifiInjector.java:190)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiService.<init>(WifiService.java:32)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance0(Native Method)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance(Constructor.java:334)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:96)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1106)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.048  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.internal.util.WakeupMessage.<init>(WakeupMessage.java:54)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.internal.util.WakeupMessage.<init>(WakeupMessage.java:73)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.net.ip.IpManager.<init>(IpManager.java:672)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at android.net.ip.IpManager.<init>(IpManager.java:590)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.FrameworkFacade.makeIpManager(FrameworkFacade.java:142)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiStateMachine.<init>(WifiStateMachine.java:959)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiInjector.<init>(WifiInjector.java:222)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiService.<init>(WifiService.java:32)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance0(Native Method)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance(Constructor.java:334)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:96)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1106)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.069  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.internal.util.WakeupMessage.<init>(WakeupMessage.java:54)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.internal.util.WakeupMessage.<init>(WakeupMessage.java:73)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.net.ip.IpManager.<init>(IpManager.java:674)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at android.net.ip.IpManager.<init>(IpManager.java:590)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.FrameworkFacade.makeIpManager(FrameworkFacade.java:142)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiStateMachine.<init>(WifiStateMachine.java:959)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiInjector.<init>(WifiInjector.java:222)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiService.<init>(WifiService.java:32)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance0(Native Method)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance(Constructor.java:334)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:96)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1106)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.070  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.071  1539  1563 D CommandListener: Clearing all IP addresses on wlan0
05-15 01:33:47.071  1580  2142 E HalDeviceManager: isSupported: called but mServiceManager is null!?
05-15 01:33:47.071  1580  2142 I WifiNative-wlan0: Vendor HAL not supported, Ignore stop...
05-15 01:33:47.072  1580  2142 D WificondControl: tearing down interfaces in wificond
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiController.<init>(WifiController.java:154)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiInjector.<init>(WifiInjector.java:233)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.WifiService.<init>(WifiService.java:32)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance0(Native Method)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance(Constructor.java:334)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:96)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1106)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.074  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.075  1580  1580 D WifiController: isAirplaneModeOn = false, isWifiEnabled = true, isScanningAvailable = false
05-15 01:33:47.076  1580  1580 I WifiService: getVerboseLoggingLevel uid=1000
05-15 01:33:47.076  1580  1580 E SupplicantStaIfaceHal: Can't call setDebugParams, ISupplicant is null
05-15 01:33:47.076  1580  1580 W WifiDiags: no ring buffers found
05-15 01:33:47.076  1580  1580 W WifiDiags: Failed to start packet fate monitoring
05-15 01:33:47.076  1580  1580 I WifiService: Registering wifi
05-15 01:33:47.077  1580  1580 D SystemServerTiming: StartWifi took to complete: 40ms
05-15 01:33:47.077  1580  1580 I SystemServer: StartWifiScanning
05-15 01:33:47.077  1580  1580 I SystemServiceManager: Starting com.android.server.wifi.scanner.WifiScanningService
05-15 01:33:47.077  1580  1580 I WifiScanningService: Creating wifiscanner
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.scanner.WifiScanningServiceImpl.<init>(WifiScanningServiceImpl.java:284)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.wifi.scanner.WifiScanningService.<init>(WifiScanningService.java:38)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance0(Native Method)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Constructor.newInstance(Constructor.java:334)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:96)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:70)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1109)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.078  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.079  1580  1580 I WifiScanningService: Publishing wifiscanner
05-15 01:33:47.079  1580  1580 D SystemServerTiming: StartWifiScanning took to complete: 2ms
05-15 01:33:47.079  1580  1580 I SystemServer: StartWifiRtt
05-15 01:33:47.079  1580  1580 I SystemServiceManager: Starting com.android.server.wifi.RttService
05-15 01:33:47.079  1580  1580 I RttService: Creating rttmanager
05-15 01:33:47.079  1580  1580 I RttService: Starting rttmanager
05-15 01:33:47.080  1580  1580 D SystemServerTiming: StartWifiRtt took to complete: 0ms
05-15 01:33:47.080  1580  1580 I SystemServer: No Wi-Fi Aware Service (Aware support Not Present)
05-15 01:33:47.080  1580  1580 I SystemServer: StartWifiP2P
05-15 01:33:47.080  1580  1580 I SystemServiceManager: Starting com.android.server.wifi.p2p.WifiP2pService
05-15 01:33:47.083  1580  1580 I WifiP2pService: Registering wifip2p
05-15 01:33:47.083  1580  1580 D SystemServerTiming: StartWifiP2P took to complete: 4ms
05-15 01:33:47.083  1580  1580 I SystemServer: StartEthernet
05-15 01:33:47.083  1580  1580 I SystemServiceManager: Starting com.android.server.ethernet.EthernetService
05-15 01:33:47.084  1580  1580 I EthernetServiceImpl: Creating EthernetConfigStore
05-15 01:33:47.084  1580  1580 E IpConfigStore: Error opening configuration file: java.io.FileNotFoundException: /data/misc/ethernet/ipconfig.txt (No such file or directory)
05-15 01:33:47.084  1580  1580 W EthernetConfigStore: No Ethernet configuration found. Using default.
05-15 01:33:47.084  1580  1580 I EthernetServiceImpl: Read stored IP configuration: IP assignment: DHCP
05-15 01:33:47.084  1580  1580 I EthernetServiceImpl: Proxy settings: NONE
05-15 01:33:47.085  1580  1580 I EthernetService: Registering service ethernet
05-15 01:33:47.086  1580  1580 D SystemServerTiming: StartEthernet took to complete: 3ms
05-15 01:33:47.086  1580  1580 I SystemServer: StartConnectivityService
05-15 01:33:47.088  1580  1580 D ConnectivityService: ConnectivityService starting up
05-15 01:33:47.089  1580  1580 W SystemServer: ***********************************************
05-15 01:33:47.089  1580  1580 E SystemServer: BOOT FAILURE starting Connectivity Service
05-15 01:33:47.089  1580  1580 E SystemServer: java.lang.NullPointerException: missing INetworkStatsService
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.internal.util.Preconditions.checkNotNull(Preconditions.java:128)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:722)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.server.ConnectivityService.<init>(ConnectivityService.java:690)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1151)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.089  1580  1580 E SystemServer: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.089  1580  1580 D SystemServerTiming: StartConnectivityService took to complete: 3ms
05-15 01:33:47.089  1580  1580 I SystemServer: StartNsdService
05-15 01:33:47.090  1580  1580 D NsdService: Network service discovery is enabled
05-15 01:33:47.091  1580  1580 D SystemServerTiming: StartNsdService took to complete: 2ms
05-15 01:33:47.091  1580  1580 I SystemServer: StartUpdateLockService
05-15 01:33:47.091  1580  1580 D SystemServerTiming: StartUpdateLockService took to complete: 0ms
05-15 01:33:47.091  1580  1580 I SystemServer: WaitForAsecScan
05-15 01:33:47.091  1580  1580 D SystemServerTiming: WaitForAsecScan took to complete: 0ms
05-15 01:33:47.091  1580  1580 I SystemServer: StartNotificationManager
05-15 01:33:47.092  1580  1580 I SystemServiceManager: Starting com.android.server.notification.NotificationManagerService
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.notification.SnoozeHelper.<init>(SnoozeHelper.java:87)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.notification.NotificationManagerService.onStart(NotificationManagerService.java:1376)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:124)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:111)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1198)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.103  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: No service published for: alarm
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: alarm
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:211)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$5.createService(SystemServiceRegistry.java:209)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.notification.NotificationManagerService.init(NotificationManagerService.java:1272)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.notification.NotificationManagerService.onStart(NotificationManagerService.java:1394)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:124)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:111)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1198)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.106  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.110  1580  1580 D ConditionProviders.SCP: new ScheduleConditionProvider()
05-15 01:33:47.110  1580  1580 I ConditionProviders:  Allowing condition provider org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:47.111  1580  1580 I NotificationListeners:  Allowing notification listener org.lineageos.trebuchet/com.android.launcher3.notification.NotificationListener
05-15 01:33:47.111  1580  1580 I ConditionProviders:  Allowing condition provider com.android.camera2
05-15 01:33:47.111  1580  1580 D ZenLog  : set_zen_mode: off,init
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: No service published for: trust
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: android.os.ServiceManager$ServiceNotFoundException: No service published for: trust
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.os.ServiceManager.getServiceOrThrow(ServiceManager.java:75)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.KeyguardManager.<init>(KeyguardManager.java:331)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$24.createService(SystemServiceRegistry.java:365)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$24.createService(SystemServiceRegistry.java:363)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry$CachedServiceFetcher.getService(SystemServiceRegistry.java:973)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.SystemServiceRegistry.getSystemService(SystemServiceRegistry.java:925)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at android.app.ContextImpl.getSystemService(ContextImpl.java:1667)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at org.lineageos.internal.notification.LineageNotificationLights.<init>(LineageNotificationLights.java:126)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.notification.NotificationManagerService.onStart(NotificationManagerService.java:1448)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:124)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:111)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1198)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.113  1580  1580 E SystemServiceRegistry: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.121   526   526 D lights  : set_light_notification colorRGB=00000000, onMS=0, offMS=0
05-15 01:33:47.123  1580  1580 E System  : ******************************************
05-15 01:33:47.123  1580  1580 E System  : ************ Failure starting system services
05-15 01:33:47.123  1580  1580 E System  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:47.123  1580  1580 E System  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:47.123  1580  1580 E System  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.123  1580  1580 E System  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.123  1580  1580 E System  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.123  1580  1580 E System  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.123  1580  1580 E System  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.123  1580  1580 D SystemServerTiming: StartNotificationManager took to complete: 32ms
05-15 01:33:47.123  1580  1580 E Zygote  : System zygote died with exception
05-15 01:33:47.123  1580  1580 E Zygote  : java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:47.123  1580  1580 E Zygote  : 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:47.123  1580  1580 E Zygote  : 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.123  1580  1580 E Zygote  : 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.123  1580  1580 E Zygote  : 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.123  1580  1580 E Zygote  : 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.123  1580  1580 E Zygote  : 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.123  1580  1580 D AndroidRuntime: Shutting down VM
05-15 01:33:47.123  1580  1580 E AndroidRuntime: *** FATAL EXCEPTION IN SYSTEM PROCESS: main
05-15 01:33:47.123  1580  1580 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'void com.android.server.net.NetworkPolicyManagerService.bindNotificationManager(android.app.INotificationManager)' on a null object reference
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1202)
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at com.android.server.SystemServer.run(SystemServer.java:416)
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at com.android.server.SystemServer.main(SystemServer.java:279)
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:440)
05-15 01:33:47.123  1580  1580 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:787)
05-15 01:33:47.123  1580  1580 I Process : Sending signal. PID: 1580 SIG: 9
05-15 01:33:47.152   536   536 I lowmemorykiller: ActivityManager disconnected
05-15 01:33:47.152   536   536 I lowmemorykiller: Closing Activity Manager data connection
05-15 01:33:47.152  1535  1535 E Zygote  : Exit zygote because system server (1580) has terminated
05-15 01:33:47.152   384   384 I ServiceManager: service 'wifi' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'wifiscanner' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'rttmanager' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'wifip2p' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'ethernet' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'servicediscovery' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'updatelock' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'notification' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'meminfo' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'gfxinfo' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'dbinfo' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'cpuinfo' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'permission' died
05-15 01:33:47.153  1535  1535 F libc    : Fatal signal 6 (SIGABRT), code 0 in tid 1535 (main), pid 1535 (main)
05-15 01:33:47.153   384   384 I ServiceManager: service 'processinfo' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'user' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'otadexopt' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'package_native' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'package' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'battery' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'dropbox' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'overlay' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'usagestats' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'settings' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'vibrator' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'input_method' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'accessibility' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'mount' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'storagestats' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'uimode' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'webviewupdate' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'sec_key_att_app_id_provider' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'scheduling_policy' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'telephony.registry' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'account' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'content' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'lock_settings' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'deviceidle' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'device_policy' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'statusbar' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'clipboard' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'network_management' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'textservices' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'network_score' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'sensorservice' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'device_identifiers' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'batterystats' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'appops' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'power' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'recovery' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'display' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'activity' died
05-15 01:33:47.153   384   384 I ServiceManager: service 'procstats' died
05-15 01:33:47.173  2155  2155 I crash_dump64: obtaining output fd from tombstoned, type: kDebuggerdTombstone
05-15 01:33:47.173   751   751 I /system/bin/tombstoned: received crash request for pid 1535
05-15 01:33:47.174  2155  2155 I crash_dump64: performing dump of process 1535 (target tid = 1535)
05-15 01:33:47.174  2155  2155 F DEBUG   : *** *** *** *** *** *** *** *** *** *** *** *** *** *** *** ***
05-15 01:33:47.174  2155  2155 F DEBUG   : LineageOS Version: 'unknown'
05-15 01:33:47.174  2155  2155 F DEBUG   : Build fingerprint: 'Android/treble_arm64_avN/phhgsi_arm64_a:8.1.0/OPM2.171019.029.B1/180514:userdebug/test-keys'
05-15 01:33:47.174  2155  2155 F DEBUG   : Revision: '0'
05-15 01:33:47.174  2155  2155 F DEBUG   : ABI: 'arm64'
05-15 01:33:47.174  2155  2155 F DEBUG   : pid: 1535, tid: 1535, name: main  >>> zygote64 <<<
05-15 01:33:47.174  2155  2155 F DEBUG   : signal 6 (SIGABRT), code 0 (SI_USER), fault addr --------
05-15 01:33:47.174  2155  2155 F DEBUG   :     x0   0000000000000000  x1   0000000000000009  x2   0000000000000005  x3   0000000000000003
05-15 01:33:47.174  2155  2155 F DEBUG   :     x4   0000000040100401  x5   a802a00080404000  x6   0000000000000000  x7   7f7f7f7f7f7f7f7f
05-15 01:33:47.174  2155  2155 F DEBUG   :     x8   0000000000000081  x9   e6e0840440b9944b  x10  0000007ff3056d00  x11  0000000000000038
05-15 01:33:47.174  2155  2155 F DEBUG   :     x12  000000000000000b  x13  ffffffffffffffff  x14  ff00000000000000  x15  ffffffffffffffff
05-15 01:33:47.174  2155  2155 F DEBUG   :     x16  00000071293b8300  x17  000000712a6c155c  x18  0000000070de6150  x19  000000712d3bca50
05-15 01:33:47.174  2155  2155 F DEBUG   :     x20  00000071293641e6  x21  000000712936464a  x22  00000071293646a6  x23  000000000000062c
05-15 01:33:47.174  2155  2155 F DEBUG   :     x24  000000712936468e  x25  0000007129364669  x26  000000712d3bca40  x27  0000000000000002
05-15 01:33:47.174  2155  2155 F DEBUG   :     x28  00000071293bd000  x29  0000007ff30572d0  x30  000000712931e00c
05-15 01:33:47.174  2155  2155 F DEBUG   :     sp   0000007ff3057270  pc   000000712a6c1564  pstate 0000000060000000
05-15 01:33:47.409  2155  2155 F DEBUG   : 
05-15 01:33:47.409  2155  2155 F DEBUG   : backtrace:
05-15 01:33:47.409  2155  2155 F DEBUG   :     #00 pc 000000000006a564  /system/lib64/libc.so (kill+8)
05-15 01:33:47.409  2155  2155 F DEBUG   :     #01 pc 0000000000176008  /system/lib64/libandroid_runtime.so ((anonymous namespace)::SigChldHandler(int)+280)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #02 pc 00000000000005f0  [vdso:000000712d251000]
05-15 01:33:47.410  2155  2155 F DEBUG   :     #03 pc 0000000000069ea0  /system/lib64/libc.so (__ppoll+4)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #04 pc 00000000000265e4  /system/lib64/libc.so (poll+88)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #05 pc 000000000002e9a8  /system/lib64/libjavacore.so (Linux_poll(_JNIEnv*, _jobject*, _jobjectArray*, int)+800)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #06 pc 000000000030bad0  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.Linux.fcntlVoid [DEDUPED]+160)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #07 pc 0000000000300a74  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (libcore.io.BlockGuardOs.poll+228)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #08 pc 00000000002b67a4  /system/framework/arm64/boot-core-libart.oat (offset 0xd5000) (android.system.Os.poll+84)
05-15 01:33:47.410  2155  2155 F DEBUG   :     #09 pc 000000000164e488  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteServer.runSelectLoop+664)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #10 pc 0000000001652ed8  /system/framework/arm64/boot-framework.oat (offset 0x614000) (com.android.internal.os.ZygoteInit.main+2728)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #11 pc 000000000054744c  /system/lib64/libart.so (art_quick_invoke_static_stub+604)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #12 pc 00000000000dc7b0  /system/lib64/libart.so (art::ArtMethod::Invoke(art::Thread*, unsigned int*, unsigned int, art::JValue*, char const*)+260)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #13 pc 000000000046bb70  /system/lib64/libart.so (art::InvokeWithArgArray(art::ScopedObjectAccessAlreadyRunnable const&, art::ArtMethod*, art::ArgArray*, art::JValue*, char const*)+100)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #14 pc 000000000046b79c  /system/lib64/libart.so (art::InvokeWithVarArgs(art::ScopedObjectAccessAlreadyRunnable const&, _jobject*, _jmethodID*, std::__va_list)+420)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #15 pc 0000000000372a54  /system/lib64/libart.so (art::JNI::CallStaticVoidMethodV(_JNIEnv*, _jclass*, _jmethodID*, std::__va_list)+620)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #16 pc 00000000000a6fb8  /system/lib64/libandroid_runtime.so (_JNIEnv::CallStaticVoidMethod(_jclass*, _jmethodID*, ...)+120)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #17 pc 00000000000a9728  /system/lib64/libandroid_runtime.so (android::AndroidRuntime::start(char const*, android::Vector<android::String8> const&, bool)+832)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #18 pc 0000000000002440  /system/bin/app_process64 (main+1328)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #19 pc 00000000000a14d4  /system/lib64/libc.so (__libc_init+88)
05-15 01:33:47.415  2155  2155 F DEBUG   :     #20 pc 0000000000001e70  /system/bin/app_process64 (_start_main+80)
05-15 01:33:47.547  2155  2155 E crash_dump64: unable to connect to activity manager: No such file or directory
05-15 01:33:47.547   751   751 E /system/bin/tombstoned: Tombstone written to: /data/tombstones/tombstone_02
05-15 01:33:47.609     1     1 W init    : type=1400 audit(0.0:162): avc: granted { open } for path="/dev/hw_bfm" dev="tmpfs" ino=9613 scontext=u:r:init:s0 tcontext=u:object_r:bfmr_device:s0 tclass=chr_file
