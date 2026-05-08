先下载， pip install matplotlib

一些常见图表：

| 目标    | 方法                           |
| ----- | ---------------------------- |
| 折线图   | `ax.plot(x, y)`              |
| 散点图   | `ax.scatter(x, y)`           |
| 柱状图   | `ax.bar(categories, values)` |
| 直方图   | `ax.hist(data, bins=10)`     |
| 标题    | `ax.set_title("Title")`      |
| x 轴标签 | `ax.set_xlabel("X")`         |
| y 轴标签 | `ax.set_ylabel("Y")`         |
| 图例    | `ax.legend()`                |
| 网格    | `ax.grid(True)`              |
| 保存    | `fig.savefig("file.png")`    |

numpy是numerical python

```
#柱状图
import matplotlib.pyplot as plt 
import numpy as np 
x = np.linspace(0, 10, 200) 
y = np.sin(x) 
fig, ax = plt.subplots(figsize=(4, 3)) 
ax.plot(x, y, linewidth=2) 
ax.set_xlabel("Time (s)") 
ax.set_ylabel("Signal") 
ax.set_title("Sine wave") 
plt.show()
```

```
#折线图
import matplotlib.pyplot as plt  
import numpy as np  
  
categories = ["a","b","c","d","e"]  
values = [1,2,3,4,5]  
  
fig,ax = plt.subplots(figsize=(5,5))  
ax.bar(categories,values)  
  
ax.set_xlabel("x")  
ax.set_ylabel("y")  
ax.set_title("title")  
  
plt.show()
```

```
#散点图
import matplotlib.pyplot as plt  
import numpy as np  
  
x = np.random.rand(50)  
y = np.random.rand(50)  
  
fig,ax = plt.subplots(figsize=(5,5))  
  
ax.scatter(x,y)  
  
ax.set_xlabel("x")  
ax.set_ylabel("y")  
ax.set_title("title")  
  
plt.show()
```

