### ROOT与TWRP使用须知

注：必须适配机型包，不然变砖；提前传输资源文件

#### TWRP使用

**TWRP=REC 进入方法（高通机）**：三个键，同时按住；出现360logo后，松关机键；其它键，保持按住，直到进入twrp，松开全部按键

TWRP视频操作: https://www.bilibili.com/video/BV1dgcUeWEN1/

**TWRP设置中文语言、刷机**：

<img src="https://360rom.github.io/doc/pic/twrp设置和刷包.png" class="center-image">

 1. TWRP刷包（第一次、或更换系统，务必双清）
 2. 部分TWRP，自带推荐安装组件，一般均不选
 3. 部分TWRP，自带功能简单，可刷写匹配的TWRP文件升级
 4. 刷写TWRP后，务必装载，最高安卓版本的纯净系统，优化使用体验
 5. 部分因乱按，TWRP 显示为系统根目录，非存储文件夹；可尝试切换到 sdcard 开头的目录，找传输的文件

#### Magisk须知

1. 部分功能，须上网环境支持
2. Riru和zygisk(magisk)不能同时启用，只能2选一
3. Supersu程序、Magisk框架冲突；两者只能，安装选其一
4. 面具版本V23~20以下，支持搜索模块仓库；高版本面具，移除了该功能 
5. 错误的刷写/安装组件，会导致手机不开机/卡Logo等现象（部分因刷模块，假死机，可刷写卸载模块恢复）
6. 在Magisk V22后,zip包与apk包,合二为一；安装的Magisk App本体,自带了刷写功能;更改文件扩展名( .apk →.zip)获得Magisk刷写zip文件；将文件重命名为uninstall.zip，即Magisk卸载zip文件
7. Magisk V22 是，最后一个支持 Jellybean 和 Kitkat 的主要版本

#### Xposed须知

如装载XP框架重启，出现异常，卡第一屏，开机时多次点按电源键。长震动后，就可停用框架正常开机

1. 任意XP卸载版，即可卸载XP
2. XP版本请与安卓版本，刷写一致
3. XP最高支持，安卓8.X版，且不在维护更新
 
| 安卓版本 | 8.X | 8 | 7.X | 7 | 6 |
| -- | ---- | --- | ------ | -- | ---- | 
| SDK代码 | 27 | 26 | 25 | 24 | 23 |

#### Magisk和Xposed刷写

 Magisk/Xposed离线下载：https://wwr.lanzouw.com/iOIFf2kvksda

提示：Magisk，为当前主流ROOT方式

<img src="https://360rom.github.io/doc/pic/twrp-magisk.png" class="center-image">


#### EdXposed和LSPosed刷写

1. 两者均支持：框架、模块功能与使用
2. 组件/模块/框架，以稳定兼容为基础，过高/低，导致不兼容
2. 部分模块、组件环境，不支持共存或同时启用，需关闭其一
3. . LSPosed和EdXposed，最低支持：安卓8.x 错误的刷写/安装组件，会导致手机不开机/卡 Logo 等现象
4. LSPosed，基于 EdXposed 开发的新框架，有更高的使用与精炼性，且自带模块仓库，支持非全局，特定的 APP 服务支持
5. EdXposed 依赖于（安装顺序）Riru-core、Riru-EdXposed；同需选择兼容系统版本；其次，在安装 EdXposed 管理器 APP
6. EdXposed 存 sandhook 和 yahfa 版；依喜好选择即（V0.4.6.0_beta 版本适合安卓 10.0 版本以上
7. EdXposed 管理器，管理 xposed 插件的开启和关闭；依使用的 EdXposed 发行日期，选择接近时间版本即可
8. 受 Magisk 版本不同，安装方式略有变化；如 Magisk 支持模块仓库，则搜索安装，反之，需要下载并选择安装
 
 ##### EdXposed安装
 
**方法一**：Magisk支持 在线仓库

1. 打开 Magisk 在线仓库，通过搜索关键词：riru、edxpoded 并安装
  
 <img src="https://360rom.github.io/doc/pic/magisk-edxposed.png" class="center-image">
 
2. 官网下载安装 edxposed 管理器即可（首次安装，不生效，需重启解决）

**方法二**：Magisk不支持 在线仓库

1. 下载 EdXposed 依赖组件；通过 Magisk 本地模块安装

  <img src="https://360rom.github.io/doc/pic/magisk-本地安装.png" class="center-image">
  
2. 选择下载的 Riru-core、Riru-EdXposed；按安装顺序安装/重启
 
  <img src="https://360rom.github.io/doc/pic/magisk-模块安装.png" class="center-image">
  
3. 安装 EdXposed 管理器 APP；重启手机，即可激活使用
  
----------

 ##### LSPXposed安装

* 面具版本≥24 先启用 zygisk 在下载 lsp 安装带有 zygisk 的文件
* 面具版本<24 升级面具或下载 Riru 模块 在下载 Riru LSPosed 文件

**方法一**：支持在线仓库

1. 通过 Magisk 在线仓库，搜索关键词，下载 Riru 模块，在下载 Riru LSPosed文件；安装、重启即可

**方法二**：不支持在线仓库

1. Magisk 设置里，打开 aygisk 功能选项（设置完成后，需重启）

      <img src="https://360rom.github.io/doc/pic/magisk-.png" class="center-image">
	  
 <img src="https://360rom.github.io/doc/pic/magisk-zygisk.png" class="center-image">
 
2. 下载&放置存储 LSP 支持的组件；通过 Magisk 本地模块安装

    <img src="https://360rom.github.io/doc/pic/magisk-本地安装.png" class="center-image">
	
3. 安装 LSP 管理器 APP（可选），重启手机，即可激活

    <img src="https://360rom.github.io/doc/pic/LSPosed.png" class="center-image">
	  
**报错和排查原因**

问： LSP 组件默认安装后，桌面无 APP 图标？
* 拨号盘输入*#*#5776733#*#*，可打开应用程序
* LSP 模块压缩包解压，有安装 lsp 管理器 APP，可进行本地式安装使用
  
#### ROOT套件官方下载地址

**注**：如官方弃置或其它，这里不再更新

* Magisk：
https://github.com/topjohnwu/Magisk/releases
* Lsp：
https://github.com/LSPosed/LSPosed/releases
* Riru-core：
https://github.com/RikkaApps/Riru/releases
* EdXposed：
https://github.com/ElderDrivers/EdXposed/releases/
* EdXposed管理器：
https://github.com/ElderDrivers/EdXposedManager/releases
* 合集离线下载：