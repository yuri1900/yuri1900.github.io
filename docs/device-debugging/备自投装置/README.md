### 调试方法

#### 10kV备自投

试验10kV备自投，看说明书采常开还是常闭

3501，3502开关位置接到模拟断路器跳闸（常闭）辅助接点，

备自投方式一，先合模拟断路器（100），然后拉I母电压空开，3501跳闸，100合闸。

 

#### 110kV备自投

##### 进线备自投

进线备自投的跳闸回路一般可通过保护跳闸或手跳两种方式实现，但两种方式都有各自需要注意的问题。

（1）采用保护跳闸方式在设计中必须要考虑闭锁重合闸问题，因为采用保护跳开工作线路开关后，保护装置会误认为开关偷跳而启动重合闸将原已被分开的线路开关又重新合上，导致无法隔离有故障的原工作线路，备自投也因此无法正常工作，因此必须用另一副跳闸输出接点去闭锁该线路保护的重合闸。

（2）采用手跳方式就可以不用再考虑闭锁重合闸的问题，因为手动跳闸、遥控跳闸的操作回路已经考虑闭锁重合闸了。在人为手分工作线路开关时，为了避免备自投合备用线路开关，往往接入保护合后继电器接点，并加入“手分闭锁备自投”回路，但这将会造成备自投通过手跳回路跳开工作线路后，“手分闭锁备自投”回路又闭锁备自投，导致无法合备用线路。因此可取消保护合后继电器接点接入备自投装置，以便备自投装置能正确动作。为了防止人为手分工作线路开关时备自投误投备用线路，应在备自投的现场运行规程里要求再人工断开工作线路开关前将备自投退出。

对于对侧设重合闸的系统，备自投可等待对侧重合一次失败后启动自投，也可直接自投。重合失败后自投对恢复供电较有利，但自投延时将延长一个重合动作周期。原则上对供电容量大、装置可靠性较高、供电线路较长、重合成功率低或对连续性供电有特殊要求的重要负荷可采用直接自投方式；对装置可靠性相对较低的常规继电器备自投的负荷可采用先重合后自投方式。

###### 方式一

 

###### 方式二

母联合位，进线1分位，进线2合位，合上YH刀闸

备自投的电压采的是保护第1组电压，

在I母YH柜，模拟I II母线失压，进线1有压，备自投动作。

 

##### 分段备自投

###### 方式三

###### 方式四

#### 110kV链式备自投

### 故障排查



10kV分段备自投跳主变低压侧开关，错误的接到手跳，会报开关偷跳

 

事故原因：分段备自投跳主变低压侧开关103接到了手跳回路（手跳与保护跳闸端子太近）上（正常应接保护跳闸），当拉开103开关，4s后分段备自投动作手跳103，同时手跳103闭锁了备自投装置，0.3s后备自投无法合上312开关。

 

312跳102的正电有时才有75V，负电140V，过一会恢复，说是直流巡检仪的问题