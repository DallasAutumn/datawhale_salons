###### <sup>Task03</sup><br><sub>常见分布与假设检验</sub><br>**99-华广学习小队-段秋阳**<br>*2020.06.27*

<div STYLE="page-break-after: always;"></div>

# 一般随机变量

离散型随机变量，连续型随机变量

连续型随机变量的概率密度函数：

$$P\{a\le X \le b\}=\int_a^b f(x)dx$$

# 常见分布

## 离散型分布

### 二项分布

n次伯努利试验产生的结果的概率分布

$$P(X=k)=C_n^kp^kq^{n-k}$$

### 泊松分布

$$P\{X=k\}=e^{-\lambda}\frac{\lambda^k}{k!}$$

### 几何分布

经过$k$次实验首次成功的概率：

$$p\{X=n\}=(1-p)^{n-1}p$$

### 负二项分布

实验一直进行到成功$r$次的概率：

$$P\{X=n\}=C_{n-1}^{r-1}p^r(1-p)^{n-r}$$

### 超几何分布

$$P\{X=n\}=\frac{C_k^xC_{N-k}^{n-x}}{C_N^n}$$

## 连续型分布

### 均匀分布

$$f(x)=\begin{cases}\frac{1}{b-a}&&a\le x\le b\\0&& others\end{cases}$$

$$F(x)=\begin{cases}0&&x<a\\\frac{x-a}{b-a}&&a\le x\le b\\1&&x>b\end{cases}$$

### 正态分布

$$f(x)=\frac{1}{\sqrt{2\pi}\sigma}\exp\{-\frac{(x-\mu)^2}{2\sigma^2}\}$$

### 指数分布

$$f(x)=\begin{cases}\lambda e^{-\lambda x}&&x\ge 0\\0&&x<0\end{cases}$$

$$F(x)=P\{X\le x\}=1-e^{-\lambda x}$$

指数分布的无记忆性：

$$P\{X>s+t|X>t\}=P\{X>s\}$$

# 假设检验

## 正态总体的样本均值与样本方差的分布

### 单个正态总体

样本均值的分布：

$$\overline X\sim N(\mu, \sigma^2), \frac{\overline X-\mu}{\sigma/\sqrt n}\sim N(0,1),\frac{\overline X-\mu}{s/\sqrt n}\sim t(n-1)$$

样本方差的分布：

$$\sum_{i=1}^n(\frac{X_i-\mu}{\sigma})^2\sim\chi^2(n),\frac{(n-1)s^2}{\sigma^2}=\sum_{i-1}^n(\frac{X_i-\overline X}{\sigma})^2\sim\chi^2(n-1)$$

### 两个正态总体

$$S_{XY}^2=\frac{(n_1-1)S_X^2+(n_2-1)S_Y^2}{n_1+n_2-2}$$

样本均值差的抽样分布：

$$\overline X-\overline Y\sim N(\mu_1-\mu_2,\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}),\frac{\overline X-\overline Y-(\mu_1-\mu_2)}{\sqrt{\sigma_1^2/n_1+\sigma_2^2/n_2}}\sim N(0,1)$$

样本方差比的抽样分布：

$$F=\frac{S_X^2/\sigma_1^2}{S_Y^2/\sigma_2^2}\sim F(n_1-1,n_2-1)$$

特别地，当$\sigma_1^2=\sigma_2^2=\sigma^2$时，

$$T=\frac{\overline X-\overline Y-(\mu_1-\mu_2)}{S_{XY}\sqrt{\frac{1}{n_1}+\frac{1}{n_2}}}\sim t(n_1+n_2-2)$$

$$W=\frac{(n_1+n_2-2)S_{XY}^2}{\sigma^2}\sim\chi^2(n_1+n_2-2)$$

> 有了这些分布之后，就可以在此基础上进行区间估计和假设检验















