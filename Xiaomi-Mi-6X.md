## Function Availability & Known Bugs 功能可用性和已知问题

>**The following reports are based on MIUI 10 (8.7.26), if you have any bugs and based on custom roms, ask author of the rom first, or flash back MIUI before flash GSI.<br />以下报告基于 MIUI 10（8.7.26），如果你在遇到 bug，并且使用过自定义刷机包，请先联系刷机包的作者，或者先刷回 MIUI 然后再刷 GSI。**

>**Bugs and untested items are shown bold. 3rd-party apps untested. 问题和未测试项以粗体显示。未测试第三方应用。**

>**[Temp patches have been moved here.](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us) [临时补丁已经转移至这里。](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn)**

* Camera 摄像头
  * Front 前置: OK (AOSP 9.0 v106+) / [Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#flashlight) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#flashlight) (AOSP 8.1/AOSP 9.0 v105-)

  * Rear 后置: 
    * Upper one 上方摄像头: **Not working 不可用** ([Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#dual-cam) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#dual-cam))
    * Lower one 下方摄像头: OK
  * **Enabling Do Not Disturb (DND) will cause stock camera app to FC (force close). 开启勿扰会导致默认相机强行停止。**-->[#161](https://github.com/phhusson/treble_experimentations/issues/161)

* LED Light 呼吸灯: OK (AOSP 9.0 v104+ / AOSP 8.1 v25)
    * *If the light always on, reboot may help. 如果呼吸灯常亮，重启可能解决问题。*-->[#197](https://github.com/phhusson/treble_experimentations/issues/197)

* Speaker / Microphone 听筒/麦克风: OK

* Bluetooth 蓝牙
  * Music 音乐: OK
  * File Transfer 文件传输: OK
  * Headset (Calls) 通话: **Not working 不可用**-->[#177](https://github.com/phhusson/treble_experimentations/issues/177)

* Wi-Fi: 
  * Client 客户端: OK
  * Server (Hotspot) 服务器 (热点): OK (AOSP 8.1 v22+ / AOSP 9.0 v107+)
    * **5GHz Wi-Fi hotspot is not working. 5GHz Wi-Fi 热点不可用。**
  * Cast 投屏: 
    * 8.1: **Untested 未测试**
    * 9.0: **Not working 不可用**

* RIL (Calls 通话 / SMS 短信 / Data 数据):
  * CMCC/CHN-UNICOM 中国移动/中国联通: OK
  * CHN-CT 中国电信: **LTE Only by default 默认情况下仅限 4G 网络** ([Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#cdma-network) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#cdma-network))
  * Dual SIMs 双卡: OK
  * VoLTE: **Disabled by default 默认禁用** ([Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#volte-support) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#volte-support))

* Fingerprint Reader 指纹识别: *Varies by the manufacturer 因制造商而异*
  * FPC: OK (AOSP 9.0 v107+)
  * Goodix: **Not working 不可用**-->[#237](https://github.com/phhusson/treble_experimentations/issues/237)
  * *You can check the manufacturer using 3rd-party apps, or run `getprop | grep goodix` command in ADB shell/terminal, if you get any return, you may be using Goodix.  If you are sure you're using FPC, try flashing stock MIUI before flashing the ROM again. 你可以使用第三方应用查看制造商，或者在 ADB 命令行/终端中运行 `getprop | grep goodix` 命令，若有任何返回值，你有可能在使用 Goodix。如果你确信你在使用 FPC，在刷入 ROM 之前先刷入官方 MIUI。*

* Brightness control 亮度控制: OK (AOSP 9.0 v107+ / AOSP 8.1 v25)
    * **The minimum brightness is still brighter. 最低亮度仍然比较亮。**-->[#224](https://github.com/phhusson/treble_experimentations/issues/224)

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
      * MTP/PTP: **Not working 不可用**-->[#225](https://github.com/phhusson/treble_experimentations/issues/225)
      * OTG: OK
        * *If you can't use otg, please change better one. 如果你不能使用 OTG，请换一根好一点的线缆。*
  * *Quick charge works better than stock MIUI, but the phone didn't show the charging status while quick charging. 快充较官方 MIUI 表现更好，但快充时不显示充电信息。*

* Sensors 传感器:
  * Pedometer 计步器：
    * 8.1: **Untested 未测试**
    * 9.0: **Always zero 始终为零**

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

## Notes 注意事项

* **After v23, `/data` partition will be encrypted. Please backup your data before flashing. v23 版本后 `/data` 分区会被加密。请在刷入前备份数据。**-->[Disable Encryption](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#disable-encryption) [禁用加密](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#disable-encryption)
* **Rollback protection will be enabled for Xiaomi Mi 6X after MIUI Stable V9.6.4.0 / Dev 8.8.6. You can still flash GSI images after those version, but you should avoid flashing any MIUI ROM older than those, or your phone will be bricked. 小米 6X 将在 MIUI 稳定版 V9.6.4.0 / 开发版 8.8.6 之后开启防回刷机制。你仍可以刷入 GSI 映像，但你应避免刷入更早的 MIUI ROM，否则手机会变砖。**
  * *It's not affected if you never flash after those version. 如从未刷入过这些版本则不受影响。*
* Xiaomi Mi 6X (wayne) is similar to Xiaomi Mi A2 (jasmine), but the latter one has A/B partitions, the former one only have A partition. 小米 6X 和 小米 A2 相似，但后者拥有 A/B 分区，前者只有 A 分区。

## Notes about Custom ROMs 关于自定义 ROM 的注意事项

* Some people reported that brightness are locked (based on AOSPExtended), the maintainer ([fatesay](https://github.com/bin8001)) recommended to flash other custom roms first. 有人报告在使用过 AOSPExtended 然后刷入 GSI 会出现亮度被锁定的问题，维护人员（[fatesay](https://github.com/bin8001)）建议先行刷入其它自定义刷机包。
* Some people reported that phone was muted, not be able to use camera, etc. after flashing 9.0 ROM. Best try flashing stock MIUI before flashing the ROM. 有人报告刷入后手机出现静音、无法使用相机等问题。最好在刷入 ROM 前刷入官方 MIUI。


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
* suwakowww @ AOSP v105 @ system-arm64-aonly-gapps-su.img, 2018-09-19
* suwakowww @ AOSP v106 @ system-arm64-aonly-gapps-su.img, 2018-10-03
* markg85 @ AOSP v106, AOSP v107 @ unknown, 2018-11-10, 2018-11-09, **Boot loop [#281](https://github.com/phhusson/treble_experimentations/issues/281)**
* suwakowww @ AOSP v107 @ system-arm64-aonly-gapps-su.img, 2018-11-10