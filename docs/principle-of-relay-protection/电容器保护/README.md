### 欠压保护

（1）设置目的

欠压保护主要是为了防止电容器因备自投或重合闸动作，电容器失电后短时间内再次带电时，由于残余电荷的存在对电容器造成冲击损坏。

欠压保护延时应小于备自投或重合闸动作时间。

为了防止TV断线时欠压保护误动，设置有电流判据进行闭锁。

（2）动作条件

1）三个线电压均低于欠压定值

2）三相电流均小于电流闭锁定值

3）线电压从有压到欠压

4）断路器在合位

### 过电压保护

（1）设置目的

过电压保护主要是防止运行电压（稳态过电压）过高造成电容器损坏，根据需要可以选择动作告警还是跳闸。

为了避免10kV（中性点不接地系统）系统发生单相接地造成保护误动，电压判据采用线电压。

中性点不接地电力系统发生单相接地时，虽然各相对地电压发生变化，但各相间电压（线电压）仍然对称平衡

（2）动作条件

1）三个线电压中的任一个电压高于过电压整定值

2）断路器在合位

### 不平衡保护

（1）设置目的

不平衡保护主要用来保护电容器内部故障，单只或者部分电容器故障退出运行，电容器三相参数不平衡造成其余电容器损坏。

可以根据一次设备接线情况选择配置不平衡电压保护和不平衡电流保护

 

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps104.jpg) 

电容器分相差压保护和不平衡电压保护反映的都是单星形接线电容器组中电容量不平衡的保护，主要用于保护电容器内部故障。

当电容器单元里的小元件发生击穿或熔丝熔断后所引起的电压及电流的变化极其微小，虽然不会引起过电压保护和电流保护动作跳闸，但是其余运行元件所承受的电压将加大，特别是遇到电网谐波扰动和异常电压升高将加剧元件故障，随着故障元件被击穿隔离，电容器不平衡逐渐加大，所以需要电容量不平衡保护来跳开断路器，从而达到保护电容器，隔离故障点的作用。

电容器分相差压保护和不平衡电压保护所需的电压均来自电容器本体的放电PT（也称作放电线圈）。

电容器放电PT有两种接线方式：开口不平衡电压接线方式（针对不平衡电压保护）和分相差压接线方式（针对分相差压保护）。

1开口不平衡电压接线方式

不平衡电压保护反映的是电容器组内部的不平衡现象。正常运行时，三相电压平衡，放电PT开口处电压为零，当电容器某相内部元件损坏，将引起电容器组三相电容不平衡，三相电容器的端电压将不再对称，在放电PT的开口处就会出现零序电压。

这是用于开口不平衡电压的电容器及放电PT的一次接线照片：

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps105.png) 

这是电容器装置铭牌上的一次主接线原理图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps106.png) 

这是现场实际一次接线示意图（A1到A4为A相的4只电容器，见一次接线照片，B、C相同理）。

每相PT有2个一次端头——A和X，且A-X间电压反映该相并联电容器组的两端电压。

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps107.png) 

每相PT有2个二次端头——a和x

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps108.png) 

 

这是不平衡电压放电PT的铭牌

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps109.png) 

这是三相PT的一、二次接线示意图（贴在PT上）。

示意图中电压继电器（实际为电容器保护不平衡电压输入端子）感受到的电压为：A、B、C相电压的矢量和，即不平衡电压（零序电压）。

由于A、B、C相电容器组的容量几乎相等，因此正常运行时，不平衡电压为0。

当某电容器故障时，A、B、C相电容器组的容量不等，就会产生不平衡电压。

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps110.png) 

这是A、B、C相PT的现场实际二次接线图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps111.png) 

这是设计图的一二次原理图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps112.png) 

***\*2分相差压接线方式\****

电容器组的分相电压差动保护，简称差压保护。是通过检测同相电容器两串联段之间的电压，并作比较。设备正常时上、下两段电容值相等，两放电线圈一次承受的电压相同，差压为零。当某段出现故障时，上、下段电容值将发生变化，因此就会产生差压。

这是用于分相差压的电容器及放电PT的一次接线照片

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps113.png) 

这是电容器装置铭牌上的一次主接线原理图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps114.png) 

这是现场实际一次接线示意图（A1到A6为A相的6只电容器，见一次接线照片）。

每相PT有3个一次端头——A1、A2、X。

可见，一次端头A2为公共端头，PT一次端头A1-A2间电压反映电容器A4、A5、A6两端电压；PT一次端头A2-X间电压反映电容器A1、A2、A3两端电压。

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps115.png) 

 

每相PT有4个二次端头——a1、a2、x1、x2

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps116.png) 

这是分相差压放电PT的铭牌，标注了每组一次端头和二次端头的额定电压，可以看出一次端头A2为公共端头。

一次端头A1-A2额定电压为11/2/√3 kV；

对应的二次端头a1-x1额定电压为100V；

一次端头A2-X额定电压为11/2/√3 kV；

对应的二次端头a2-x2额定电压为100V。

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps117.png) 

这是每相PT的一、二次接线示意图（贴在PT上）。

可以看出一次端头A1-A2对应二次端头a1-x1，一次端头A2-X对应二次端头a2-x2。

示意图中电压继电器（实际为电容器保护某相差压输入端子）感受到的电压为：二次a1-x1间电压与二次a2-x2间电压的矢量差，即差压。

由于电容器A1、A2、A3的总容量与电容器A4、A5、A6的总容量几乎相等，因此正常运行时，一次端头A1-A2间电压与A2-X间电压幅值相位相等，对应的二次a1-x1间电压与二次a2-x2间电压也幅值相位相等，此时差压为0。

当某电容器（如电容器A6）故障时，串联的两组电容器的容量不等，两端电压也不等，A相就会产生差压。

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps118.png) 

这是A、B、C相PT的现场实际二次接线图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps119.png) 

 

这是设计图的一二次原理图

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps120.png) 