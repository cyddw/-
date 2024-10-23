## 参考文献：[U型槽无线信道多径传播特性测量与建模方法的研究](https://xueshu.baidu.com/usercenter/paper/show?paperid=9d5e9d5d9315c0accfaae7850234ac4a)、[移动通信基础](https://blog.csdn.net/pgone1/article/details/125843891)
### 宽带信道和窄带信道
**宽带系统：** 信道带宽大于多径信道的相关带宽，使得接收端收到的信号之间产生干扰  
**窄带系统：** 信道带宽小于多径信道的相关带宽
### CDL  
CDL下的信道冲激响应表示如下：  
<img width="496" alt="image" src="https://github.com/user-attachments/assets/f9b0f48e-fbf1-4ea1-9dc9-a335b4826171">  
其中，T<sub>l</sub>表示第l个簇到达的时间，即第l个簇中第1条ray到达的时间，τ<sub>kl</sub>表示第l个簇中第k条ray到达的时间和T<sub>l</sub>的差值

### [CDL参数](https://developer.aliyun.com/article/743747#:~:text=%E2%80%A2%20%E6%B0%B4%E5%B9%B3%E5%8F%91%E5%B0%84%E8%A7%92%EF%BC%88AOD%EF%BC%8CAzimuth%20of%20Departure%EF%BC%89%EF%BC%9A%E7%A9%BA%E9%97%B4%E4%BF%A1%E9%81%93%E5%A4%9A%E5%BE%84%E4%B8%8E%E5%8F%91%E5%B0%84%E7%AB%AF%E6%B0%B4%20%E5%B9%B3%E6%96%B9%E5%90%91%E7%9A%84%E5%A4%B9%E8%A7%92%EF%BC%9B%20%E2%80%A2%20%E6%B0%B4%E5%B9%B3%E5%88%B0%E8%BE%BE%E8%A7%92%EF%BC%88AOA%EF%BC%8CAzimuth,of%20Arrival%EF%BC%89%EF%BC%9A%E7%A9%BA%E9%97%B4%E4%BF%A1%E9%81%93%E5%A4%9A%E5%BE%84%E4%B8%8E%E6%8E%A5%E6%94%B6%E7%AB%AF%E6%B0%B4%E5%B9%B3%20%E6%96%B9%E5%90%91%E7%9A%84%E5%A4%B9%E8%A7%92%EF%BC%9B%20%E2%80%A2%20%E5%9E%82%E7%9B%B4%E5%8F%91%E5%B0%84%E8%A7%92%EF%BC%88ZOD%EF%BC%8CZenith%20of%20Departure%EF%BC%89%EF%BC%9A%E7%A9%BA%E9%97%B4%E4%BF%A1%E9%81%93%E5%A4%9A%E5%BE%84%E4%B8%8E%E5%8F%91%E5%B0%84%E7%AB%AF%E5%9E%82%E7%9B%B4%20%E6%96%B9%E5%90%91%E7%9A%84%E5%A4%B9%E8%A7%92%EF%BC%9B)

+ AOD：离开方位角

+ AOA：到达方位角

+ ZOD：离开天顶角

+ ZOA：到达天顶角
