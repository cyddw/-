## 参考文献：[CSDN](https://blog.csdn.net/xys430381_1/article/details/110456496)、[CSDN](https://blog.csdn.net/oTengYue/article/details/89644170)

## 什么是惩罚(正则化)

我们经常看到，标准损失函数通常由两项组成，**数据损失项和惩罚项**，并将惩罚项乘以超参数λ，用来平衡这两项。

其中惩罚项的作用就是**防止模型过拟合，提高模型的泛化能力**

> <img width="299" alt="image" src="https://github.com/user-attachments/assets/86360bc2-67dd-4373-9cd5-3188d9760d24">

其中，第一项是Loss Function，我们希望其尽可能小；第二项是Penalty Term，我们也希望其尽可能小(因为其越小，说明该模型越简单)

由于Penalty Term代表模型复杂度，因此其一般是**模型复杂度的单调递增函数**，例如：

> <img width="579" alt="image" src="https://github.com/user-attachments/assets/1d30d152-de46-4eac-b81e-e1a83b170f8c">

## L0、L1和L2范数

+ L0范数：向量中非0元素的个数

> L0范数

+ L1范数：向量中各个元素绝对值之和

+ L2范数：向量元素绝对值的平方和再开平方
