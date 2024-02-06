| MMS                          | 即制造报文规范，是ISO/IEC9506 标准所定义的一套用于工业控制系统的通信协议。 |                                           |
| ---------------------------- | ------------------------------------------------------------ | ----------------------------------------- |
| GOOSE                        | 是一种面向通用对象的变电站事件。主要用于实现在多IED 之间的信息传递，包括传输跳合闸信号（命令），具有高传输成功概率。 | Generic object oriented substation events |
| SV                           | 采样值。基于发布/订阅机制，交换采样数据集中的采样值的相关模型对象和服务，以及这些模型对象和服务到ISO/IEC8802-3 帧之间的映射。 | Sampled value                             |
| ICD 文件                     | 由装置厂商提供给系统集成厂商，该文件描述IED 提供的基本数据模型及服务，但不包含IED 实例名称和通信参数。 | IED Capability Description                |
| SSD 文件                     | 应全站唯一，该文件描述变电站一次系统结构以及相关联的逻辑节点，最终包含在SCD 文件中。 | System Specification Description          |
| ***\*SCD\**** ***\*文件\**** | 应全站唯一，该文件描述所有IED 的实例配置和通信参数、IED 之间的通信配置以及变电站一次系统结构，由系统集成厂商完成。SCD 文件应包含版本修改信息，明确描述修改时间、修改版本号等内容。 | Substation Configuration Description      |
| ***\*CID\**** ***\*文件\**** | 每个装置有一个，由装置厂商根据SCD 文件中本IED 相关配置生成。 | Configuration IED Description             |
| IED                          | 智能电子设备                                                 | Intelligent Electronic Device             |