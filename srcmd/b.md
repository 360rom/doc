### 驱动安装

 1. 驱动不支持“服务器·”系统
 2. 如重装，软件会弹出卸载环节
 3. 安装过程，输入框内容，随意填写即可
 4. 电脑，设备管理器，查看对应端口；部分驱动，安装后，可能需自行添加（如添加后，仍不支持，即为，不兼容或不适用）

#### 360手机驱动(高通芯)

官方360手机驱动(高通机通用)：[下载](https://wwr.lanzouw.com/iKoFJ2fdc2id)

视频安装教程：

**360手机驱动安装教程**

 1. 双击程序，执行安装，一路next、install、 finish默认

<img src="https://360rom.github.io/doc/pic/360手机驱动.png" class="center-image">

#### 9008高通驱动  

 1. 双击程序，执行安装，一路next、install、 finish默认
  
<img src="https://360rom.github.io/doc/pic/9008驱动.png" class="center-image">

#### MTK端口驱动


##### 禁用驱动程序强制签名

注：仅适用于MTK端口驱动；一般大于win7系统，需电脑配置禁用

1. Win+R打开运行窗口，输入：gpedit.msc
2. 用户配置->管理模版->系统->驱动程序安装

<img src="https://360rom.github.io/doc/pic/禁用驱动程序强制签名-1.png" class="center-image">

3. 双击“设备驱动程序的代码签名”，选择“已启用”，选择“忽略”，确定

<img src="https://360rom.github.io/doc/pic/禁用驱动程序强制签名-2.png" class="center-image">

### 刷机解锁
**注**：云锁机，需特殊处理
  <img src="https://360rom.github.io/doc/pic/防盗锁.png" class="center-image">

#### Fastboot刷机模式(常用)

**总结（高通）**：手机关机，长按音量上键不放，数据线连接电脑和手机，再次按音量上键确认即可

视频操作：https://www.bilibili.com/video/BV1RgcUeWE5f/

1. 手机彻底关机
2. 数据线USB一头，先插入电脑（台式插入机箱后）
3. 另一只手，按住手机音量上键不放，然后将数据线手机口
4. 手机出现提示界面后，再次按音量上键确认；到此即成功进入
   
  <img src="https://360rom.github.io/doc/pic/fastboot.png" class="center-image">
  
  <img src="https://360rom.github.io/doc/pic/电脑fastboot.jpg" class="center-image">
  
 视频教程：https://www.bilibili.com/video/BV1314y1F714/
* 部分假死机，可通过此方法，快速判断电脑：兼容性、硬件、系统问题
* <font color='red'>有锁机、忘记密码等；要长按关机键，关机，然后，快速按住音量上键，连接电脑和数据线</font>

#### ☇Fastboot异常解决

多数因USB端口、电脑兼容性问题所致；使用拓展坞，连接变更USB环境，可解决多数存在问题

**异常表现：**

 1. 掉驱动
 2. 手机左上角，出现白色英文字体
 3. 电脑弹出，英文报错，端口异常等提示
   
**解决方案：**

  <img src="https://360rom.github.io/doc/pic/刷机端口异常解决.png" class="center-image">


#### OTA本地卡刷
 
 1. 打开手机 设置-系统更新（N5/6/7代 按钮位置或不同）
2. 击右上角 ⋮  选择 本地更新
3. 找到传输的刷机包，选择并同意授权，等待刷写（需资源匹配）

 <img src="https://360rom.github.io/doc/pic/ota升级.png" class="center-image">
 
### USB模式

USB操作，需对应的驱动支持，请提前电脑安装

#### USB开发者模式

视频操作：https://www.bilibili.com/video/BV1RgcUeWEbN/

 1. 打开手机 设置-系统-关于手机
 2. 滑找到 版本号 并连续点击7下
 3. 退出并找 开发者选项（注：N5 代或其它，还需返回设置，在查找） 
 4. 往下滑 找到打开 USB调试

 <img src="https://360rom.github.io/doc/pic/开发者模式.png" class="center-image">
 
#### USB调试文件传输

 1. 打开“开发者选项”并启用USB调试
 2. 数据线连接手机和电脑；看手机提示 切换USB为 文件传输模式
 3. 注意观察手机，提示授权，全部同意

 <img src="https://360rom.github.io/doc/pic/USB文件传输.png" class="center-image">


#### USB测试模式

* 亦称9001模式；仅特殊情况使用，如刷写通信基带
* 密码：当前日期+IMEI后四位

 视频教程：
 
 1. 拨号盘输入：*20121220#  进入工程模式
 2. 选择"通信类设置"-“其他信息-“USB切换”-切换到测试场景
 3. 打开开发者模式，并启用USB调试
 3. 数据线连接手机和电脑，下拉通知或依提示，勾选：测试模式

 <img src="https://360rom.github.io/doc/pic/USB测试模式.png" class="center-image">
 
#### 工程模式类

手机拨号盘输入，非必情况，不需要

* *#06# 查看IMEI串码  
*  <p>*#9527*#测验模式</p>
* *20121220# 工程模式
