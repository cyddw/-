## 现有模型的不足
目前常见的模型有以下三类：物理模型、数据模型以及混合模型  
**物理模型的不足：** 方程数量多，需要保证数据的精确性  
**数据模型的不足：** 难以预测没有历史数据的情形
## 因果模型介绍
### 因果和相关的区别
因果的定义：  
<img width="499" alt="image" src="https://github.com/user-attachments/assets/20982fc4-4c00-4436-9f66-76ff823a9da0">  
### 常见的三种因果模型
CGM:用于描述结构和因果关系，并使用有向无环图表示
SCM:由CGM和一系列结构方程组成，其中结构方程包括函数、内生变量和噪声，**适用于变量之间的函数关系相对明确的情况**  
PO:用于变量之间因果关系复杂且不明确的情况，需要因果效应估计。其中因果估计被用来验证因果关系。
### Average Treatment Effect(ATE)
在PO中，一般通过观察ATE来进行因果估计：  
<img width="251" alt="image" src="https://github.com/user-attachments/assets/7342d361-b96a-4bfc-b975-1d23770a6be6">  
### Instrumental Variable
工具变量是处理隐藏混杂因素(Confounding Variables)的一种常用方法。工具变量能够在SCM和PO框架内进行因果识别。
## 基本思路

## 具体实现
## 结果分析
