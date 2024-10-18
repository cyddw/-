## 参考文献：[知乎](https://zhuanlan.zhihu.com/p/123211148)


### RNN的优势

**RNN对具有序列特性的数据非常有效，它能挖掘数据中的时序信息以及语义信息**，利用了RNN的这种能力，使深度学习模型在解决语音识别、语言模型、机器翻译以及时序分析等NLP领域的问题时有所突破。

相比于全连接神经网络，RNN可以更好的挖掘语义：

> <img width="676" alt="image" src="https://github.com/user-attachments/assets/5a00085c-ffd3-4ce2-a7e6-16a539f79f62">

### RNN的基本原理

RNN原理图如下：

> <img width="537" alt="image" src="https://github.com/user-attachments/assets/f787fc7e-9287-49d0-881f-9f233a3df28a">

抛开W参数，剩下的X->U->S->V->O即为全连接神经网络，因此输入输出公式如下：

> <img width="346" alt="image" src="https://github.com/user-attachments/assets/e50302f9-d0d1-4bc3-a097-ea7a5afbf48a">



