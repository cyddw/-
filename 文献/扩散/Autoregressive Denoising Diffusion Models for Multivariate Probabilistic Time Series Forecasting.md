## 传统模型的不足

传统的用于时间序列预测的模型大部分聚焦于**单变量**情形，同时其训练数据集**规模小**

## 基本思路

结合自回归模型和EBMs模型，提出了TimeGrad模型，用于解决多元概率时间序列预测问题

## TimeGrad模型

**目标：**

<img width="391" alt="image" src="https://github.com/user-attachments/assets/ff27875f-2e9a-4d72-8869-a61de8a09f0b">

希望通过1:t<sub>0</sub>-1的多变量**x**以及1:T的协变量来预测出t<sub>0</sub>的多变量**x**




 
