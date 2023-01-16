#Programing/Python 

## 导入一个模块

### 直接导入一个模块

   ```python
   # import <库名>
   import math
   # import <库名> as 别名
   import pandas as pd
   # <库名>.<函数>([<参数>])
   math.sqrt(x)
   # <库名>.<属性>
   math.pi
   ```

### 导入一个模块的 **所有对象**

   ```python
   >>> from math import *
   >>> sqrt(9)
   3.0
   >>> pi
   3.141592653589793
   ```

### 导入一个模块的 **指定对象**

   ```python
   >>> from math import sqrt, pi
   >>> sqrt(9)
   3.0
   >>> pi
   3.141592653589793
   ```
