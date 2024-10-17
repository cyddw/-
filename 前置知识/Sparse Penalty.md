## 参考文献：[CSDN](https://blog.csdn.net/xys430381_1/article/details/110456496)

> ### 什么是penalty term？

> 罚函数的基本思想是构造辅助函数，把原来的约束问题转化为求辅助函数极小化的无约束问题。

## 什么是惩罚(正则化)

我们经常看到，标准损失函数通常由两项组成，**数据损失项和惩罚项**，并将惩罚项乘以超参数λ，用来平衡这两项。

其中惩罚项的作用就是**防止模型过拟合，提高模型的泛化能力**

> <img width="299" alt="image" src="https://github.com/user-attachments/assets/86360bc2-67dd-4373-9cd5-3188d9760d24">

