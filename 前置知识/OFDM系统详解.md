## 资源块(Resource Block)  
<img width="770" alt="image" src="https://github.com/user-attachments/assets/2339b23b-2813-4685-a8f5-0f09bdbeea21">

### 参考文献：[知乎](https://zhuanlan.zhihu.com/p/24416610)

## OFDMA和OFDM
**OFDM工作模式（左图）：用户是通过不同时间区分出来的。每一个时间片段，一个用户完整占据全部的子载波，并且发送一个完整的数据包（如图中红色部分标出的WLAN Packet）。**  
  
**OFDMA工作模式（右图）：用户是根据时频资源块RU区分出来的。我们首先将整个信道的资源分成一个个小的固定大小的时频资源块，这个时频资源块也就是RU（Resource unit）。在该模式下，用户的数据是承载在每一个RU上的，故从总的时频资源上来看，每一个时间片上，有可能有多个用户同时发送。**  
<img width="773" alt="image" src="https://github.com/user-attachments/assets/4002f231-9279-4a30-a258-8ff0de0e30df">  
### 参考文献：[知乎](https://zhuanlan.zhihu.com/p/24416610)

## 导频  
在802.11中，始终是用特定的子载波作为导频子载波，从而完成信道估计的功能，在802.11ax中，导频子载波的分配如下：  
<img width="698" alt="image" src="https://github.com/user-attachments/assets/21bd71b2-5778-47cb-882c-561f2abba4e7">  
其中红色的直线即代表导频子载波的位置，其导频资源是均匀分布在整个信道上的。比如在RU为26个子载波的情况下，每一个RU中都包含了2个pilot，在RU为52个子载波的情况下，每一个RU包含4个pilot。通过这些pilot的设置，在传输过程中，接收方才可以有效地估计信道，并完成解调的工作。

### 参考文献：[知乎](https://zhuanlan.zhihu.com/p/24416610)


