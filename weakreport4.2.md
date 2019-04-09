## <p align = "center"> 工作周报 </p> ##
<p align="center">(4.9-4.14)</p>

### 1. 主要内容 ###
1.将之前的类别0-9由原本的单一类别修改为九个类别(即缺少一个类别)，计算不同数据集激活位置占总数的百分比。
2.用数学表示类别10比类别0-9表现更好，考虑用一段区间上的均值,即平均激活位置,公式为:
&emsp;&ensp;&ensp;&ensp;$AvgActPosition=\frac{\sum_{i}^n\sum_{i}^k ActivatePosition(J)}{n} $
其中：
&emsp;&emsp;&emsp;J为数据集
&emsp;&emsp;&emsp;K为神经网络的全连接层的层数
&emsp;&emsp;&emsp;n为下图中激活次数的区间
&emsp;&emsp;即计算一段区间上一个数据集激活的位置百分比的均值，有图可见类别10(十个类别均有的数据集)优于类别0-9(缺少一个类别的数据集)
<div align="center">
<img src="C:\Users\zhangkai\Documents\git\ninekind.png" align="center"></div>
### 2.下周计划 ###
1、考虑识别准确率与单张图片或一个数据集之间的关系，从而可以将数据集进行排序，易识别错误的图片排在数据集前部。
