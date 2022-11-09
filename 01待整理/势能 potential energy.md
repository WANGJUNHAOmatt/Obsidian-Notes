---
aliases: 
tags: 
date created: Sunday, October 9th 2022, 7:03:17 pm
date modified: Wednesday, November 9th 2022, 9:56:11 am
---

## 势能 potential energy

由于 [[力 force#保守力|保守力]] 做功 只与质点 的始末位置 有关，那么，这类功就可以写成某个状态量的差值。

我们把与质点位置有关的能量称为质点的 **势能**，用符号 $E_p$ 表示。

- 势能 是 状态（坐标）的函数
- 势能与 势能零点的选取有关
- 势能不会独立存在，而是属于系统的

于是，万有引力和弹性力的势能分别为：
- 引力势能 $E_p = -G\frac{m'm}{r}$
- 弹性势能 $E_p = \frac{1}{2}kx^2$

### 势能的表示

#### 势能曲线

我们称 势能随坐标变化的曲线 为 **势能曲线**。

##### 重力势能曲线

![[Gravitational_energy.png]]

```python
import numpy as np
import matplotlib.pyplot as plt

# 绘制重力势能曲线

m = 10  
g = 9.8  
y = np.arange(0, 100, 0.1)  
ep = m * g * y  
  
plt.plot(y, ep)  
plt.title("Plot of Gravitational energy")  
plt.xlabel("Height of the particle")  
plt.ylabel("Gravitational energy")  
plt.text(20, 8000, r"$E_p = mgy$")  
plt.text(30, 7000, r"$m = 10\mathrm{kg}$")  
plt.text(30, 6000, r"$g = 9.8 \mathrm{m/s^2}$")  
plt.savefig('./output/Gravitational_energy.png', transparent=False, dpi=80, bbox_inches="tight")  
plt.show()
```

##### 弹性势能曲线

![[ElasticPotentialEnergyCurve.png]]

```python
k = 1  
x = np.arange(-10, 10, 0.01)  
ep = 0.5 * k * (x ** 2)  
  
plt.plot(x, ep)  
plt.title("elastic potential energy curve")  
plt.xlabel("displacement of the spring from its equilibrium point")  
plt.ylabel("Elastic Potential Energy")  
plt.text(0, 45, r"$E_p = \frac{1}{2} k x^2$")  
plt.text(1, 40, r"$(k = 1)$")  
plt.savefig("./output/ElasticPotentialEnergyCurve.png", transparent=False, dpi=80, bbox_inches="tight")  
plt.show()
```


