## Function Availability & Known Bugs 功能可用性和已知问题

**Bugs and untested items are shown bold. 3rd-party apps untested. 问题和未测试项以粗体显示。未测试第三方应用。**

* Camera 摄像头
  * Front 前置: OK
    * **Flash light will always on when using. 闪光灯在使用摄像头时会常亮。**-->[#169](https://github.com/phhusson/treble_experimentations/issues/169)
  * Rear 后置: Upper one 上方摄像头: **Not working 不可用**, Lower one 下方摄像头: OK
    * You can append `persist.camera.expose.aux=1` to `/system/build.prop` and reboot to "enable" the upper-one camera, **but seems still not working in camera app** (Can be detected but can't use). 你可以往`/system/build.prop`追加`persist.camera.expose.aux=1`并重启以“启用”上方的摄像头，**但似乎在相机应用仍然不可用**（可以被检测到但无法使用）。
  * **Enabling Do Not Disturb (DND) will cause stock camera app to FC (force close). 开启勿扰会导致默认相机强行停止。**-->[#161](https://github.com/phhusson/treble_experimentations/issues/161)

* LED Light 呼吸灯: OK (AOSP v104 / AOSP v25)

* Speaker / Microphone 听筒/麦克风: OK

* Bluetooth 蓝牙
  * Music 音乐: OK
  * File Transfer 文件传输: OK
  * Headset (Calls) 通话: **Not working 不可用**-->[#177](https://github.com/phhusson/treble_experimentations/issues/177)

* Wi-Fi: 
  * Client 客户端: OK
  * Server (Hotspot) 服务器 (热点): *Varies by Android system version 因 Android 系统版本而异*
      * 8.1: OK
      * 9.0: **Not working 不可用**

* RIL (Calls 通话 / SMS 短信 / Data 数据):
  * CMCC/CHN-UNICOM 中国移动/中国联通: OK
  * CHN-CT 中国电信: **LTE Only by default**, *but you can try to enable CDMA1x / CDMA2000 network:* **默认情况下仅限 4G 网络**，*但你可以尝试启用CDMA1x / CDMA2000 网络：*
    1. *Insert UIM card (best for slot 1 or single card) 插入 UIM 卡（最好放卡 1 插槽或者单卡）*
    2. *Disable "Enhanced 4G LTE Mode" 禁用“增强型 4G LTE 模式”*
    3. *That's all. MEID should be found now. 完成。MEID 应该能找到了。*
  * Dual SIMs 双卡: OK
  * VoLTE: **Disabled by default**, *but you can try to enable it:* **默认禁用**，*但你可以尝试启用它：*
    1. *Append `persist.dbg.volte_avail_ovr=1` to `/system/build.prop` and reboot to enable VoLTE support. 往`/system/build.prop`追加`persist.dbg.volte_avail_ovr=1`并重启以启用 VoLTE 支持。*
    2. *Install `org.codeaurora.ims.apk` (find it yourself) and reboot you phone once or twice. 安装`org.codeaurora.ims.apk`（自己找）然后重启手机（如不行再重启一遍）。*

* Fingerprint Reader 指纹识别: *Varies by the manufacturer 因制造商而异*
  * FPC: OK
    * **It will send "return (enter)" key in normal use. 在正常使用时会发送“回车”键。**
  * Goodix: **Not working 不可用**
  * *You can check the manufacturer using 3rd-party apps, or run `getprop | grep goodix` command in ADB shell/terminal, if you get any return, you may be using Goodix.  If you are sure you're using FPC, try flashing stock MIUI before flashing the ROM again. 你可以使用第三方应用查看制造商，或者在 ADB 命令行/终端中运行 `getprop | grep goodix` 命令，若有任何返回值，你有可能在使用 Goodix。如果你确信你在使用 FPC，在刷入 ROM 之前先刷入官方 MIUI。*

* Brightness control 亮度控制: OK (AOSP v104 / AOSP v25)
    * **Auto brightness seems not working. 自动亮度似乎不可用。**

* USB connection USB 连接: *Varies by Android system version 因 Android 系统版本而异*
  * 8.1: 
      * Charging 充电: OK
      * USB Debugging USB 调试: OK
      * USB Network Sharing USB 网络共享: OK
      * MTP/PTP: OK
  * 9.0: 
      * Charging 充电: OK
      * Reverse Charging 反向充电: OK
      * USB Debugging USB 调试: OK
      * USB Network Sharing USB 网络共享: OK
      * Audio Jack 耳机插槽: OK
      * MTP/PTP: **Not working 不可用**
      * OTG: **Not Working 不可用**
  * *Quick charge works better than stock MIUI, but the phone didn't show the charging status while quick charging. 快充较官方 MIUI 表现更好，但快充时不显示充电信息。*

## How To Flash 如何刷入

* Backup your data 备份数据
* Unlock your phone 解锁手机
* Flash TWRP 刷入 TWRP
* Boot into TWRP and wipe `/data`, `/cache`, `/dalvik-cache` and `/system` (Best format whole `/data` partition) 进入 TWRP，清除 `/data`、`/cache`、`/dalvik-cache` 和 `/system` （最好格式化整个 `/data` 分区）
* Connect your phone to the computer, and mount `/sdcard` partition via MTP 将手机与电脑连接，在 MTP 上挂载 `/sdcard` 分区
* Copy system image into your phone 将系统映像复制到手机
* Flash system image (`*.img` files) in TWRP (Flashing in Fastboot will throw `FAILED (command write failed (Unknown error))`) 在 TWRP 内刷入系统映像（`*.img` 文件，如在 Fastboot 内刷入会显示 `FAILED (command write failed (Unknown error))`）

(Flash in TWRP 在 TWRP 内刷入)

````
......
[镜像刷入开始]
刷入镜像：/sdcard/system-arm64-aonly-gapps-su.img
正在计算镜像刷入详情...
I:Image filename is: system-arm64-aonly-gapps-su.img
正在刷入System镜像...
I:Flash command: 'simg2img '/sdcard/system-arm64-aonly-gapps-su.img' '/dev/block/mmcblk0p61''
I:simg2img '/sdcard/system-arm64-aonly-gapps-su.img' '/dev/block/mmcblk0p61' process ended with RC=0
[镜像刷入完成]
I:Set page: 'action_complete'
I:operation_end - status=0
......
````
(Flash in Fastboot 在 Fastboot 内刷入)

````
fastboot flash system system-arm64-aonly-gapps-su.img
target reported max download size of 536870912 bytes
erasing 'system'...
OKAY [  0.546s]
sending sparse 'system' (524284 KB)...
OKAY [ 12.064s]
writing 'system'...
OKAY [  0.000s]
sending sparse 'system' (524284 KB)...
FAILED (command write failed (Unknown error))
finished. total time: 13.614s
````
* Reboot and Enjoy! 重启体验吧！

## Notes 注意

* **After v23, `/data` partition will be encrypted. Please backup your data before flashing. v23 版本后 `/data` 分区会被加密。请在刷入前备份数据。**
* **Some people reported that phone was muted, not be able to use camera, etc. after flashing 9.0 ROM. Best try flashing stock MIUI before flashing the ROM. 有人报告刷入后手机出现静音、无法使用相机等问题。最好在刷入 ROM 前刷入官方 MIUI。**
* Xiaomi Mi 6X (wayne) is similar to Xiaomi Mi A2 (jasmine), but the latter one has A/B partitions, the former one only have A partition. 小米 6X 和 小米 A2 相似，但后者拥有 A/B 分区，前者只有 A 分区。
* Rollback protection will be enabled for Xiaomi Mi 6X after MIUI Stable V9.6.4.0 / Dev 8.8.6. You can still flash GSI images after those version, but you should avoid flashing any MIUI ROM older than those, or your phone will be bricked. 小米 6X 将在 MIUI 稳定版 V9.6.4.0 / 开发版 8.8.6 之后开启防回刷机制。你仍可以刷入 GSI 映像，但你应避免刷入更早的 MIUI ROM，否则手机会变砖。
  * *It's not affected if you never flash after those version. (I (suwakowww) was using MIUI Dev 8.7.26 before flashing.) 如从未刷入过这些版本则不受影响。（我（suwakowww）在刷入前使用 MIUI 开发版 8.7.26。）*
* Installing Magisk doesn't affect the encryption, but you can find encryption disabling tools using search engines. 安装 Magisk 不影响加密，但你可以使用搜索引擎寻找取消加密的工具。
* If you confused by the wrong brand/model, you can modify `/system/build.prop` to fix it manually, just fint them and change below (case-sensitive): 如果你对手机品牌/型号有要求，可以自行修改`/system/build.prop`以修复，找到下面的配置并更改即可（区分大小写）：
````
ro.product.model=Mi 6X
ro.product.brand=xiaomi
ro.product.name=wayne
ro.product.device=wayne
ro.product.manufacturer=Xiaomi
````

## Tested By 由以下人员测试

* suwakowww @ AOSP v22 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-07
* suwakowww @ AOSP v23 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-17
* suwakowww @ AOSP v101 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-22
* suwakowww @ AOSP v102 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-23
* best yuan(`16***37@qq.com`), pipipig(`22***13@qq.com`), stubbom(`29***82@qq.com`), tingyichen, xcxmiku, 墨水淘气包(`17***32@qq.com`), etc. (sort by alphabet, are reported in QQ group) @ AOSP v102, AOSP v101, PixelExperience, etc. , 2018-08-25
* suwakowww @ AOSP v103 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-30
* markg85 @ AOSP v103, AOSP v23 @ unknown, 2018-09-01, [#168](https://github.com/phhusson/treble_experimentations/issues/168), [#169](https://github.com/phhusson/treble_experimentations/issues/169)
* suwakowww @ AOSP v104 @ system-arm64-aonly-vanilla-su.img, 2018-09-05
* markg85 @ AOSP v25 @ unknown, 2018-09-06