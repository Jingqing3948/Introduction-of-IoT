# GPS
## What is GPS?(3 major segments)
The Global positioning system (GPS) is a space-based satellite navigation system that provides location and time information, where there is an **unobstructed line of sight** to 4 or more GPS satellites.

components : 
- Space segment: hardware in orbit around the earth, 
- Control segment: a system of ground stations,
- User segment: handheld receivers
## Basic Steps
- Positioning
- Timing
- SV Ranging
- Trilateration
- Correction of errors
## **Two basic steps of localization technologies**
1) Measuring
2) Calculation

## How GPS works?
- Range from each satellite calculated
  
	range = time delay * speed of light

	Determining Range: Receiver and satellite use same code, compare incoming code with receiver generated code.
- Trilateration is used to determine you position or "fix"
- At least 3 satellites required for 2D fix. However, 4 satellites should always be used (receiver clock error)(**SVs have highly accurate atomic clocks!**)
## Disadvantages of GPS 
- Not apply for indoor environments.
- The largest problem is **multi-path effect!**
## ERROR
- **(Most): due to the atmosphere**
- **Satellite clock errors** 
- SV position errors
- Quality of GPS receiver
- **Multi-path errors**

## Multi-path
Multi-path occurs when **signals are reflected off of objects** such as trees or buildings.


## Other positioning technologies
- cellular based
- WiFi positioning
- Bluetooth positioning
- RFID chips embedded in the environment

## Three typical methods of localization
- ToA: Time of Arrival
- TDoA: Time difference of Arrival
	(The biggest advantage is that it **doesn’t need time synchronization.**)
- signal feature based localization
	(Not rely on special hardwares, but **leverage the signal feature directly 直接利用信号特性**)

*随着人类对外部世界的改造，对未知领域与空间的拓展，人类需要的信息来源、种类、数量、精度不断增加，对信息获取的手段也提出了更高的要求。传感器因此而生。在现实生活中，传感器无处不在。*

# Sensor:
A sensor is a converter **that measures physical quantity** and converts it into a signal.

由敏感元件和转换元件和测量电路（有时还会加上辅助电源）组成，能感受到并被测量，并能将检测和感受到的信息按一定规律转化为电信号并输出。

别名：transducer, probe, gauge, detector

stimulus = physical quantity = measurand 
## Types
- Active Sensor: generate electric current
- Passive sensor: require additional electrical energy.
- contact sensor: a sensor that requires **physical** contact **with the stimulus**. 
- non-contact sensor: require no physical contact. 

*智能传感器有一定的信息处理能力（含有微处理器）。*

## 传感器的常用参数
- Input : stimulus or measurand 
- output: electrical signal
- Transfer Function:
Relation between input and output
## Range, span, IFS, OFS of sensors 
- Range：lowest and highest values of the stimulus (两个值）
- Span: the **arithmetic** differences （上⾯两个值的差）between the highest and lowest values of the stimulus (that can be sensed within acceptable errors.)
- Input full scale (IFS) = span
- output full scale (OFS) : difference between the highest and lowest values of the output **of the sensor corresponding to the span of the sensor.**
## ERROR
- Errors : deviation from “ideal”
- static errors: not time dependent
- dynamic errors : time dependent 
- system errors: constant at all times and conditions. can be corrected by calibration.
- random errors : due to uncontrolled variables. can be reduced by averaging.
## Some terms about sensors
- **Resolution 分辨率**: the minimum increment of stimulus **to which it can be responded 能感知到的最小变化**. 
- **Accuracy 准确性**: tells you how close a measured value to the true value 注意和分辨率区分.
- **precision**: how close the measured values to each other 更集中.
- **repeatability or reproducibility** ：failure of the sensor to represent the same value under identical conditions **when measured at different times.** 不同时间，统一条件，不同结果
- **sensitivity 敏感度**: change in output **for a given unit change in input**. represents the slope of the transfer function. 代表可变换函数的斜率
- **response time**：(delay time)
indicates the time needed for the output to reach steady state(达到稳定所需要的时间）
- **Reliability (MTBF)**：
the ability of the device to **perform its stated function, under normal operating conditions without failure.**
# Wireless Sensing
- Contact sensing 如手环检测心率；手机触摸屏
- Contact-free sensing (Light, sound, electricity, magnetism)

**Acoustic Sensing**
- Audio (<20kHz)
- Ultrasound (>20kHz, unaudible)

## RF sensing
**Basic principle**: Targets such as humans in the transmission paths will reflect, refract, diffract 反射，折射，衍射， and scatter the RF signals following physical laws. By capturing these signals and processing the patterns, events in the environment can be sensed.

**3 Types of commonly used wireless media:** WiFi, Millimeter Wave, UWB (Ultra Wide Band)

**Advantages of RF sensing**: 
- contactless
- pervasiveness 广泛性
- low cost (both money and energy) 
- privacy preservation 隐私保护.

**Application of RF Sensing** :
- Localization
- Human activity recognition
- Gesture recognition
- Vital signs

**3 Types of wireless sensing** :
- Acoustic Sensing
- RF Sensing
- RFID

# Crowd Sensing 群体感知
## New Sensing paradigm: Mobile Crowd Sensing
It treat mobile devices of ordinary users as basic sensing units, and leverage them to distribute sensing tasks and collecting sensing data.
## Basic Feature
- Crowd-based information sensing
- Cooperative data transmission
- Crowd intelligence for complex tasks

**People/Human-centric:"Prosumer(Producer+Consumer)**
## Advantages
- Low cost
- easy maintenance
- Good scalability 扩展性强（只需要招募更多用户）

## Challenges
- Sensing quality
- Privacy protection
- Incentive 激励

## 智能传感器(not mentioned in exam)
- 自学习、自诊断与自补偿能力
- 符合感知能力
- 灵活的通信能力

### MEMS
Micro-Elextro-Mechanical Systems 微机电系统，泛指特征尺度在亚微米毫米范围的装置。

## 无线传感器与执行器网络的研究(not mentioned in exam)

随着WSN的不断深入，人们认识到在某些应用环境中必须要将执行器和传感器结合起来，无线传感器与执行器网络(wireless sensor and actor network，WSAN)

传感器节点很多且静态不移动，执行器节点移动，不需要很多。

各个节点之间都要能够协同通信。
- 自主机制：各个传感器节点选择合适的执行器节点执行。
- 半自主机制：传感器节点传到汇聚节点（相当于中控中心）再选择执行器节点执行。
- 协同机制：控制者在控制中心根据汇聚节点收集到的传感器节点信息，向汇聚节点发送指令，再由执行器节点执行。


## 无线多媒体传感网络的研究(not mentioned in exam)
Wireless multimedia sensor network(WMSN)需要对视频、音频、图像等多媒体信息感知、传输、处理，需要比传统WSN更加直观、清晰的信息。

其他：

**Undeerwater Wireless Sensor Network, UWSN 水下无线传感网络** 主要利用声波进行通信和组网。

**Wireless Underground Sensor Network, WUSN 地下无线传感器网络**

**Integrate NanoSensor System, INS 集成纳米传感器系统**

