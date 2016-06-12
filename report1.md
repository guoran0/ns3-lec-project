#**实验报告**#
##郭冉 2012019020018##
### 实验要求 ###
1、用命令行输入自己的姓名，学号以及输出频率。

2、利用unix实用工具wc(word count)统计输出的总次数。

3、利用unix实用工具grep筛选特定信息


### 实验结果及分析 ###


![输入姓名、学号及输出频率的终端输出截图](http://i.imgur.com/BVnNhH1.png)

在hello-simulator.cc中分别增加创建string型变量number，double型变量frequency用来存储学号及输出频率，并将仿真停止时间改为10秒，如图所示，姓名name参数输入GR，学号number参数输入2012019020018，输出频率frequency参数输入3。

![利用wc、grep进行统计及筛选截图](http://i.imgur.com/hUGlY0H.jpg)

如图所示，对scratch文件夹下的hello-simulator.cc进行word count统计，输入命令wc hello-simulator.cc显示结果为54行，213个单词，1632个字节。

在终端输入时加入筛选命令grep，输入 ./waf --run="scratch/hello-simulator --name=GR --number=2012019020018 --frequency=3"|grep "+6"，可以筛选出第六秒的输出情况。

之后在提交的过程中将hello-simulator.cc改名为ns3-lec1-project1.cc提交到github完成任务。