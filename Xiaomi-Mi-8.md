## Function Availability & Known Bugs 功能可用性和已知问题

>**The following reports are based on MIUI 9 (9.5.11.0), if you have any bugs and based on custom roms, ask author of the rom first, or flash back MIUI before flash GSI.<br />以下报告基于 MIUI 9（9.5.11.0），如果你在遇到 bug，并且使用过自定义刷机包，请先联系刷机包的作者，或者先刷回 MIUI 然后再刷 GSI。**

>**Bugs and untested items are shown bold. 3rd-party apps untested. 问题和未测试项以粗体显示。未测试第三方应用。**

* Camera 摄像头
  * Front 前置: OK
  * IRCamera 红外摄像头: **Not working 不可用**
  * Rear 后置: 
    * S5K3M3: **Not working 不可用**
    * IMX363: OK

* LED Light 呼吸灯: OK

* Speaker / Microphone 听筒 / 麦克风: OK

* Bluetooth 蓝牙
  * Music 音乐: OK
  * File Transfer 文件传输: OK
  * Headset (Calls) 通话: **Not working 不可用**

* Wi-Fi: 
  * Client 客户端: OK
  * Server (Hotspot) 服务器 (热点): OK (AOSP 8.1 v22+ / AOSP 9.0 v107+)
    * **5GHz Wi-Fi hotspot is not working. 5GHz Wi-Fi 热点不可用。**
  * Cast 投屏: 
    * 8.1: **Untested 未测试**
    * 9.0: **Not working 不可用**

* NFC: OK (Tested with WeChat 已使用微信测试)

* RIL (Calls 通话 / SMS 短信 / Data 数据):
  * CMCC/CHN-UNICOM 中国移动/中国联通 (GSM/WCDMA/LTE FDD & TDD): OK
  * CHN-CT 中国电信 (CDMA1X/CDMA2000/LTE FDD & TDD): OK
  * Dual SIMs 双卡: OK
  * VoLTE: **Disabled by default 默认禁用** ([Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#volte-support) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#volte-support))

* Fingerprint Reader 指纹识别: OK

* Brightness control 亮度控制: OK
    * **Auto brightness seems not working. 自动亮度似乎不可用。**
    * **The minimum brightness is still brighter. 最低亮度仍然比较亮。**-->[#224](https://github.com/phhusson/treble_experimentations/issues/224)

* USB connection USB 连接:
    * Charging 充电: OK
    * Reverse Charging 反向充电: OK
    * USB Debugging USB 调试: OK
    * USB Network Sharing USB 网络共享: OK
    * Audio Jack 耳机插槽: OK
    * MTP/PTP: OK
    * OTG: OK
    * *If you can't use otg, please change a better cable. 如果你不能使用 OTG，请换一根好一点的线缆。*
    * *The phone didn't show the charging status while quick charging. 快充时不显示充电信息。*

## How To Flash 如何刷入

* Backup your data 备份数据
* Unlock your phone 解锁手机
* Flash TWRP 刷入 TWRP
* Boot into TWRP and wipe `/data`, `/cache`, `/dalvik-cache` and `/system` (Best format whole `/data` partition) 进入 TWRP，清除 `/data`、`/cache`、`/dalvik-cache` 和 `/system` （最好格式化整个 `/data` 分区）
* Connect your phone to the computer, and mount `/sdcard` partition via MTP 将手机与电脑连接，在 MTP 上挂载 `/sdcard` 分区
* Copy system image into your phone 将系统映像复制到手机
* Flash system image (`*.img` files) in TWRP 在 TWRP 内刷入系统映像（`*.img` 文件）
  > Maybe you should disable FBE (file-based encryption) before reboot 可能你需要在重启前禁用 FBE（文件级加密）
* Reboot and Enjoy! 重启体验吧！

## Notes 注意事项

* None for now. 暂无。

## Notes about Custom ROMs 关于自定义 ROM 的注意事项

* None for now. 暂无。

## Tested By 由以下人员测试

* suwakowww @ AOSP v107 @ system-arm64-aonly-gapps-su.img, 2018-11-27