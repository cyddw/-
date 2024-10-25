## 参考文献：[知乎](https://zhuanlan.zhihu.com/p/36529237)

## RBM的基本思路

> <img width="607" alt="image" src="https://github.com/user-attachments/assets/f76edebc-2781-4eb1-8d22-a159c995c658">

对于上述的二层神经网络，RBM与传统MLPs不同的是，其多了一个反向的过程，即从隐藏层输入，从可见层输出，其中权重w不变，偏置b改变，并通过KL散度作为目标函数，使得输出的预测分布和实际输入分布尽可能一致：

> <img width="615" alt="image" src="https://github.com/user-attachments/assets/450d6415-aa28-4165-976f-378c712d7df5">

## RBM的应用

> <img width="783" alt="image" src="https://github.com/user-attachments/assets/3ea3a209-d537-41a2-a375-79fd36257369">

