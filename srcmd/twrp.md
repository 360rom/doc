温馨提示：提前装载360机型驱动；资源文件，可联系获取；部分机型综合性能老旧，暂不提供


### N4S-MTK ROOT

 <h3 align='center'> 360N4S-MTK ROOT TWRP教程</h3>
 
----------

### N4S骁龙版 ROOT

 <h3 align='center'> 360N4S骁龙版 ROOT TWRP教程</h3>

 1. 卡刷降级系统版本为V042以下
 2. 电脑安装360手机驱动、高通9008驱动、QPST
 3. 解压360N4S骁龙版，Twrp文件
 
  <img src="https://360rom.github.io/doc/pic/n4s骁龙版-twrp文件.png" class="center-image">
  
 4. 手机打开，开发者模式，并启用USB调试和OEM解锁
  
  <img src="https://360rom.github.io/doc/pic/OEM.png" class="center-image">
  
 5. 通过abd或cmd，输入： adb reboot edl 回车，手机会自动关机，呼吸灯闪

  <img src="https://360rom.github.io/doc/pic/adb reboot edl.png" class="center-image"> 
  
 6. 在电脑设备管理器中，查看9008端口
  
   <img src="https://360rom.github.io/doc/pic/9008端口.png" class="center-image"> 
  
 7. 打开QPST附属工具QFIL后，点击“Browse”，加载解压的elf和xml文件，patch不加载

   <img src="https://360rom.github.io/doc/pic/QFIL-N4S骁龙版进度.png" class="center-image"> 
 
提示：QFIL右上角显示9008端口，说明QFIL已识别且上线（如有9008端口，但未自动识别上线，则点击Select Port…选择对应端口；解压TWRP资源，路径与文件夹名，推荐简短，且数字或英文）

8. 留意QFIL的进度条和状态信息，看到蓝色字体 Dowenload Succeed 提示，就代表刷入成功（如失败，长按开机键开机，在重进模式操作·）

  <img src="https://360rom.github.io/doc/pic/n4s骁龙版-twrp.png" class="center-image"> 
  
9. 断开数据线，三键同按；出现360 Logo后松开“电源键”，“音量上+下键”继续按住，直到进入TWRP界面，全部松开；第一次进入twrp，须滑动允许修改
10. 刷写适配，纯净系统即可
----------

### N5 ROOT

 <h3 align='center'> 360N5 ROOT TWRP教程</h3>

1. 系统降刷到安卓版本6，如V092、V111、V116
2. 手机打开，开发者模式，并启用USB调试和OEM解锁

 <img src="https://360rom.github.io/doc/pic/OEM.png" class="center-image">
 
3. 手机进入fastboot模式，插入数据线，连接电脑
    
4. 打开root工具，等待工具自动检测，并按照软件提示操作

 <img src="https://360rom.github.io/doc/pic/n5tool.png" class="center-image">
 
5. 刷写完成后，手机端会自动进入Twrp模式；第一次进入twrp，须滑动允许修改

<img src="https://360rom.github.io/doc/pic/n5-twrp.png" class="center-image">
   
6. 刷写适配，纯净系统即可（该机，首次开机/装系统，开机慢，耐心等待）

----------

### N5S ROOT

 <h3 align='center'> 360N5S ROOT TWRP教程</h3>
 

1. 系统降刷到安卓版本6，如V092、V116
2. 手机打开，开发者模式，并启用USB调试和OEM解锁
 
 <img src="https://360rom.github.io/doc/pic/OEM.png" class="center-image">
 
3. 数据线连接手机和电脑，并留意手机，授权USB设备
4.  通过abd或cmd，输入命令行操作
    
 <img src="https://360rom.github.io/doc/pic/n5s-tool.png" class="center-image">
 
**adb命令行**

> 1.	adb push recovery.img /data/local/tmp/recovery.img   从电脑传送rec文件到手机(adb push命令后的recovery.img文件随文件名而改变)
> 2.	adb shell   进入命令模式
> 3.	su   权限
> 4.	dd if=/data/local/tmp/recovery.img of=/dev/block/bootdevice/by-name/recoveryname/recoveryname/recovery   替换rec
> 5.	exit   退出
> 6.	exit   退出
> 7.	adb reboot recovery   重启到rec

 <img src="https://360rom.github.io/doc/pic/n5s-twrp.png" class="center-image">
 
5. 重启后，即进入TWRP，刷写适配纯净系统即可

**注**： 

1. adb devices 命令，可查看设备是否在线
2. 完成所有adb命令后，如系统，开机和重启几次，为正常现象
3. N5S的root工具，可适用于N5
   
----------

### N6 ROOT

 <h3 align='center'> 360N6 ROOT TWRP教程</h3>

1. 降刷系统版本到V070或以下
2. 电脑安装360手机驱动、高通9008驱动、QPST
3. 手机彻底关机，短接或工程线，进入9008模式

 <img src="https://360rom.github.io/doc/pic/9008端口.png" class="center-image">
 
4. 解压N6的TWRP Recovery文件
5. 打开QPST附属工具QFIL后，点击“Browse”，加载解压的elf和xml文件，patch不加载
   
<img src="https://360rom.github.io/doc/pic/QPST工具QFIL.png" class="center-image">

 <img src="https://360rom.github.io/doc/pic/QFIL-N6.png" class="center-image">
 
提示：QFIL右上角显示9008端口，说明QFIL已识别且上线（如有9008端口，但未自动识别上线，则点击Select Port…选择对应端口；解压TWRP资源，路径与文件夹名，推荐简短，且数字或英文）

6. 留意QFIL的进度条和状态信息，看到蓝色字体 Dowenload Succeed 提示，就代表刷入成功（如失败，长按开机键开机，在重进模式操作·）
   
 <img src="https://360rom.github.io/doc/pic/QFIL-N6进度.png" class="center-image">
 
7. 断开数据线，三键同按；出现360 Logo后松开“电源键”，“音量上+下键”继续按住，直到进入TWRP界面，全部松开；第一次进入twrp，须滑动允许修改
8. 刷写适配，纯净系统即可
----------

### N6Lite ROOT

 <h3 align='center'> 360N6Lite ROOT TWRP教程</h3>
 

1. 系统，线/卡刷，降级到V058
2. 电脑安装360手机驱动、高通9008驱动、QPST
3. 手机完全关机，按住音量下键，数据线连接电脑；并在设备管理器中，查看9008端口(出现端口，即松开按键；如无，则重复此步骤)

<img src="https://360rom.github.io/doc/pic/9008端口.png" class="center-image"> 

4. 解压360 N6Lite的V043刷机包

   <img src="https://360rom.github.io/doc/pic/N6L-V043.png" class="center-image"> 

5. 打开QPST附属工具QFIL后，点击“Browse”，加载解压的elf和xml文件，patch不加载

提示：QFIL右上角显示9008端口，说明QFIL已识别且上线（如有9008端口，但未自动识别上线，则点击Select Port…选择对应端口；解压TWRP资源，路径与文件夹名，推荐简短，且数字或英文）

6. 留意QFIL的进度条和状态信息，看到蓝色字体 Dowenload Succeed 提示，就代表刷入成功（如失败，长按开机键开机，在重进模式操作·）

   <img src="https://360rom.github.io/doc/pic/QFIL-N6L-twrp文件.png" class="center-image"> 

7. 在QFIL刷入V043版本后，手机再次关机；按住音量下键不放，进入9008模式

8. 再次打开QFIL工具，刷入TWRP资源文件

  <img src="https://360rom.github.io/doc/pic/N6l-twrp文件.png" class="center-image"> 
   
9. 断开数据线，三键同按；出现360 Logo后松开“电源键”，“音量上+下键”继续按住，直到进入TWRP界面，全部松开；第一次进入twrp，须滑动允许修改]
 
<img src="https://360rom.github.io/doc/pic/N6L-TWRP.png" class="center-image"> 

10. 刷写适配，纯净系统即可
  
----------

 ### N6Pro ROOT
 
 <h3 align='center'> 360N6RO ROOT TWRP教程</h3>

1. 降刷系统版本到V070或以下
2. 电脑安装360手机驱动、高通9008驱动、QPST
3. 手机彻底关机，短接或工程线，进入9008模式

 <img src="https://360rom.github.io/doc/pic/9008端口.png" class="center-image">
 
4. 解压N6PRO的TWRP Recovery文件
   
 <img src="https://360rom.github.io/doc/pic/N6P-TWRP文件.png" class="center-image">
 
5. 打开QPST附属工具QFIL后，点击“Browse”，加载解压的elf和xml文件，patch不加载
   
 <img src="https://360rom.github.io/doc/pic/QFIL-N6P进度.png" class="center-image">
 
提示：QFIL右上角显示9008端口，说明QFIL已识别且上线（如有9008端口，但未自动识别上线，则点击Select Port…选择对应端口；解压TWRP资源，路径与文件夹名，推荐简短，且数字或英文）

6. 留意QFIL的进度条和状态信息，看到蓝色字体 Dowenload Succeed 提示，就代表刷入成功（如失败，长按开机键开机，在重进模式操作·）
 
7. 断开数据线，三键同按；出现360 Logo后松开“电源键”，“音量上+下键”继续按住，直到进入TWRP界面，全部松开；第一次进入twrp，须滑动允许修改
8. 刷写适配，纯净系统即可
 
----------

 ### N7 ROOT
 <h3 align='center'> 360N7 ROOT TWRP教程</h3>
 
