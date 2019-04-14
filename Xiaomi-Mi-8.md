<a href="#chinese">看不懂英文点这里。</a>

## Function Availability & Known Bugs

>**The following reports are based on MIUI 9 (9.5.11.0), if you have any bugs and based on custom roms, ask author of the rom first, or flash back MIUI before flash GSI.**<br />😀: OK&#9;😐: Fixable&#9;😢: **Not Working**&#9;🤔: **Untested**

* Camera

|Camera           |Status|Comment|
|:---------------:|:----:|-------|
|S5K2T7(Front)    |😀   |&nbsp;|
|S5K5E8(Rear,Aux) |😢   |&nbsp;|
|IMX363(Rear,Main)|😀   |&nbsp;|
|Unknown(IR)      |😢   |&nbsp;|


* Bluetooth

|Profile|Status|Comment|
|:-----:|:----:|-------|
|HFP    |😢   |[Issue #177](https://github.com/phhusson/treble_experimentations/issues/177)|
|A2DP   |😀   |&nbsp;|
|OBEX   |😀   |&nbsp;|


* Wi-Fi: 

|Item           |Status|Comment|
|:-------------:|:----:|-------|
|Client         |😀   |&nbsp;|
|Server(Hotspot)|😐   |**5GHz Wi-Fi hotspot is not working.**|
|Cast           |😢   |**Android 8.1 untested.**|


* RIL (Calls / SMS / Data):

    * Network

    |Type    |Operator              |Status|Comment|
    |:------:|:--------------------:|:----:|-------|
    |GSM     |CMCC/CHN-UNICOM       |😀   |&nbsp;|
    |CDMA 1X |CHN-CT                |😀   |&nbsp;|
    |WCDMA   |CHN-UNICOM            |😀   |&nbsp;|
    |TD-SCDMA|CMCC                  |🤔   |&nbsp;|
    |CDMA2000|CHN-CT                |😀   |&nbsp;|
    |LTE FDD |CHN-UNICOM/CHN-CT/CMCC|😀   |&nbsp;|
    |LTE TDD |CMCC/CHN-UNICOM/CHN-CT|😀   |&nbsp;|

    * Misc

    |Item     |Status|Comment|
    |:-------:|:----:|-------|
    |Dual SIMs|😀   |If you use CDMA network, you should put UIM card on slot1.|
    |VoLTE    |😐   |Disabled by default, [enable here](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#volte-support).|


* USB connection: *Varies by Android system version*

|Item               |8.1|9.0|Comment        |
|:-----------------:|:-:|:-:|---------------|
|Charging           |🤔|😀|*The phone didn't show the charging status while quick charging. (QC 3.0+ only, QC 2.0 and normal charging is OK)*|
|USB Debugging      |🤔|😀|&nbsp;|
|USB Network Sharing|🤔|😀|&nbsp;|
|MTP/PTP            |🤔|😀|&nbsp;|
|Reverse Charging   |🤔|😀|&nbsp;|
|Audio Jack         |🤔|😀|&nbsp;|
|OTG                |🤔|😀|*If you can't use otg, please change a better cable.*|


* Misc

|Item              |Status|Comment|
|:----------------:|:----:|-------|
|LED Light         |😀   |&nbsp; |
|Speaker           |😀   |&nbsp; |
|Microphone        |😀   |&nbsp; |
|Brightness        |😀   |&nbsp; |
|Fingerprint Reader|😀   |&nbsp; |
|NFC               |😀   |&nbsp; |


## How To Flash

* Backup your data
* Unlock your phone
* Flash TWRP
    * Flash twrp directly:
    ````
    fastboot flash recovery twrp-3.2.3-1-dipper.img
    ````
    * Then reboot to recovery.
* Boot into TWRP and wipe `/data`, `/cache`, `/dalvik-cache` and `/system` (Best format whole `/data` partition)
* Connect your phone to the computer, and mount `/sdcard` partition via MTP
* Copy system image into your phone
* Flash system image (`*.img` files) in TWRP
    >Maybe you should disable FBE (file-based encryption) before reboot
* Reboot and Enjoy!

## Notes

* If you living in China, recommends to logout your Google Account and pull out all of your SIM card first, or it may let you stuck on "Checking information" after flashed.

## Notes about Custom ROMs

* None for now. 暂无。

<a href="#testers">Tested version here.</a>

## <a name="chinese">功能可用性和已知问题</a>

>**以下报告基于 MIUI 9（9.5.11.0），如果你在遇到 bug，并且使用过自定义刷机包，请先联系刷机包的作者，或者先刷回 MIUI 然后再刷 GSI。**<br />😀：正常工作&#9;😐：可进行修复&#9;😢：**无法工作**&#9;🤔：**未测试**

* 摄像头

|摄像头            |状态  |注意事项|
|:----------------:|:----:|--------|
|S5K2T7（前置）    |😀   |&nbsp;  |
|S5K5E8（后置，主）|😢   |&nbsp;  |
|IMX363（后置，副）|😀   |&nbsp;  |
|未知（红外）      |😢   |&nbsp;  |


* 蓝牙

|配置|状态  |注意事项|
|:--:|:----:|--------|
|HFP |😢   |[Issue #177](https://github.com/phhusson/treble_experimentations/issues/177)|
|A2DP|😀   |&nbsp;|
|OBEX|😀   |&nbsp;|


* Wi-Fi: 

|项目           |状态  |注意事项|
|:-------------:|:----:|--------|
|客户端         |😀   |&nbsp;  |
|服务端（热点） |😐   |**5GHz Wi-Fi 热点不可用。**|
|投屏           |😢   |**Android 8.1 未测试。**|


* RIL（通话/短信/数据）：

    * 网络

    |网络制式|运营商                |状态  |注意事项|
    |:------:|:--------------------:|:----:|-------|
    |GSM     |移动/联通             |😀   |&nbsp;|
    |CDMA 1X |电信                  |😀   |&nbsp;|
    |WCDMA   |联通                  |😀   |&nbsp;|
    |TD-SCDMA|移动                  |🤔   |&nbsp;|
    |CDMA2000|电信                  |😀   |&nbsp;|
    |LTE FDD |联通/电信/移动        |😀   |&nbsp;|
    |LTE TDD |移动/联通/电信        |😀   |&nbsp;|

    * 杂项

    |项目 |状态  |注意事项|
    |:---:|:----:|--------|
    |双卡 |😀   |如果使用 CDMA 网络，建议把 UIM 卡放在插槽 1 上。|
    |VoLTE|😐   |默认禁用，[开启方法](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#volte-support)。|


* USB 连接: *因 Android 系统版本而异*

|项目        |8.1|9.0|注意事项       |
|:----------:|:-:|:-:|---------------|
|充电        |🤔|😀|*使用 QC 3.0 或以上快充时不显示充电信息。(QC 2.0或普通充电则正常)*。|
|USB 调试    |🤔|😀|&nbsp;|
|USB 网络共享|🤔|😀|&nbsp;|
|MTP/PTP     |🤔|😀|&nbsp;|
|反向充电    |🤔|😀|&nbsp;|
|音频插槽    |🤔|😀|&nbsp;|
|OTG         |🤔|😀|*如果你不能使用 OTG，请换一根好一点的线缆。*|


* 杂项

|项目    |状态  |注意事项|
|:------:|:----:|-------|
|呼吸灯  |😐   |&nbsp; |
|听筒    |😀   |&nbsp; |
|麦克风  |😀   |&nbsp; |
|亮度控制|😀   |&nbsp; |
|指纹识别|😀   |&nbsp; |
|NFC     |😀   |&nbsp; |


## 如何刷入

* 备份数据
* 解锁手机
* 刷入 TWRP
    * 直接进行刷入：
    ````
    fastboot flash recovery twrp-3.2.3-1-dipper.img
    ````
    * 然后重启到恢复环境。
* 进入 TWRP，清除 `/data`、`/cache`、`/dalvik-cache` 和 `/system` （最好格式化整个 `/data` 分区）
* 将手机与电脑连接，在 MTP 上挂载 `/sdcard` 分区
* 将系统映像复制到手机
* 在 TWRP 内刷入系统映像（`*.img` 文件）
    >可能你需要在重启前禁用 FBE（文件级加密）
* 重启体验吧！

## 注意事项

* 如果你在中国居住，建议在刷入前退出你的 Google 账户并取出所有 SIM 卡，否则有可能在“正在核对信息”处卡住。

## 关于自定义 ROM 的注意事项

* 暂无。

## <a name="testers">Tested By 由以下人员测试</a>

* AOSP 8.1

    * *Untested 未测试*
* AOSP 9.0

    * suwakowww @ AOSP v107 @ system-arm64-aonly-gapps-su.img, 2018-11-27
    * suwakowww @ AOSP v111 @ system-arm64-aonly-gapps-su.img, 2019-03-23

Template: @zguithues, @hackintosh5, @suwakowww

Chinese version: @suwakowww