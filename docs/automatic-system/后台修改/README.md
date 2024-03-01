### **PCS-9700（南瑞继保）**

电脑登录  用户名：ems   密码：123456、Nems-9700  登录“NR“软件，选择0分钟   用户名：rcs-super  mm：1/空 

改名：开始→维护程序→数据库组态→点：“解锁图“→登录→改名→整体统一保存→该遥测系数为变比电流一次值→eq：400/5的系数为400→改遥控编号→“一次设备配置“是与主接线图各图元关联的，改完后→点击发布按钮→左键将“发布至物理“→先改主接线图→改分图时点“操作“→刷新OIO→全选→左键字符替换→改完后先保存再发布（为了删除旧图保存新图草稿）


### **CSC2000（四方）**

按“左下角“→运行→C：\CSC2000\BIN\WizTool.ese→用户：Z   密码：Z→间隔管理→间隔列表→找对应间隔→把名字一改→“间隔别名是地址“→改后关掉→遥测可以改→系统→实施序输出→Yes→输出（不要点别的）

备份：我的电脑→C盘→CSC2000→全选（除了：AHDB/Event/hisdata/HISDB四个不选）→复制：在别的盘粘贴→“WizApp“后台开始。

### **CSC2000V2**

修改后需要重启后台才能改过名字

 

### **CSGC3000SA** 

后台用户修改间隔名称步骤

更改前工程备份

1、修改之前首先做一个修改之前的备份，linux 系统下桌面主文件夹/csgc3000sa/usr /工程文件夹，最后修改完后同样拷贝这个文件夹里的工程做备份。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps276.jpg) 

 

2、Linux 系统备份，拷贝 csgc3000sa/usr 里面的工程比如puxinbian可以点击右键压缩/压缩到，名字自己命名，一般在后面加上日期方便查找，比如 puxibian20220629

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps277.jpg) 

 

 

 

运行界面下进入编辑

 

运行界面下找到四方小图标右键，选择“配置工具”，选择最下面的建模组态，用户名、密码均为admin

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps278.jpg) 

修改间隔名称

1、点击模型数据管理，见下图，双击“公司：电网公司”

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps279.png) 

2、找到需要修改间隔名称的间隔，右键，更改别名进行修改。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps280.png) 

3、见下图，然后点左上角保存。

 

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps281.png) 

修改遥测变比（如不涉及更改可以忽略）

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps282.png) 

1、单击右上角模型数据库，单击 SCADA 库，实时监视与统计，修改变比，单击遥测，找到相应间隔。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps283.png) 



2、找到系数一列，找到电流，修改变比，比如变比如果是 400/5就填 80，同时需要修改有功和无功的系数，有功和无功系数是，电压系数×电流系数/1000，（注意，一般电流单位为安 A，电压为千伏 kV，有功为兆瓦 MW，无功为兆乏 MVar）。更改完毕后点保存表数据。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps284.png) 

3、然后左上角点击保存所有，确定

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps285.png) 

 

 

 

 

 

 

 

 

 

 

 

 

修改遥信描述（如不涉及更改可以忽略）

点击遥信选择相应间隔，修改别名，然后点击保存数据表，然后同遥测保存步骤，左上角保存，确定，然后左上角保存所有，确定。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps286.png) 

修改遥控编号（如不涉及更改可以忽略）

点击遥控选择相应间隔，修改别名，然后点击保存数据表，然后同遥测保存步骤，左上角保存，确定，然后左上角保存所有，确定。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps287.png) 

修改图形

1、点击图形组态工具，双击主接线图或启动画面找到主接线图

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps288.png) 

2、上面有一个小手实时平移图标单击可以拖动图形。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps289.png) 

3、找到相应设备停止，右键左键单击相应设备，比如漳容 1，修改名称和别名（注意名称和别名要一样），确定，修改完毕后，左上角点击保存所有。

 

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps290.png)![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps291.png) 

4、同样，打开分图，对分图进行修改，修改完毕后，左上角点击保存，保存所有。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps292.png) 

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps293.png) 

5、打开全站通讯图，双击需要修改名字的间隔，对间隔名进行修改，修改完毕后，左上角点击保存，保存所有。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps294.png) 

6、全部修改完后，单击保存，确定，保存所有，确定。

![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps295.png) 

同步到其它监控主机

点击工程文件发布，弹出画面勾选config、gragh。勾选所有主机名称scada*。点击“连接”，连接状态显示“已经连接”，点击“开始传输”。![img](file:///C:\Users\yuri\AppData\Local\Temp\ksohtml22920\wps296.jpg)

同步到其它监控主机

右上角点击×，提示保存所有数据及信息打√ ，确定。

 

### **四方csc3000**

改后台（补充版）：右键点四方图标，选配置工具，然后建模组态，模型数据管理，找到对应的间隔改名称保存；右键点四方图标，选配置工具，然后建模组态，选图形组态管理，找到小电流接地选线，通道状态，低频低压减载，主接线（或者启动画面）打开找到相应间隔，改名称；主界面图：在图形名称点开主接线图，找到要改的间隔名称，分画面图：在图形名称找到要改的间隔，点进去改名称（不需要改图形名称）然后保存；直流消失互报改法：在建模组态第一行点开模型数据库点进去，打开SCADA库，打开实时监视与统计，打开遥信，找出相邻间隔直流消失，改名称！点击校验及同步，点击工程文件发布，选择graph文件打勾，然后点击连接，点击开始传输！如果另一台后台机名称没有更新，在另一台后台机点击进入任意一个间隔的分画面！如果报文出线（杏五线-备用线）名称未改过来的，打开二次装置库，打开智能装置，找到相应的间隔改名称！然后再退出主画面就更新完毕。

### **PRS7000（长园深瑞）**

打开后台“rtdb“→终端→长园深圳南瑞PRS7000   SCADA   自动化

在终端输入→cfgtool回车→用户：a   密码：a→厂站配置→间隔配置→修改后保存→图形组态里修改→主接线图；画面索引；间隔图；注：数据连接和按钮参数全要改

Beifen ：dbManager   dbManager   127.0.0.1左键打开→nari

 

### **NS2000（南瑞科技）**

进入系统组态→设备组态（修改名称）保存→再单间隔内修改→设备类（开关、刀闸、线路、其他）手动修改并保存→遥信表→选中第一列→名称设置（生成四遥）保存→工具里有：系统重要参数确认→逻辑节点类修改→小电流修改
