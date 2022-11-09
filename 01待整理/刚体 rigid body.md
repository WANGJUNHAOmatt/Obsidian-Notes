---
aliases: 
tags: 
date created: Monday, October 10th 2022, 2:14:16 pm
date modified: Wednesday, November 9th 2022, 9:56:11 am
---

## 刚体

如果在 外力 的作用下，物体的形状和大小不发生变化，也就是说，物体内任意两点的距离都保持恒定，这种理想化的物体就叫做 **刚体**。

## 刚体的运动

### 平动

若刚体中所有点的运动轨迹都保持完全相同，或者说刚体内任意两点间的连线总是平行于它们初始位置间的连线，则刚体的这种运动叫做 **平动**。

### 转动

当刚体中所有的点都绕某一直线做圆周运动时，这种运动叫做 **转动**，而这条直线叫做 **转轴**。 

#### 定轴转动

##### 角速度

在极坐标下，刚体对转轴的角速度为：
$$ \omega = \frac{\mathrm{d}\theta}{\mathrm{d}t} $$

角速度矢量的方向 遵循 **[[右手螺旋定则]]**。

###### 角速度与切向速度的关系

$$
v = r \omega
$$

##### 角加速度

$$
\alpha = \lim_{\triangle t \to 0} \frac{\triangle \omega}{\triangle t} = \frac{\mathrm{d} \omega}{\mathrm{d} t}
$$

###### 角加速度和切向、法向加速度的关系

$$
\begin{align}
a_t &= r \alpha \\
a_n &= r \omega^2 
\end{align}
$$

##### 匀变速转动公式

$$
\begin{align}
\omega &= \omega_0 + \alpha t \\
\theta &= \theta_0 + \omega_0 t + \frac{1}{2} \alpha t^2 \\
\omega^2 &= \omega_0^2 + 2 \alpha(\theta - \theta_0)
\end{align}
$$

#### 非定轴转动
