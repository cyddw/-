### 时间序列数据和时空数据
时间序列数据的定义：  
<img width="457" alt="image" src="https://github.com/user-attachments/assets/4efeec15-9244-4394-a90a-b7c107dce1f4">  
时间序列包括单变量和多变量：  
<img width="243" alt="image" src="https://github.com/user-attachments/assets/0677a9c8-16bb-4b29-ab0e-5b38bd07f317">  
时空数据的定义：  
<img width="512" alt="image" src="https://github.com/user-attachments/assets/6d01ae66-b192-4bb6-8323-57e9a24e718b">  
## 扩散模型
### 1.Denoised Diffusion Probabilistic Models (DDPMs)
**Diffusion Process:**   
通过下面的过程对原始数据进行K步加噪处理： 
  
<img width="853" alt="image" src="https://github.com/user-attachments/assets/2c153f61-57ca-4a91-883b-c5cdb56781a5">  
  
则第k步的数据满足的分布如下：  
  
<img width="515" alt="image" src="https://github.com/user-attachments/assets/dc92e4d1-f881-4e22-a062-a46b83ea6ed4">

根据高斯分布的性质，可以从第0步直接得到第k步的分布：  
  
<img width="520" alt="image" src="https://github.com/user-attachments/assets/ef9fe7b2-f6d3-441b-a180-196be6a6bb5a">

**Denoising Process:**

由贝叶斯公式可以得到：

<img width="600" alt="image" src="https://github.com/user-attachments/assets/e7613937-9acb-42b1-9935-41a5ad597b93">

将具体数值带入，可以得到：

<img width="857" alt="image" src="https://github.com/user-attachments/assets/d6ff88a3-9aad-4063-8856-616a7a640e20">



## 参考文献：[bilibili](https://www.bilibili.com/video/BV1tz4y1h7q1/?spm_id_from=333.337.search-card.all.click&vd_source=887e79a2964e5ce84cbcf68e50febd27)

