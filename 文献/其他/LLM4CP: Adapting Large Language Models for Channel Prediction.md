## 现有模型的不足  
现有的基于深度学习的信道预测模型缺乏对实际模型的完美匹配，同时存在泛化能力差等问题。  
**1.** 现有模型的预测能力受到网络规模的限制。难以准确地模拟复杂的空间、时间和频率关系，特别是对于高速场景和FDD系统。  
**2.** 与基于模型的方法相比，基于深度学习的方法表现出较差的泛化能力，当CSI分布发生变化时，需要进行再训练。而诸如元学习等提高泛化能力的方法需要增加计算复杂度。
## 基本思路
考虑到LLM的泛化能力和建模能力，利用上行链路的历史CSI结合LLM预测下行链路的未来CSI，同时解决了CSI数据迁移到LLM的问题
## 具体实现
### 前提假设
单个BS和单个用户组成的多输入单输出（MISO）OFDM模型
### 符号说明
N<sub>t</sub>=N<sub>h</sub>×N<sub>v</sub>表示BS的天线数量  

<img width="446" alt="image" src="https://github.com/user-attachments/assets/a09ae541-100b-4548-94d1-4cb8cab72073">

### 信道模型
假定BS端使用UPA天线，用户端使用全向天线，同时考虑基于簇的多径信道模型，则在时刻t，频率f的下行链路的CSI表示如下：  
<img width="380" alt="image" src="https://github.com/user-attachments/assets/ec4e6c5c-4683-4d70-80b8-ac299787a2c7">  
其中，导向矢量具体建模如下：  
<img width="389" alt="image" src="https://github.com/user-attachments/assets/100382cb-492f-40be-8a85-d59f6f3f3196">  
### 信号模型
考虑BS端进行[预编码](https://blog.csdn.net/weixin_43871127/article/details/104593325)，则接收端信号表示如下：  
<img width="376" alt="image" src="https://github.com/user-attachments/assets/789ae755-7941-4e3e-a476-17e9433bc48b">  
频谱效率表示如下：  
<img width="380" alt="image" src="https://github.com/user-attachments/assets/7cad7944-9ae9-4592-aa32-3e72a1ac53eb">  
预编码矩阵选择如下：  
<img width="383" alt="image" src="https://github.com/user-attachments/assets/71ede610-9b25-4257-84fe-cc20f61239c2">
### 预测模型
传统的TDD和FDD模型对下行CSI的获取：  
<img width="568" alt="image" src="https://github.com/user-attachments/assets/ab5f055c-7580-440c-9915-02046b6ecc81">  
基于LLM的信道预测模型：  
<img width="598" alt="image" src="https://github.com/user-attachments/assets/444f4dab-9e35-4ef4-9413-1650c910b570">  
目标函数：  
<img width="424" alt="image" src="https://github.com/user-attachments/assets/3460d946-de87-4cf0-bb05-51059b34f1dc">  
其中，NMSE表示归一化均方误差




## 结果分析
