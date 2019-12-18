# Matplotlib学习笔记

## 一. 基础知识

### 散点图

通过散点图探究数据之间的相关问题（正相关，负相关，不相关）

```python
import numpy as np
import matplotlib.pyplot as plt
N = 1000
x = np.random.randn(N)
y = np.random.randn(N)
plt.scatter(x, y, c="r", marker="o", alpha=0.5)
plt.show()
```

scatter(x ,y, s, c, market)函数详解

| 参数   | 解释                                |
| ------ | ----------------------------------- |
| x      | array_like                          |
| y      | array_like                          |
| s      | 点的面积，                          |
| c      | 点的颜色                            |
| marker | 点的形状（在官方文档搜索"markers"） |
| alpha  | 点的透明度（0-1，重叠的点颜色加深） |

### 折线图

通过折线图观察数据的变化趋势

