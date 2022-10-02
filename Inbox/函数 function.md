---
aliases: 
tags: 
title: 函数 function
date created: Tuesday, September 13th 2022, 12:25:59 pm
date modified: Thursday, September 29th 2022, 11:29:14 pm
---

## 属性
$$
u = f(P), \quad P(x_1, x_2, \cdots, x_n) \in D
$$

### 元

函数可以接受的输入参数数量，就是函数的「元」

### 连续

#### 在某点连续

$$
\lim_{(x, y) \to (x_0, y_0)}f(x, y) = f(x_0, y_0)
$$
此时，$f(x, y)$ 在 $P_0(x_0, y_0) \in D$ 点 **连续**。

#### 间断点

若 $f(x, y)$ 在 $P_0(x_0, y_0) \in D$ 点不连续，则称 $P_0(x_0, y_0)$ 是 函数 $f(x, y)$ 的一个间断点。


## 运算

### 导数

#### 偏导数

对于二元函数 $z = f(x, y)$，如果只有 自变量 $x$ 变化，此时函数对 $x$ 的导数，就称为二元函数 $z = f(x, y)$ 对于 $x$ 的**偏导数**。

计作 $\frac{\partial z}{\partial x}$，$\frac{\partial f}{\partial x}$，$z_x$ 或 $f_x(x, y)$，其定义为：
$$
 f_x(x, y) = \lim_{\triangle x \to 0}\frac{f(x + \triangle x, y) - f(x, y)}{\triangle x}
$$
### 微分

如果函数 $z = f(x, y)$，在 $(x, y)$点的 **全增量** 
$$
\triangle z = f(x + \triangle x, y + \triangle y) - f(x, y)
$$
可表示为
$$
\triangle z = A \triangle x + B \triangle y + o(\rho) \quad (\rho = \sqrt{(\triangle x)^2 + (\triangle y)^2})
$$ 其中 $A, B$ 不依赖于 $\triangle x, \triangle y$，而仅与 $x_0, y_0$ 有关，则称函数 $z = f(x, y)$，在 $(x, y)$点「可微分」，
而称 $A \triangle x + B \triangle y$ 为函数 $z = f(x, y)$，在 $(x, y)$点的「全微分」，记做 $\mathrm{d}z$，即 $\mathrm{d}z = A \triangle x + B \triangle y$。

#### 全微分 与 偏导数 的关系

##### 必要条件
如果函数 $z = f(x, y)$，在 $(x, y)$ 点 **可微分**，则函数在该点的偏导数 $\frac{\partial z}{\partial x}, \frac{\partial z}{\partial y}$ **必定存在**，且函数 $z = f(x, y)$，在 $(x, y)$点的**全微分**为
$$
\mathrm{d}z = \frac{\partial z}{\partial x} \triangle x + \frac{\partial z}{\partial y} \triangle y = \frac{\partial z}{\partial x} \mathrm{d} x + \frac{\partial z}{\partial y} \mathrm{d} y
$$

##### 充分条件
如果函数 $z = f(x, y)$ 的偏导数 $\frac{\partial z}{\partial x}, \frac{\partial z}{\partial y}$ 在点 $(x, y)$ **连续**，则函数在该点**可微分**。

##### 近似等式
如果函数 $z = f(x, y)$，在 $(x, y)$ 点 的两个偏导数 $f_x(x, y)$ 和 $f_y(x, y)$ 都连续，并且 $|\triangle x|$ 和 $|\triangle y|$ 都较小时，有近似等式
$$
\triangle z \approx \mathrm{d} z = f_x(x, y) \triangle x + f_y(x, y) \triangle y
$$
即
$$
f(x + \triangle x, y + \triangle y) \approx f(x, y) + f_x(x, y) \triangle x + f_y(x, y) \triangle y
$$

