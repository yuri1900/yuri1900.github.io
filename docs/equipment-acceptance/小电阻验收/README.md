***\*小电阻模式\****要考虑各个相关联的逻辑：

接地变（跳闸矩阵、硬压板、接入电缆）、

10kV分段保护（接入电缆、接入端子）

10kV备自投（增加电出口插件、定值控制字、硬压板、接入电缆）

主变保护（虚端子、跳闸矩阵）、

主变低压侧合智单元（虚端子、硬压板、接入点）、

主变本体LCP柜（硬压板、接入电缆）的配置。

 

接地变用接地变柜本体LH，不使用接地变开关柜零序CT

10kV零序电流在后台应显示外接零序CT电流，不使用自产零序电流

### **（1）**

最近不到一年时间，西安供电公司开始推广小电阻模式，之前新投变电站设计之初，二次设计部分都未考虑到这种方式。所以验收时先确认是否小电阻系统，二次设计是否考虑，保护装置是否满足要求。

### **（2）**

依据《国网陕西省电力公司文件 ***\*陕电运检〔2019〕 9 号\**** 文：国网陕西省电力公司关于印发 10kV 系统中性点接地方式选用技术原则（试行）等两项工作指导意见的通知》中的

**4 运行原则**

4.1 **低电阻接地系统必须且只能有一个中性点接地运行，当接地变压器或中性点电阻失去时，主变压器的同级断路器必须同时打开。**

4.2正常运行情况下，低电阻接地系统的主变压器低压侧应分列运行，**不允许几个低电阻接地系统并列运行**，以免接地电流过大，引起设备损坏及保护失去选择性。

4.3当一台主变压器带多段母线并列运行时，应将**主变压器所在母线上的接地变压器保持运行**，其余母线上接地变应退出运行。

4.4接地变所提供的接地点是构成零序保护所必须的，因此在运行操作过程中**应始终保证有接地点存在。**

4.5接地变接于主变压器相应引线时，与主变压器同时投入或退出运行，不应兼做站用变功能。

**5继电保护配置基本原则**

5.3**当接地变接于变电站10kV母线时，主变压器的差动保护以及未闭锁10kV备自投的其他保护动作宜联跳接地变支路。**（反过来说主变低后备保护不用联跳接地变）

### **（3）**

依据《国网陕西省电力公司文件**陕电设备〔2021〕63号**国网陕西省电力公司关于印发10kV系统低电阻接地方式改造综合治理方案的通知》中

**一、主网侧设备改造**

1.**在运35-110kV变电站，单相接地故障电容电流大于150A，且电缆化率高于90%的变电站10kV系统，采用中性点经低电阻接地方式。**当电容电流小于150A，但10kV电缆采用共沟槽、共隧道敷设方式的配电系统，长远考虑，采用中性点经低电阻接地方式；当10kV电缆与110kV及以上电压等级电缆线路采用共沟槽、共隧道敷设方式时，则必须采用中性点经低电阻接地方式。

2.新建110kV变电站，中、远期规划满足采用中性点经低电阻接地方式条件时，按照110kV新建变电站通用设计110-A2-3、110-A2-6陕西实施方案，采用10kV系统中性点经低电阻接地方式建设。新建35kV变电站参照执行。

3.在运变电站，由于10kV间隔数量局限，低电阻改造时，采用低电阻设备替换原消弧线圈设备，原有的接地变保持不变，采用接地变接于10kV母线方式，不采用接地变接于主变低压引线方式，同时接地变应兼做站用变使用。**新建变电站，10kV接地变和站用变应分别独立设置。**

4.**新改扩建采用低电阻接地方式的变电站选择，应统筹规划，按照成规模的目标，尽可能选取同一区域的变电站一并改变接地方式，避免一站改变接地方式时，周围变电站全是消弧线圈接地方式的现象。采用低电阻接地方式时，10kV所有保护应配置零序保护功能。**

**四、保护配置要求**

1.接地变保护配置

（1）**接地变间隔配置两段式相间过流保护，配置一段定时限零序过流保护**，零序电流定值整定为75-90A（一次值），**1时限整定为1.5s，跳本侧相邻分段并闭锁本侧相邻分段自投；2时限整定为1.8s，跳接地变和主变压器同侧断路器。**（这个文件说明有些含糊，未明确说明接地变相间过流保护联跳行为，容易误认为和零序电流逻辑一样，实际整定计算整定时相间过流I、II段保护都只跳接地变和本侧主变低压侧断路器。）

（2）**主变保护动作后应联跳接地变开关**；当改造困难时可暂不配置主变保护联跳接地变功能，由监控专业进行人工操作，后续进行主变保护改造时需完善主变保护联跳接地变功能。

（3）**10kV备自投应完善联跳接地变功能，备自投跳开主变低压侧开关同时应跳开该段母线接地变开关**；当改造困难时可暂由监控专业进行人工操作，全站综自改造时完善功能。

### **（4）**

**以柳莺变（原灞桥科技园变）为例**，说明小电阻功能实现的完善过程：

1、设计之初，二次设计未考虑到新增的小电阻模式，未进行二次设计，现场确定为小电阻模式后，与设计沟通变更设计。

2、起初依据**陕电设备〔2021〕63号文变更设计时，未拿到整定计算接地变的调试定值，陕电设备〔2021〕63**号文未明确说明接地变相间过流保护联跳行为，容易误认为和零序电流逻辑一样，**I段跳本侧相邻分段并闭锁本侧相邻分段自投；II段跳接地变和主变压器同侧断路器。**

实际整定计算整定时相间过流I、II段保护都只跳接地变和本侧主变低压侧断路器。

接地变本身有四个跳闸出口，起初为了节省跳闸出口，出口1给了本间隔，出口2跳分段，出口3本侧主变低压开关，增加了2个跳分段、跳主变低压开关的压板，并在接地变跳闸矩阵设置相应保护的跳闸出口；想着电缆接到主变低压开关手跳回路，自然就闭锁了10kV自投，后来拿到接地变定值，才发现接地变相间过流保护不闭锁备自投，只能将接地变出口4分配给闭锁备自投并增加压板和电缆，10kV备自投处并接到闭锁备自投开入，主变低压开关侧改接到非电量跳闸入口。

（要考虑的是10kV假如有三段母线，接地变只有4个跳闸出口，怎么实现II母的接地变保护联切2个分段开关和闭锁2个备自投）

3、主变保护动作后应联跳接地变开关，因为当时没有拿到陕电运检〔2019〕9号文，只依据陕电设备〔2021〕63号文，想到的是只要主变保护只要跳开低压侧开关的同时就联跳本段母线上的接地变开关，首先考虑主变低压侧合智单元只要接到主变保护的跳闸令，要是有跳闸备用出口，再经过增加跳闸压板可直接提供给接地变电缆接线跳闸用，拉接到接地变不用的超温跳闸接入点。结果思源弘瑞的合智单元没有直接的跳闸备用出口，只有一个备用开出1”，接着就考虑主变保护跳低压一分支”的虚端子可以一对多，同时提供给主变低压侧合智单元的“保护永跳1”和“备用开出1”的接收点，这样主变保护的跳闸矩阵不用额外设置，可因为思源弘瑞的合智单元功能受限，不能实现同一装置一对多；

后来只能将主变保护里的“跳闸备用1”拉到主变低压侧合智单元“备用开出1”，同时在主变保护的跳闸矩阵的相应保护里都要增加“跳闸备用1”。注意A、B套主变保护，和主变低压侧A、B套合智单元都要配置。

**主变差动保护、高后备保护联跳接地变，低后备保护不联跳接地变。**

原本本体保护联跳接地变在主变本体LCP柜处，电缆接线到主变本体备用跳闸出口即可，注意备用跳闸出口压板的投入，拉接到接地变不用的超温跳闸接入点。当前因为非电量保护变压器本体故障，所以取消非电量动作联切接地变，利用备自投动作逻辑。

同时，非电量跳开主变两侧，备自投合211，联切接地变。

4、10kV备自投应完善联跳接地变功能，备自投跳开主变低压侧开关同时应跳开该段母线接地变开关。

柳莺变10kV备自投新增加了一块开出插件，并增加配线和联切1#接地变、2#接地变，电缆拉接到接地变不用的超温跳闸接入点。

>需要注意在备自投保护定值的控制字里要投入“联切功能”。备自投跳1号主变低压侧合母联联切1#接地变，备自投跳2号主变低压侧合母联联切2#接地变。

接地变规程要求

1. 接地变零序过流I段I时限：1.5s跳10kV分段（母联）开关，并且闭锁备自投；

II时限 1.8s跳接地变开关和主变低压侧开关

2. 主变差动保护动作跳10kV低压侧开关，同时联跳接地变

10kV 备自投跳主变低压侧开关，同时联接地变

3. 接地变（相间）过流保护跳接地变及主变低压侧开关，且不闭锁10kV备自投

长征变情况：由于10kV主变低压侧合智一体A套只有一个备用开出接点，因此无法同时实现上述2中的情况。

因此：10kV 备自投跳主变低压侧开关联跳接地变是通过10kV主变低压侧合智一体A套。A套收到GOOSE跳闸令后，通过直跳(BIO)模件的备用开出（该开出接点对应装置上的15,16两个端子）联切接地变。

具体通过10kV备自投的联切功能，联切I母跳闸矩阵中的“跳闸出口1”来联切1号接地变；联切II母跳闸矩阵中的“跳闸出口2”来联切2号接地变，将上述GOOSE跳闸令发给主变低压侧合智一体A。

主变差动保护是通过主保护的跳闸矩阵，通过将“跳闸备用1”软压板投入，将联切接地变的GOOSE信号发送给10kV主变低压侧合智一体B套。直跳(BIO)模件的备用开出（该开出接点对应装置上的15,16两个端子）联切接地变。

最后将上述两个15,16分别在对应的101,102开关柜内的端子排短接，再通过接地变柜门上的“联切接地变”硬压板，接入接地变保护装置的备用开入端子。