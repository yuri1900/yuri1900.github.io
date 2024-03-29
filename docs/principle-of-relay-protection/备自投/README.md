### 13.5.1常见备自投方式

1、母联或桥（分段）断路器备自投

2、进线备自投

3、变压器备自投

4、桥接线变压器备自投

5、均衡负荷备自投

6、双母接线备自投

### 13.5.2基本原理

 　备用电源自动投入装置一次接线方式较多，但备自投原理比较简单。下面介绍几种变电站中典型的备自投方式原理。对更复杂的备自投方式，都可以看成是这些典型方式的组合。

 　投入备自投充电过程时：装置上电后，15秒内均满足所有正常运行条件，则备自投充电完毕，备自投功能投入，可以进行启动和动作过程判断；当满足任一退出条件时，备自投立即放电，备自投功能退出。

 　退出备自投充电过程时：装置上电后，满足启动条件后备自投进行动作过程判断。在正常运行条件或退出条件下，备自投可靠不动作。

 

#### （1）分段备自投（10kV）

 

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps121.png)

分段备自投接线示意图

 

a）正常运行条件

1）分段断路器3DL处于分位置，进线断路器1DL、2DL均处于合位置

2）母线均有电压

3）备自投投入开关处于投入位置

 

b）启动条件

1）II段备用I段：I段母线无压，1DL进线1无流，II段母线有压

2）I段备用II段：II段母线无压，2DL进线2无流，I段母线有压

 

c）动作过程

1）对启动条件1：

​    若1DL处于合位置，则经延时跳开1DL，确认跳开后合上3DL

  　 若1DL处于分位置，则经延时合上3DL

2）对启动条件2：

   若2DL处于合位置，则经延时跳开2DL，确认跳开后合上3DL

   若2DL处于分位置，则经延时合上3DL

d）退出条件

 　1）3DL处于合位置

 　2）备自投一次动作完毕

 　3）有备自投闭锁输入信号

4）备自投投入开关处于退出位置

#### （2）进线备自投（110kV）

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps122.png)

进线备自投接线示意图

 

a）正常运行条件

1）进线2备用进线1：1DL、3DL处于合位置，2DL处于分位置，两段母线均有电压，备自投投入开关处于投入位置

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps123.png)

1）进线1备用进线2：2DL、3DL处于合位置，1DL处于分位置，两段母线均有电压，备自投投入开关处于投入位置

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps124.png)

b）启动条件

1）进线2备用进线1：母线无电压，进线1无流，进线2有电压

2）进线1备用进线2：母线无电压，进线2无流，进线1有电压

c）动作过程：

 1）对启动条件1，2DL处于分位时

  　 若1DL处于合位置，则经延时跳开1DL，确认跳开后合上2DL

  　 若1DL处于分位置，则经延时后合上2DL

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps125.png)

 2）对启动条件2，1DL处于分位时

   若2DL处于合位置，则经延时跳开2DL，确认跳开后合上1DL

   若2DL处于分位置，则经延时后合上1DL

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps126.png)

d）退出条件

1）备自投一次动作完毕

2）1DL、2DL均处于合位置

3）有备自投闭锁输入信号

4）备自投投入开关处于退出位置 

#### （3）桥备自投（110kV）

 

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps127.png)

桥备自接线投示意图

 

a）正常运行条件

 　1）桥断路器3DL处于分位置，进线断路器1DL、2DL均处于合位置

 　2）进线1、进线2均有电压

 　3）备自投投入开关处于投入位置

b）启动条件

1）进线2有电压，进线1无电压且无电流

 　2）进线1有电压，进线2无电压且无电流

c）动作过程

1）对启动条件1

若1DL处于合位置，则经过延时跳开1DL，确认跳开后，合上3DL

若1DL处于分位置，则经延时后合上3DL

2）对启动条件2

若2DL处于合位置，则经过延时跳开2DL，确认跳开后，合上3DL

若2DL处于分位置，则经延时后合上3DL

d）退出条件

1）3DL处于合位置

2）备自投一次动作完毕

3）有备自投闭锁输入信号

4）备自投投入开关处于退出位置

#### （4）变压器备自投

![img](file:///C:\Users\15492\AppData\Local\Temp\ksohtml3412\wps128.png)

变压器备自投接线示意图（一台变压器为主变压器，另一台变压器为辅变压器）

 

a） 正常运行条件

 　1）主变压器各侧断路器处于合位置，辅变压器各侧断路器处于分位置

 　2）母线有压，辅变压器进线有压

 　3）备自投投入开关处于投入位置

b）启动条件

 　主变压器无电流，母线无电压，且辅变压器进线有压

c）动作过程

 　当主变压器无电流，母线无电压，且辅变压器进线有压时：

若主变压器二次断路器处于合位置，则经延时跳开主变压器各侧断路器，确认跳开后，依次合上辅变压器各侧断路器

若主变压器二次断路器处于分位置，则经延时依次合上辅变压器一二次断路器

d）退出条件

  1）备自投一次动作完毕

  2）3DL、4DL均处于合位置

  3）有备自投闭锁输入信号

4）备自投投入开关处于退出位置