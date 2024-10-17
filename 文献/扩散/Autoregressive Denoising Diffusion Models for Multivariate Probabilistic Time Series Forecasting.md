## 总结

这篇paper提出了一个用**DM模型**解决**多元概率时间序列预测**的方法

## 传统模型的不足

传统的用于时间序列预测的模型大部分聚焦于**单变量**情形，同时其训练数据集**规模小**

## 基本思路

结合自回归模型和EBMs模型，提出了TimeGrad模型，用于解决多元概率时间序列预测问题

## TimeGrad模型

**目标：**

<img width="391" alt="image" src="https://github.com/user-attachments/assets/ff27875f-2e9a-4d72-8869-a61de8a09f0b">

希望通过1:t<sub>0</sub>-1的多变量**x**以及1:T的协变量来预测出t<sub>0</sub>:T的多变量**x**

**基本思路：**

<img width="436" alt="image" src="https://github.com/user-attachments/assets/e7e89991-f2e1-4b00-9184-0f7edc52a1fa">

通过RNN网络，输入t-1时刻前的数据、t时刻的协变量以及t-2时刻隐藏层的特征，输出得到t-1时刻隐藏层的特征，将该特征作为参数输入扩散模型中，得到t时刻的数据

**具体步骤：**

**1.RNN网络训练**

<img width="365" alt="image" src="https://github.com/user-attachments/assets/e3b28940-d9fc-4822-bd26-0f07c1271003">

**2.数据输入**

**3.DM模型采样**

<img width="368" alt="image" src="https://github.com/user-attachments/assets/702b44e4-da6d-40a0-b191-86604d280649">







 
