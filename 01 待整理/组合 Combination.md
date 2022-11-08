
## 组合

组合 和 排列的区别是，组合不考虑顺序。

因此，以 5 个元素 取 3 个元素 为例，可以这样考虑：
1. 首先，和排列一样“考虑重复”地进行比较
2. 除去 重复度，排除重复技术的部分
	1. 取 3 张牌，每一种 组合，都对应了 $P_3^3$ 种排列

因此，可以得出：
$$ C_n^k = \frac{P_n^k}{P_k^k} = \frac{n!}{(n-k)!k!} $$

## 代码实现

- 依赖函数：[[排列 Permutation]]

```python
def combination(_n: int, _k: int):  
    if _n < 0 or _k < 0:  
        raise ValueError("n and k must be positive")  
    if _n < _k:  
        raise ValueError("k must equal or less than n")  
    if _n == 0 or _k == 0:  
        return 1  
    return permutation(_n, _k) // permutation(_k, _k)
```
