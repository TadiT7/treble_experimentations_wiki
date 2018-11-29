## Function Availability & Known Bugs 功能可用性和已知问题

>**The following reports are retelling feedback from ``用户名需大于5位小于 @ Coolapk``.<br />以下报告为复述``用户名需大于5位小于 @ 酷安网``的反馈**

>**Bugs and untested items are shown bold. 3rd-party apps untested. 问题和未测试项以粗体显示。未测试第三方应用。**

* Camera 摄像头: **Untested 未测试**

* LED Light 呼吸灯: **Untested 未测试**

* Speaker / Microphone 听筒 / 麦克风: **Broken sound 破音**

* Bluetooth 蓝牙： **Untested 未测试**

* Wi-Fi: 
  * Client 客户端: OK
  * Server (Hotspot) 服务器 (热点): OK
    * **5GHz Wi-Fi hotspot is not working. 5GHz Wi-Fi 热点不可用。**
  * Cast 投屏: 
    * 8.1: **Untested 未测试**
    * 9.0: **Not working 不可用**

* RIL (Calls 通话 / SMS 短信 / Data 数据):
  * CMCC/CHN-UNICOM 中国移动/中国联通 (GSM/WCDMA/LTE FDD & TDD): **Untested 未测试**
  * CHN-CT 中国电信 (CDMA1X/CDMA2000/LTE FDD & TDD): **LTE Only by default 默认情况下仅限 4G 网络**
  * Dual SIMs 双卡: **Untested 未测试**
  * VoLTE: **Disabled by default 默认禁用** ([Fixable](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#volte-support) [可修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#volte-support))

* Fingerprint Reader 指纹识别: OK
  * **It will send "return (enter)" key in normal use. 在正常使用时会发送“回车”键。**

* Brightness control 亮度控制: **Flickering 闪屏**
    * **Auto brightness seems not working. 自动亮度似乎不可用。**
    * **The minimum brightness is still brighter. 最低亮度仍然比较亮。**-->[#224](https://github.com/phhusson/treble_experimentations/issues/224)

* USB connection USB 连接: **Untested 未测试**

## How To Flash 如何刷入

* **Untold 未说明**

## Notes 注意事项

* If you living in China, recommends to logout your Google Account and pull out all of your SIM card first, or it may let you stuck on "Checking information" after flashed. 如果你在中国居住，建议在刷入前退出你的 Google 账户并取出所有 SIM 卡，否则有可能在“正在核对信息”处卡住。

## Notes about Custom ROMs 关于自定义 ROM 的注意事项

* None for now. 暂无。

## Tested By 由以下人员测试

* 用户名需大于5位小于 @ AOSP v107 @ system-arm64-aonly-gapps-su.img, 2018-11-28