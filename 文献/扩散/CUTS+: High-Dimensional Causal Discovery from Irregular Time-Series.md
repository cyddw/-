## 总结

这篇paper提出了两个方法:**C2FD**和**MPGNN**，前者解决了数据维度过高的问题，后者不仅减少了计算开支也补全了irregular数据的不足。同时也提供了**如何从高维数据发现Granger因果**的方法，但是其未考虑**confounding factor**的问题

## 现有模型的不足

**CUTS模型**在应对高维数据时表现出不足，而**现有的因果发现模型**局限于处理N<20的数据集，难以处理大型数据集

## 因果发现模型的分类

+ Constraint-based approaches

+ Score-based learning algorithms

+ Convergent Cross Mapping

+ Additive Noise Model-based approaches

+ Granger-causality-based approaches

## 基本思路

> <img width="781" alt="image" src="https://github.com/user-attachments/assets/e5568478-bb32-457f-bbf1-aacd9d6869d4">

由上图可知，整体框架分为两个部分：**Causal Discovery Stage**和**Prediction Stage**

+ Causal Discovery Stage：发现变量之间的Granger因果关系

+ Prediction Stage：预测数据，对缺失的irregular数据进行插值补充

### Causal Discovery Stage

+ 引入**Coarse-to-fine Causal Discovery**方法，其目的是为了减少大型数据集带来的维度爆炸问题，基本思想：

> 将N*T的数据集按照N这个维度进行分割，分割成多个互斥的子集;在模型训练的过程中逐渐对每个子集再细分，直至每个子集只有一个变量

+ 引入矩阵M：

> <img width="373" alt="image" src="https://github.com/user-attachments/assets/ea7ec812-acc3-4c01-bdaa-5e30a9862822">

其中，G<sup>T</sup>表示同一子集所包含的元素矩阵，Q表示变量间的因果概率矩阵

+ Loss Function:

> <img width="468" alt="image" src="https://github.com/user-attachments/assets/07b8d7d4-7873-4674-aac3-593670b26949">

### Prediction Stage

+ 引入Gumbel-softmax对Causal Discovery Stage得到的M进行采样

+ 对原有的GPUs增加MPNN层以减少神经网络的冗余性

+ Loss Function：

> <img width="463" alt="image" src="https://github.com/user-attachments/assets/8cdd55d6-2884-45e7-9779-c57e8acf915d">


