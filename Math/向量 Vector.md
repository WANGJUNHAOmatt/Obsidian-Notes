---
aliases: 
tags: 
title: 向量 Vector
date created: Wednesday, August 31st 2022, 4:41:46 pm
date modified: Thursday, September 29th 2022, 11:29:24 pm
---

## 向量的8条公理
> 满足以下 8 条 规则，即可按照向量进行运算。

1. $\vec{u} + (\vec{v} + \vec{w}) = (\vec{u} + \vec{v}) + \vec{w}$
2. $\vec{v}+\vec{w} = \vec{w}+\vec{v}$
3. There is a vector 0 such that $0 + \vec{v} = \vec{v}$ for all $\vec{v}$
4. For every vector $\vec{v}$ there is a vector $-\vec{v}$ so that $\vec{v} + (-\vec{v}) = 0$
5. $a(b\vec{v}) = (ab) \vec{v}$
6. $1 \vec{v} = \vec{v}$
7. $a(\vec{v} + \vec{w}) = a \vec{v} + a \vec{w}$
8. $(a + b) \vec{v} = a \vec{v} + b \vec{v}$

## 向量间的关系

### 垂直

夹角为 $\frac{\pi}{2}$ 的两个向量 互相垂直。

## 向量的运算

### 向量间的运算

#### 投影

向量 $a$ 在轴 $u$ 上的的投影，等于 $a$ 的 模 乘以 向量 $a$ 与 轴 $u$ 的夹角。

$$ \mathrm{Prj}_u \vec{a} = |a| \cos \varphi $$
##### 投影的线性性质

- $\mathrm{Prj}_u(a+b) = \mathrm{Prj}_u a + \mathrm{Prj}_u b$
- $\mathrm{Prj}_u \lambda a = \lambda \mathrm{Prj}_u a$

#### 内积 inner product |数量积、点积

$$ \langle \alpha, \beta \rangle = \sum_{i=1}^{n} \alpha_i \beta_i = \alpha^T \beta = |a||b| \cos \varphi $$

#### 外积 ｜ 向量积、叉积

$$ a \times b = |a| |b| \sin \theta = \begin{vmatrix}
i & j & k \\
a_x & a_y & a_z \\
b_x & b_y & b_z
\end{vmatrix}$$

#### 混合积

$$ [abc] = (a \times b) \cdot c $$


#### 夹角

两个 **非零向量** 之间的 不超过 $\pi$ 的夹角称为向量 $a$ 与 $b$ 的夹角，记作 $(a\hat{,}b)$

##### 方向角

非零向量 $a$ 与 空间直角坐标系的 三个坐标轴的夹角 $\alpha, \beta, \gamma$ 称为向量 $a$ 的 **方向角**。

###### 方向余弦

向量 $a$ 方向角的余弦函数 $\cos \alpha, \cos \beta, \cos \gamma$ 称为 向量 $a$ 的 **方向余弦**

- 方向余弦的平方和为 1

$$ \cos^2 \alpha + \cos^2 \beta + \cos^2 \gamma = 1$$

> 将空间中的任意长度为 1 的向量，拆解成由空间的 基向量 线性组合成的形式，它们的平方和，等于 这个长度为 1 的向量 长度的平方。

### 向量和其他的运算

