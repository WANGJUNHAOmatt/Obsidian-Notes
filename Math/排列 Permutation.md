---
aliases: 
tags: 
title: 排列 Permutation
date created: Monday, July 18th 2022, 3:00:21 pm
date modified: Monday, November 7th 2022, 8:46:38 pm
---
> [!info] 排列的教科书定义 P9
> 把 $n$ 个自然数 $1, 2, \cdots, n$ 排成一列，这称之为 $n$ 个自然数的一个 **全排列**，也称为一个 $\mathbf{n}$**级排列**（简称为**排列**）

> [!cite] Permutation from WikiPedia
> 排列，就是从一个[[集合 Set]]中的元素不重复地组成的序列。

>[!tips] 注意
> 135 也是 {1, 2, 3, 4, 5} 的一个排列。

## 排列


$$ P_{n}^{k} = \frac{n!}{(n-k)!} $$

## 代码实现

- 依赖函数：[[阶乘 Factorial]]

```python
def permutation(_n: int, _k: int) -> int:  
    if _n < 0 or _k < 0:  
        raise ValueError("n and k must be positive")  
    if _n < _k:  
        raise ValueError("k must equal or less than n")  
    if _n == 0 or _k == 0:  
        return 1  
    # 之所以这里使用 // （整除）运算，是因为如果我们使用 /（除法），  
    # python 会求 一个 float 结果，调用的是 cpython 中的 double，只能表示 2^53 的值，无法表示全部的整数。  
    # 参考：https://stackoverflow.com/questions/42709746/how-to-get-the-correct-accuracy-with-big-integer-division-in-python  
    return factorial(_n) // factorial(_n - _k)
```

### 检验

- 依赖函数 `math.perm(n, k)`

```python
def check(x: int) -> bool:  
    for i in range(0, x):  
        for j in range(0, i+1):  
            if perm(i, j) != permutation(i, j):  
                print(f"perm({i}, {j}) = {perm(i, j)} and permutation({i, j}) = {permutation(i, j)}")  
                return False  
    print("check successful!")  
    return True
```

---

created at `$= dv.current().file.ctime`.
last modified at `$= dv.current().file.mtime`.