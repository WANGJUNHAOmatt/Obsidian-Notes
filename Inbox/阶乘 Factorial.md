---
aliases: 
tags: 
date created: Monday, November 7th 2022, 8:30:16 pm
date modified: Monday, November 7th 2022, 8:35:41 pm
---

## 阶乘

## 代码实现

### 循环实现
```python
def factorial(_x: int) -> int:  
    if _x < 0:  
        raise ValueError  
    if _x == 0:  
        return 1  
    _result = 1  
    while _x:  
        _result *= _x  
        _x -= 1  
    return _result
```

### 递归实现
> 容易触发最大递归深度，对于计算阶乘，并不可取。