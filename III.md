
第三讲数字交换原理与交换网络


![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-01.jpg?height=616&width=862&top_left_y=806&top_left_x=248)





![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-01.jpg?height=354&width=2442&top_left_y=1561&top_left_x=241)



回顾已学知识点

- 交换(Switching) 的含义是什么? 
 - 交换机(Switch)在通信网中的作用是什么?



交换如何实现？

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-03.jpg?height=619&width=753&top_left_y=746&top_left_x=500)

S:电话交换机

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-03.jpg?height=866&width=1022&top_left_y=656&top_left_x=1484)

可能方案之一 

- 最重要的交换技术之一: 电路交换

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-04.jpg?height=1044&width=1895&top_left_y=742&top_left_x=503)



一. 同步数字交换原理(重点)

二. TST 交换网络

三. 其它T/S交换网络

本讲小结 
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-06.jpg?height=1628&width=1954&top_left_y=268&top_left_x=264)- 程控交换机是一种电路交换设备, 其核心技术就是同步数字交换技术！

- 同步数字交换:属于电路交换模式
它主要基于两种技术来实现数字信号的交换:
(1) 同步TDM (同步时分多路复用)
(2) 时隙交换 (语音信号的传输从一个时间片切换到另一个时间片) 

#### 1.1 同步时分复用原理

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-08.jpg?height=952&width=2106&top_left_y=566&top_left_x=438)

多路复用 Multiplex

解复用(分路) \\ Demultiplex

同步时分复用原理

- 同步TDM (Time Division Multiplexing)

时隙的分配是固定的;

时隙的划分(或时隙长度)也是固定的。

- 电信网PCM数字语音时分复用标准:

30/32 CH, 64k·32 2048kbps - E1标准

$24 CH$, 1544kbps — T1标准 

2 时隙交换原理
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-10.jpg?height=978&width=2152&top_left_y=644&top_left_x=352)

$\begin{array}{lllll}4 & 3 & 2 & 1 & 0\end{array}$

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-10.jpg?height=161&width=582&top_left_y=1471&top_left_x=1753)



时隙交换原理 - 动态演示

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-11.jpg?height=709&width=2152&top_left_y=645&top_left_x=356)

时隙 432120
43210

开关总是按时隙顺序接通各触点。
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-11.jpg?height=178&width=1320&top_left_y=1468&top_left_x=1033)

3 同步数字交换单元器件

- $T$ 接线器 (Time Switch):

又称为时间交换单元

共享存储器型

- S 接线器 (Space Switch):

又称为空间交换单元

共享开关阵列型 

T 接线器 (时间交换单元)

TS $\begin{array}{llllll} & 4 & 3 & 2 & 1 & 0\end{array}$

SM:话音存储器

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-13.jpg?height=175&width=665&top_left_y=651&top_left_x=324)

$\underset{\rightarrow}{ } \rightarrow$

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-13.jpg?height=541&width=597&top_left_y=651&top_left_x=1055)

CM:控制存储器 tII,

计数器

时钟脉冲 (周期: 1时隙)

TS: 时隙 (Time Slot)

SM: 话音存储器 (Speech Memory)

CM: 控制存储器 (Control Memory)

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-13.jpg?height=590&width=764&top_left_y=1309&top_left_x=1061)

TS $4 \begin{array}{lllll} & 3 & 2 & 1 & 0\end{array}$

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-13.jpg?height=179&width=698&top_left_y=664&top_left_x=1844)

输出控制方式

(顺序写入, 控制读出)

地控制方式反映了话音数据是圵 如何写入和读出存储器的。

控制存储器保存了话音数据的读出地址, 这些地址数据总是自动地从存储器中按顺序读出的, 并且预先由控制系统写入存储器, 而在话音交换过程中保持不变。

CPU 写入

思考题

- 时间交换单元会带来交换时延吗? 如果有, 最大时延是多少?

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-14.jpg?height=694&width=1126&top_left_y=973&top_left_x=940)

$T$ 接线器 (输出控制方式) - 动态演示

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-15.jpg?height=1354&width=2327&top_left_y=561&top_left_x=328)



$T$ 接线器 (输入控制方式)

TS $4 \begin{array}{lllll} & 4 & 2 & 1 & 0\end{array}$

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-16.jpg?height=191&width=671&top_left_y=643&top_left_x=317)

SM:话音存储器
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-16.jpg?height=482&width=332&top_left_y=641&top_left_x=811)

无码了？
计洣品楍
日寸钟脉旪
(庤其:1日寸隙) C

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-16.jpg?height=533&width=563&top_left_y=666&top_left_x=1091)

CM:控制存储器

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-16.jpg?height=564&width=642&top_left_y=1318&top_left_x=1089)

TS $4 \begin{array}{lllll} & 3 & 2 & 1 & 0\end{array}$

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-16.jpg?height=190&width=698&top_left_y=666&top_left_x=1844)

输入控制方式

(控制写入,顺序读出)

控制方式反映了话音数据是如何写入和读出存储器的。

控制存储器保存了话音数据的写入地址, 这些地址数据总是自动地从存储器中按顺序读出的, 并且预先由控制系统写入存储器, 而在话音交换过程中保持不变。

$CPU$ 写入 

T接线器 (时间交换单元)

- 对于时间交换单元, 不论采用哪种工作方式, 每个输入时隙的信息都将占用一个存储单元, 每个存储单元都占有一定的空间位置，从这点看，时间交换单元虽是时隙交换, 但却是以 “空间” 位置的分配来实现交换的，所以，时间交换单元实质上是按 “空分” 存储方式工作的。 

话音存储器SM

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-18.jpg?height=1201&width=2059&top_left_y=265&top_left_x=354)

控制存储器 CM

练习: 时间接线器(输入控制方式)



(空间交换单元)
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-19.jpg?height=1046&width=2300&top_left_y=492&top_left_x=338)

时钟脉冲

(周期: 1时隙)

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-19.jpg?height=350&width=257&top_left_y=1220&top_left_x=983)

$:$

CMO

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-19.jpg?height=500&width=217&top_left_y=1197&top_left_x=1249)

CM1

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-19.jpg?height=518&width=187&top_left_y=1218&top_left_x=1458)

CM2 也有人称之为“输入控制”，因为控制存储器是为输入线分配的。

CPU 写入



(空间交换单元)

- 工作方式: 1)输入控制方式, 2)输出控制方式

- 空间交换单元的交叉接点按时隙高速接通与断开。如一帧中有不同时隙的信码要交换到同一条输出线上, 则在CM 控制下的交叉接点在一帧内就要开、关若干次。即:空间交换单元的交叉接点是以时分方式工作的，所以又叫 “时分复用的空间接线器” 。 

接线器 (输出控制方式)
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-21.jpg?height=1032&width=2250&top_left_y=518&top_left_x=322)

时钟脉冲

(周期:1时隙)
![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-21.jpg?height=558&width=982&top_left_y=1220&top_left_x=834)

输出控制方式 (控制出线的选择) 也有人称之为“输入控制”, 因为控制存储器是为输入线分配的。

CPU㝍入

CM3

控制存储器 

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-22.jpg?height=183&width=2018&top_left_y=315&top_left_x=539)

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-22.jpg?height=1339&width=2238&top_left_y=494&top_left_x=369)



填空题 2分

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-23.jpg?height=1708&width=2439&top_left_y=228&top_left_x=250)

- $T$ 接线器:

实现时隙交换

- $S$ 接线器:

只改变线路(方向), 不改变时隙!

一条入线(或出线)上的所有开关是分时动作的! (即:在任意时刻, 相连的入线和出线是一一对应的。)

- 接线器中各存储器 (CM/SM) 的存储单元数等于一帧所包含的时隙数 (复用信道数)。

- 多个交换单元 (T/S 接线器) 互联可以构成大容量的交换网络, 但仅有S接线器不能独立构成交换爻络, 必须与T 接线器结合！ 

二、TST 交换网络

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-25.jpg?height=988&width=2215&top_left_y=841&top_left_x=269)

第3讲数字交换原理与交换网络 (授课：陈科文) 

TST 三级交换网络

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-26.jpg?height=873&width=2286&top_left_y=552&top_left_x=319)

TST网络结构示例 $\quad$ iHW/oHW: 输入/输出多路复用总线 (Highway).
TS : 时隙 (Time Slot)

练习： 根据本图和已知条件, 画出TST交换原理图。 

TST 三级交换原理分析

练习： 说明三级交换TST的交换原理

1. 确定其中的各个控制存储器 (CM) 和话音存储器 (SM)的容量(即:存储单元数和每单元的比特数)。

2. 根据图中的已知条件, 画出相应的存储器 (T的SM 和CM，S的CM，并绘图表示S的控制方式)，然后填写各存储器的内容, 以实现所要求的交换。

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-27.jpg?height=548&width=1100&top_left_y=1233&top_left_x=1501)



![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-28.jpg?height=1823&width=2454&top_left_y=73&top_left_x=235)

《 第三讲数字交换原理与交换网络 》 

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-29.jpg?height=105&width=2059&top_left_y=313&top_left_x=410)

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-29.jpg?height=973&width=2264&top_left_y=457&top_left_x=285)

第三级所有 T接线器是不是多余的?

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-29.jpg?height=481&width=317&top_left_y=1415&top_left_x=1773)



思考题(关于TST网络)

- TST交换网络中, 一条入线上某个时隙的信息通过第一级 $T$ (改变时隙)和第2级 $S$ (改变线路), 就能交换到任何一条出线上的任何一个时隙中, 那么第三级T是不是多余的? 加上这一级的主要目的又是什么呢?

![](https://cdn.mathpix.com/cropped/2023_04_26_c808929090de211105c2g-30.jpg?height=570&width=1108&top_left_y=1162&top_left_x=1098)

T/S时分交换网络的结构分析


1. 将时分交换网络转换成等效的空分交换网络。

时分交换单元 $\rightarrow$ 空分交换单元

连接各级相对应的空分交换单元

2. 找出从一条入线到达某条出线的所有内部路径。



1)时分交换单元的等效空分交换单元
![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-02.jpg?height=1046&width=1870&top_left_y=704&top_left_x=434)

三级TST网络结构

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-03.jpg?height=880&width=2253&top_left_y=545&top_left_x=317)

第三级所有T接线器 是不是多余的?

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-03.jpg?height=485&width=317&top_left_y=1410&top_left_x=1770)



2) T/S交换网络的等效空分网络

- TST网络的等效空分网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-04.jpg?height=996&width=1805&top_left_y=733&top_left_x=526)



3)等效空分交换网络的内部通路

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-05.jpg?height=1294&width=2134&top_left_y=502&top_left_x=287)



提问

T/S交换网络的阻塞率如何计算?

2. 能不能设计出无阻塞的T/S交换网络?

- 先回答第2个问题!



4) 无阻塞的三级交换网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-07.jpg?height=537&width=1593&top_left_y=709&top_left_x=643)

三级空分交换网络

无阻塞的条件：  $k \geq n_{1}+n_{2}-1$



思考题

- 怎样将一个TST网络变成无阻塞网络?  (要求：说明具体的实现方法)

(提示: 先画出等效空分网络, 再根据CLOS网络无阻塞条件确定各 $T / S$ 接线器的存储器容量及其读写周期)。

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-08.jpg?height=604&width=1174&top_left_y=1041&top_left_x=1151)



三、其它T/S 交换网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-09.jpg?height=1052&width=1797&top_left_y=839&top_left_x=269)



(1) S-T-S 网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-10.jpg?height=634&width=1745&top_left_y=835&top_left_x=593)



(2)三级 T/S组合交换网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-11.jpg?height=641&width=1530&top_left_y=847&top_left_x=656)



(3) T-S-S-T 网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-12.jpg?height=884&width=1850&top_left_y=781&top_left_x=537)



(4) T-S-S-S-T 网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-13.jpg?height=918&width=1861&top_left_y=697&top_left_x=643)

(EWSD 交换机 )



(5) S-S-T-S-S 网络

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-14.jpg?height=649&width=1533&top_left_y=839&top_left_x=673)



不同结构的T/S 交换网络

- T-S-T三级网络

- S-T-S三级网络

- T-S-S-T四级网络

- T-S-S-S-T五级网络

- S-S-T-S-S五级网络

- 多级T/S结合型交换网络

- TTT三级网络

- TTTT四级网络、等等。 
![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-16.jpg?height=1642&width=1834&top_left_y=272&top_left_x=264)

电路交换的核心技术:

- 同步数字交换原理(重点)

时间 $(T)$ 接线器、空间 $(S)$ 接线器

- 典型T/S 交换网络的结构分析

不同结构, 决定不同性能和实现方式



电路交换方式

- 原理:

“开关切换”、同步时分复用

通信过程: 建立连接、传递信息、释放连接

- 特点:

带宽固定、延迟小、实时性强

线路(资源)利用率低、无差错控制

- 应用:

适于语音通信、高速传真等(如用于PSTN等电信网)

不适合突发和对差错敏感的数据业务。 

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-19.jpg?height=1861&width=2458&top_left_y=62&top_left_x=233)



练习题1

有一个同步数字S (空间) 接线器, 它有8条入线和8条出线，编号为 $0 \sim 7$, 各入线或出线上传输的每个TDM帧都有32个时隙。如果要将0号入线上23号时隙中的数据交换到7号出线上去, 试画图说明其交换原理 (要求: 在图中标明S接线器的控制方式，并填写其控制存储器中相应存储单元的地址和内容)。



练习题2

- 有一个同步数字 $T$ (时间)接线器, 它的话音存储器有1024个单元, 采用输入控制方式。如果要将该 T接线器输入线路上的357号输入时隙 (即TS357) 中的数字语音样本 (A) 交换到246号输出时隙

(TS246)中去, 试说明其交换原理(要求: 画出交换原理图，确定各存偖器的容量，并填写相应存储单元的地址和内容) 。 

练习题3：画图说明TST 网络交换原理

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-22.jpg?height=877&width=2290&top_left_y=546&top_left_x=317)

TST网络结构示例 $iHW / HW$ : 输入/输出多路复用总线 (Highway).
TS : 时隙 (Time Slot)

练习： 根据本图和已知条件，画出TST交换原理图。



思考题

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-23.jpg?height=686&width=914&top_left_y=526&top_left_x=826)

说明两部电话机A和B 通过TST交换网络实现双向通信的原理。 (要求: 画出电话机A发送至电话机B、电话机B发送至电话机A的语音信号在程控交换机内部传输和交换的原理图。)



课前导学

- 下一讲预告:

《数字交换网络的设计与分析》

- 思考以下问题:

1. 交换㲼络的言旺如何不角定?

2. 交换模块为什么要采用多级结构?

3. 交换网络的拓扑结构怎么设计? (各级交换单元怎样互连? )

4. 怎样分析交换网络的性能？(阻塞率如何计算?)

5. 如何改进交换网络的结构? 

![](https://cdn.mathpix.com/cropped/2023_04_26_85106d31b9d1b2d29decg-25.jpg?height=1868&width=2464&top_left_y=58&top_left_x=230)