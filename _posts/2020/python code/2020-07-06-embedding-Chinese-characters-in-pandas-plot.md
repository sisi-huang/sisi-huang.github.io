How to display Chinese characters in a pandas plot?
It is common to use bar chart to visualize the frequency of different categories. I scraped the data from a Chinese job portal: [lagou](https://www.lagou.com/). What I am 
interested is companies' categories for a data analyst in Shanghai. 
```
import numpy as np
import pandas as pd 

# distribution of companies with request for data analyst 
data = np.array([46,16,15,8,5,2,2,2,2,2,1,1,1]) 
ser = pd.Series(data) 
ser.index = np.array(["移动互联网","文娱","数据服务","电商","企业服务",
"教育","游戏","汽车","社交","医疗","通讯电子","广告营销","金融"]) 

# bar plot 
ser.plot("bar")
```

![A bar chart without Chinese characters](/img/bar_plot_without_chinese.png)

It is obvious to find out that all x-labels are not recognized. Therefore,
We have to set up the font in the python, 
the code here only works for macOS users.
```
import matplotlib.pyplot as plt
import matplotlib.font_manager as mfm

font_path = "/System/Library/Fonts/STHeiti Light.ttc"
prop = mfm.FontProperties(fname=font_path)

ax = ser.plot('bar')
plt.title("数据分析师-行业分布",fontproperties=prop)
ax.set_xticklabels(ser.index, fontproperties=prop)
plt.show()

```

![A bar chart with Chinese characters](/img/bar_plot_with_chinese.png)