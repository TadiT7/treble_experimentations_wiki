<a href="#chinese">看不懂英文点这里。</a>

## Function Availability & Known Bugs

>**The following reports are based on MIUI 10 (8.7.26 / 10.0.2.0), if you have any bugs and based on custom roms, ask author of the rom first, or flash back MIUI before flash GSI.<br />Bugs and untested items are shown bold. 3rd-party apps untested.<br />[Temp patches have been moved here.](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us)**<br />😀: OK&#9;😐: Fixable&#9;😢: **Not Working**&#9;🤔: **Untested**

* Camera

|Camera             |Status|Comment|
|:---------------:|:----:|-------|
|IMX376(Front)    |😀   |If you found flashlight always on, [patch here](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#flashlight).|
|IMX376(Rear,Aux) |😐  |There is a way to fix it, but need [3rd-party patch](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#dual-cam).|
|IMX486(Rear,Main)|😀   |&nbsp;|


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
    |CDMA 1X |CHN-CT                |😐   |Disabled by default, [enable here](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#cdma-network).|
    |WCDMA   |CHN-UNICOM            |😀   |&nbsp;|
    |TD-SCDMA|CMCC                  |🤔   |&nbsp;|
    |CDMA2000|CHN-CT                |😐   |Disabled by default, [enable here](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#cdma-network).|
    |LTE FDD |CHN-UNICOM/CHN-CT/CMCC|😀   |&nbsp;|
    |LTE TDD |CMCC/CHN-UNICOM/CHN-CT|😀   |&nbsp;|

    * Misc

    |Item     |Status|Comment|
    |:-------:|:----:|-------|
    |Dual SIMs|😀   |If you use CDMA network, you should put UIM card on slot1.|
    |VoLTE    |😐   |Disabled by default, [enable here](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#volte-support).|


* Fingerprint Reader: *Varies by the manufacturer*
> *You can check the manufacturer using 3rd-party apps, or run `getprop | grep goodix` command in ADB shell/terminal, if you get any return, you may be using Goodix.  If you are sure you're using FPC, try flashing stock MIUI before flashing the ROM again.*

|Manufacturer|Status|Comment|
|:----------:|:----:|-------|
|FPC         |😀   |&nbsp; |
|Goodix      |😢   |[Issue #237](https://github.com/phhusson/treble_experimentations/issues/237)|


* USB connection: *Varies by Android system version*

|Item               |8.1|9.0|Comment        |
|:-----------------:|:-:|:-:|---------------|
|Charging           |😀|😀|*The phone didn't show the charging status while quick charging. (QC 3.0+ only, QC 2.0 and normal charging is OK)*|
|USB Debugging      |😀|😀|&nbsp;|
|USB Network Sharing|😀|😀|&nbsp;|
|MTP/PTP            |😀|😐|It's OK on Android 9 based MIUI ROM.|
|Reverse Charging   |🤔|😀|&nbsp;|
|Audio Jack         |🤔|😀|&nbsp;|
|OTG                |🤔|😀|*If you can't use otg, please change a better cable.*|


* Misc

|Item      |Status|Comment|
|:--------:|:----:|-------|
|LED Light |😐   |*If the light always on, reboot may help.*-->[#197](https://github.com/phhusson/treble_experimentations/issues/197)|
|Speaker   |😀   |&nbsp; |
|Microphone|😀   |&nbsp; |
|IR        |🤔   |&nbsp; |
|Brightness|😀   |&nbsp; |


## How To Flash

* Backup your data
* Unlock your phone
* Execute `fastboot getvar anti` to check anti version
* Flash TWRP
    * If you get anti <= 3:
        * Flash twrp directly:
        ````
        fastboot flash recovery twrp-3.2.3-1-wayne.img
        ````
        * Then reboot to recovery.
    * Or if you get anti >=4:
        * Flash `dummy.bin` first (find it yourself):
        ````
        fastboot flash antirbpass dummy.bin
        ````
        * Then flash TWRP:
        ````
        fastboot flash recovery twrp-3.2.3-1-wayne.img
        ````
        * Then reboot to recovery.
* Boot into TWRP and wipe `/data`, `/cache`, `/dalvik-cache` and `/system` (Best format whole `/data` partition)
* Connect your phone to the computer, and mount `/sdcard` partition via MTP
* Copy system image into your phone
* Flash system image (`*.img` files) in TWRP
* Reboot and Enjoy!
> If you get bootloop, try to flash Magisk before first boot (Magisk 16.7+ is recommended).

## Notes

* **After v23, `/data` partition will be encrypted. Please backup your data before flashing.**-->[Disable Encryption](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_en_us#disable-encryption)
* **Rollback protection will be enabled for Xiaomi Mi 6X after MIUI Stable V9.6.4.0 / Dev 8.8.6. You can still flash GSI images after those version, but you should avoid flashing any MIUI ROM older than those, or your phone will be bricked.**
  * *It's not affected if you never flash after those version.*
* **Enabling Do Not Disturb (DND) will cause stock camera app to FC (force close).**-->[#161](https://github.com/phhusson/treble_experimentations/issues/161)
    * *Some Camera apps (e.g: Google Camera) use Camera2 API, maybe they can work normally, but you should enable Camera2 API first.*
* Xiaomi Mi 6X (wayne) is similar to Xiaomi Mi A2 (jasmine), but the latter one has A/B partitions, the former one only have A partition.
* If you living in China, recommends to logout your Google Account and pull out all of your SIM card first, or it may let you stuck on "Checking information" after flashed.
* **AOSP 10.0 should uninstall Magisk to boot.(If you have.)**

## Notes about Custom ROMs

* Some people reported that brightness are locked (based on AOSPExtended), the maintainer ([fatesay](https://github.com/bin8001)) recommended to flash other custom roms first.
* Some people reported that phone was muted, not be able to use camera, etc. after flashing 9.0 ROM. Best try flashing stock MIUI before flashing the ROM.
* miui.eu maybe changed `ro.vendor.build.fingerprint`. If you found on `/vendor/build.prop` and it's not the value of REAL device, please check there is a key named `ro.vendor.build.fingerprint_real` and match for real device or not. If yes, please copy this value and replace the value of `ro.vendor.build.fingerprint`. [Releated thread here](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/aosp-9-0-phh-treble-t3831915/post78531166).

<a href="#testers">Tested version here.</a>

## <a name="chinese">功能可用性和已知问题</a>

>**以下报告基于 MIUI 10 (8.7.26 / 10.0.2.0) ，如果你在遇到 bug，并且使用过自定义刷机包，请先联系刷机包的作者，或者先刷回 MIUI 然后再刷 GSI。<br />问题和未测试项以粗体显示。未测试第三方应用。<br />[临时补丁已经转移至这里。](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn)**<br />😀：正常工作&#9;😐：可进行修复&#9;😢：**无法工作**&#9;🤔：**未测试**

* 摄像头

|摄像头            |状态  |注意事项|
|:----------------:|:----:|--------|
|IMX376（前置）    |😀   |如果发现闪光灯常亮， [可以尝试这个修复](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#flashlight)。|
|IMX376（后置、副）|😐   |可以使用[第三方补丁](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#dual-cam)进行修复。|
|IMX486（后置、主）|😀   |&nbsp;|


* 蓝牙

|配置|状态  |注意事项|
|:--:|:----:|--------|
|HFP |😢   |[Issue #177](https://github.com/phhusson/treble_experimentations/issues/177)|
|A2DP|😀   |&nbsp;|
|OBEX|😀   |&nbsp;|


* Wi-Fi: 

|项目           |状态  |注意事项|
|:-------------:|:----:|--------|
|客户端         |😀   |&nbsp;|
|服务端（热点） |😐   |**5GHz Wi-Fi 热点不可用。**|
|投屏           |😢   |**Android 8.1 未测试。**|


* RIL（通话/短信/数据）：

    * 网络

    |网络    |运营商                |状态  |注意事项|
    |:------:|:--------------------:|:----:|--------|
    |GSM     |移动/联通             |😀   |&nbsp;|
    |CDMA 1X |电信                  |😐   |默认禁用，[开启方法](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#cdma-network)。|
    |WCDMA   |联通                  |😀   |&nbsp;|
    |TD-SCDMA|移动                  |🤔   |&nbsp;|
    |CDMA2000|电信                  |😐   |默认禁用，[开启方法](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#cdma-network)。|
    |LTE FDD |联通/电信/移动        |😀   |&nbsp;|
    |LTE TDD |移动/联通/电信        |😀   |&nbsp;|

    * 杂项

    |项目 |状态  |注意事项|
    |:---:|:----:|--------|
    |双卡 |😀   |如果使用 CDMA 网络，建议把 UIM 卡放在插槽 1 上。|
    |VoLTE|😐   |默认禁用，[开启方法](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#volte-support)。|


* 指纹识别: *因制造商而异*
> *你可以使用第三方应用查看制造商，或者在 ADB 命令行/终端中运行 `getprop | grep goodix` 命令，若有任何返回值，你有可能在使用 Goodix 传感器。如果你确信你在使用 FPC，在刷入 ROM 之前先刷入官方 MIUI。*

|制造商|状态  |注意事项|
|:----:|:----:|--------|
|FPC   |😀   |&nbsp;  |
|Goodix|😢   |[Issue #237](https://github.com/phhusson/treble_experimentations/issues/237)|


* USB 连接: *因 Android 系统版本而异*

|项目        |8.1|9.0|注意事项       |
|:----------:|:-:|:-:|---------------|
|充电        |😀|😀|*使用 QC 3.0 或以上快充时不显示充电信息。(QC 2.0或普通充电则正常)*。|
|USB 调试    |😀|😀|&nbsp;|
|USB 网络共享|😀|😀|&nbsp;|
|MTP/PTP     |😀|😐|使用基于 Android 9 的 MIUI 作为基础包即正常。|
|反向充电    |🤔|😀|&nbsp;|
|音频插槽    |🤔|😀|&nbsp;|
|OTG         |🤔|😀|*如果你不能使用 OTG，请换一根好一点的线缆。*|


* 杂项

|项目    |状态  |注意事项|
|:------:|:----:|-------|
|呼吸灯  |😐   |*如果呼吸灯常亮，重启可能解决问题。*-->[#197](https://github.com/phhusson/treble_experimentations/issues/197)|
|听筒    |😀   |&nbsp; |
|麦克风  |😀   |&nbsp; |
|红外    |🤔   |&nbsp; |
|亮度控制|😀   |&nbsp; |


## 如何刷入

* 备份数据
* 解锁手机
* 执行 `fastboot getvar anti` 以检测 anti 的值
* 刷入 TWRP
    * 如果你没有防回刷 (anti <= 3)：
        * 直接进行刷入：
        ````
        fastboot flash recovery twrp-3.2.3-1-wayne.img
        ````
        * 然后重启到恢复环境。
    * 或者，如果你有防回刷 (anti >= 4)：
        * 先刷入 `dummy.bin`（自己找）：
        ````
        fastboot flash antirbpass dummy.bin
        ````
        * 然后刷入 TWRP：
        ````
        fastboot flash recovery twrp-3.2.3-1-wayne.img
        ````
        * 然后重启到恢复环境。
* 进入 TWRP，清除 `/data`、`/cache`、`/dalvik-cache` 和 `/system` （最好格式化整个 `/data` 分区）
* 将手机与电脑连接，在 MTP 上挂载 `/sdcard` 分区
* 将系统映像复制到手机
* 在 TWRP 内刷入系统映像（`*.img` 文件）
* 重启体验吧！
> 如果你遇到卡 Android logo，尝试刷入 Magisk 后进行首次开机（推荐 Magisk 16.7 以上版本）。

## 注意事项

* **v23 版本后 `/data` 分区会被加密。请在刷入前备份数据。**-->[禁用加密](https://github.com/MI6XDev/treble_fix_for_wayne/wiki/fix_zh_cn#disable-encryption)
* **小米 6X 将在 MIUI 稳定版 V9.6.4.0 / 开发版 8.8.6 之后开启防回刷机制。你仍可以刷入 GSI 映像，但你应避免刷入更早的 MIUI ROM，否则手机会变砖。**
  * *如从未刷入过这些版本则不受影响。*
* **开启勿扰会导致默认相机强行停止。**-->[#161](https://github.com/phhusson/treble_experimentations/issues/161)
    * *部分 app (例如: Google Camera) 使用了 Camera2 API，这些应用或许可以正常工作，但你需要先行开启 Camera2 API。*
* 小米 6X 和 小米 A2 相似，但后者拥有 A/B 分区，前者只有 A 分区。
* 如果你在中国居住，建议在刷入前退出你的 Google 账户并取出所有 SIM 卡，否则有可能在“正在核对信息”处卡住。
* **AOSP 10.0 目前需要卸载 Magisk 方可正常启动。**

## 关于自定义 ROM 的注意事项

* 有人报告在使用过 AOSPExtended 然后刷入 GSI 会出现亮度被锁定的问题，维护人员（[fatesay](https://github.com/bin8001)）建议先行刷入其它自定义刷机包。
* 有人报告刷入后手机出现静音、无法使用相机等问题。最好在刷入 ROM 前刷入官方 MIUI。
* miui.eu 可能会修改`ro.vendor.build.fingerprint`的值。如果发现`/vendor/build.prop`并非真实设备的值，请检测是否存在`ro.vendor.build.fingerprint_real`且为真实设备的值。如有则将此变量值替换`ro.vendor.build.fingerprint`的值。[相关帖子在这里（英文）](https://forum.xda-developers.com/project-treble/trebleenabled-device-development/aosp-9-0-phh-treble-t3831915/post78531166)。

## <a name="testers">Tested By 由以下人员测试</a>

* AOSP 8.1
    * suwakowww @ AOSP v22 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-07
    * suwakowww @ AOSP v23 @ system-arm64-aonly-gapps-su.img.xz, 2018-08-17
    * markg85 @ AOSP v23 @ unknown, 2018-09-01
    * markg85 @ AOSP v25 @ unknown, 2018-09-06
    * suwakowww @ AOSP v26 @ system-arm64-aonly-gapps-su.img, 2018-12-??
* AOSP 9.0
    * suwakowww @ AOSP v101 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-22
    * suwakowww @ AOSP v102 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-23
    * best yuan(`16***37@qq.com`), pipipig(`22***13@qq.com`), stubbom(`29***82@qq.com`), tingyichen, xcxmiku, 墨水淘气包(`17***32@qq.com`), etc. (sort by alphabet, are reported in QQ group) @ AOSP v102, AOSP v101, PixelExperience, etc. , 2018-08-25
    * suwakowww @ AOSP v103 @ system-arm64-aonly-vanilla-nosu.img, 2018-08-30
    * markg85 @ AOSP v103 @ , [#168](https://github.com/phhusson/treble_experimentations/issues/168), [#169](https://github.com/phhusson/treble_experimentations/issues/169)
    * suwakowww @ AOSP v104 @ system-arm64-aonly-vanilla-su.img, 2018-09-05
    * suwakowww @ AOSP v105 @ system-arm64-aonly-gapps-su.img, 2018-09-19
    * suwakowww @ AOSP v106 @ system-arm64-aonly-gapps-su.img, 2018-10-03
    * markg85 @ AOSP v106, AOSP v107 @ unknown, 2018-11-10, 2018-11-09
    * suwakowww @ AOSP v107 @ system-arm64-aonly-gapps-su.img, 2018-11-10
    * suwakowww @ AOSP v108 @ system-arm64-aonly-gapps-su.img, 2018-12-06
    * suwakowww @ AOSP v109 @ system-arm64-aonly-gapps-su.img, 2019-01-15
    * suwakowww @ AOSP v111 @ system-arm64-aonly-gapps-su.img, 2019-03-10
    * sxrhd @AOSP v111 @ unknown, 2019-03-29
* AOSP 10.0
    * suwakowww @ AOSP v204 @ system-quack-arm64-aonly-gapps.img, 2019-11-13

Template: @zguithues, @hackintosh5, @suwakowww

Chinese version: @marikid, @suwakowww