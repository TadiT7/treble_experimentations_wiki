## Function Availability & Known Bugs 功能可用性和已知问题

**Bugs and untested items are shown bold. 3rd-party apps untested. 问题和未测试项以粗体显示。未测试第三方应用。**

* Camera 摄像头
  * Front 前置: OK
  * Rear 后置: Upper one 上方摄像头: **Not working 不可用**, Lower one 下方摄像头: OK
  * **Enabling Do Not Disturb (DND) will cause stock camera app to FC (force close). 开启勿扰会导致默认相机强行停止。**

* LED Light 呼吸灯: **Always on 常亮** *You may not be able to use front camera when LED light is off. Reboot may help. 呼吸灯灭则前置摄像头不可用。重启可能解决问题。*

* Speaker / Microphone 听筒/麦克风: OK

* Bluetooth 蓝牙
  * Music 音乐: OK
  * File Transfer 文件传输: OK
  * Headset (Calls) 通话: **Not working 不可用**

* Wi-Fi: OK

* RIL (Calls 通话 / SMS 短信 / Data 数据):
  * CMCC/CHN-UNICOM 中国移动/中国联通: OK, China Telecom 中国电信: **Untested 未测试**
  * Dual SIMs 双卡: OK
  * VoLTE: **Untested 未测试**
  * **MEID not found 未找到 MEID**

* Fingerprint Reader 指纹识别: *Varies by the manufacturer 因制造商而异*
  * FPC: OK
  * Goodix: **Not working 不可用**
  * *You can check the manufacturer using 3rd-party apps, or run `getprop | grep goodix` command in ADB shell/terminal, if you get any return, you may be using Goodix.  If you are sure you're using FPC, try flashing stock MIUI before flashing the ROM again. 你可以使用第三方应用查看制造商，或者在 ADB 命令行/终端中运行 `getprop | grep goodix` 命令，若有任何返回值，你有可能在使用 Goodix。如果你确信你在使用 FPC，在刷入 ROM 之前先刷入官方 MIUI。*

* Brightness control 亮度控制: **Bad 糟糕** *The brightness changes too fast, and it flashes when you lock the screen. 亮度变化过快，锁屏时屏幕会闪烁。*

* USB connection USB 连接: *Varies by Android system version 因 Android 系统版本而异*
  * 8.1: Charging 充电/USB Debugging USB 调试/USB Network Sharing USB 网络共享/MTP/PTP: OK
  * 9.0: Charging 充电/USB Debugging USB 调试/USB Network Sharing USB 网络共享: OK, MTP/PTP: **Not working 不可用**
  * *Quick charge works better than stock MIUI, but the phone didn't show the charging status while quick charging. 快充较官方 MIUI 表现更好，但快充时不显示充电信息。*

## How To Flash 如何刷入

* Backup your data 备份数据
* Unlock your phone 解锁手机
* Flash TWRP 刷入 TWRP
* Boot into TWRP and wipe /data, /cache and /system (Best format /data partition) 进入 TWRP，清除 /data、/cache 和 /system （最好格式化 /data 分区）
* Connect your phone to the computer, and mount /data partition via MTP 将手机与电脑连接，在 MTP 上挂在 /data 分区
* Copy system image into your phone 将系统映像复制到手机
* Flash system image in TWRP (Flashing in Fastboot will throw `FAILED (command write failed (Unknown error))`) 在 TWRP 内刷入系统映像（在 Fastboot 内刷入会显示 `FAILED (command write failed (Unknown error))`）

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

* **After v23, /data partition will be encrypted. Please backup your data before flashing. v23 版本后 /data 分区会被加密。请在刷入前备份数据。**
* **Some people reported that phone was muted, not be able to use camera, etc. after flashing 9.0 ROM. Best try flashing stock MIUI before flashing the ROM. 有人报告刷入后手机出现静音、无法使用相机等问题。最好在刷入 ROM 前刷入官方 MIUI。**
* Xiaomi Mi 6X (wayne) is similar to Xiaomi Mi A2 (jasmine), but the latter one has A/B partitions, the former one only have A partition. 小米 6X 和 小米 A2 相似，但后者拥有 A/B 分区，前者只有 A 分区。
* Rollback protection will be enabled for Xiaomi Mi 6X after MIUI Stable V9.6.4.0 / Dev 8.8.6. You can still flash GSI images, but you should avoid flashing any MIUI ROM older than those, or your phone will be bricked. (I (suwakowww) was using MIUI Dev 8.7.26 before flashing.) 小米 6X 将在 MIUI 稳定版 V9.6.4.0 / 开发版 8.8.6 之后开启防回刷机制。你仍可以刷入 GSI 映像，但你应避免刷入更早的 MIUI ROM，否则手机会变砖。（我（suwakowww）在刷入前使用 MIUI 开发版 8.7.26。）
* Installing Magisk doesn't affect the encryption, but you can find encryption disabling tools using search engines. 安装 Magisk 不影响加密，但你可以使用搜索引擎寻找取消加密的工具。

## Tested By 由以下人员测试

* suwakowww @ AOSP v22 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-07
* suwakowww @ AOSP v23 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-17
* suwakowww @ AOSP v101 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-22
* suwakowww @ AOSP v102 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-23
* best yuan(`16***37@qq.com`), isaacchen(`ti***64@gmail.com`), pipipig(`22***13@qq.com`), stubbom(`29***82@qq.com`), xcxmiku, 墨水淘气包(`17***32@qq.com`), etc. (sort by alphabet, are reported in QQ group) @ AOSP v102, AOSP v101, PixelExperience, etc. , 2018-08-25