---
output:
  html_document: default
---
# **Macro data CSI300**

<!-- adding in the paper -->

|频率|变量和指标名称|变量和指标简称[^1]|处理方法|参考文献|数据来源|
|----|:--------:|:-------:|----------|--------------------------|:-----:|
|||**1.宏观层面数据**<br> |
|月度|中国经济政策不确定性指数| d_cn_epu| 1阶差分并滞后1阶|Liu L, Zhang T, 2015. Economic policy uncertainty and stock market Volatility[J]. Finance Research Letters, 15: 99--105. <br> Gong X, Zhang W, Xu W, 等, 2022. Uncertainty index and stock volatility prediction: evidence from international markets[J]. Financial Innovation, 8(1): 57.|[Economic Policy Uncertainty](https://www.policyuncertainty.com/global_monthly.html "https://www.policyuncertainty.com/global_monthly.html")|
|月度|货币供应量M1|d_m1|1阶差分并滞后1阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|[国家统计局](https://data.stats.gov.cn/easyquery.htm?cn=A01 "https://data.stats.gov.cn/easyquery.htm?cn=A01")|
|日度|上证国债指数历史数据|d_SSE_Treasury|1阶差分并滞后1-5阶|Paye B S, 2012. ‘Déjà vol’: Predictive regressions for aggregate stock market volatility using macroeconomic Variables[J]. Journal of Financial Economics, 106(3): 527–546.[^2]|wind数据库|
|||**2.投资者情绪与关注度**<br> |
|月度|投资者情绪|d_CICSI|1阶差分并滞后1阶|Deng S, Xiao C, Zhu Y, et al., 2022. Dynamic forecasting of the Shanghai Stock Exchange index movement using multiple types of investor Sentiment[J]. Applied Soft Computing, 125: 109132.|国泰安数据库|
|日度|卖方推荐指数|seller_recommand_index|滞后1-5阶|戴方哲, 尹力博, 2017. 证券分析师“变脸”行为会增加股票特质波动率吗?[J]. 管理评论, 29(5): 14-22+130.|wind数据库|
|日度|百度指数|bdi|滞后1-7阶|González-Fernández M, González-Velasco C, 2020. A sentiment index to measure sovereign risk using Google Data[J]. International Review of Economics & Finance, 69: 406–418. <br> 李星毅, 刘彦初, 朱书尚, 2023. 利用互联网搜索关注度预测期权隐含波动率变动：基于人工神经网络的分析[J]. 系统工程理论与实践, : 1–20.[^3]|[百度指数](https://index.baidu.com/v2/index.html#/ "https://index.baidu.com/v2/index.html#/")|
|日度|中国隐含波动率指数CIMV|df_vix|滞后1-22阶|Bekaert G, Hoerova M, 2014. The VIX, the variance premium and stock market Volatility[J]. Journal of Econometrics, 183(2): 181–192.|[清华五道口金融科技研究院](http://xyfintech.pbcsf.tsinghua.edu.cn/info/1014/1116.htm "http://xyfintech.pbcsf.tsinghua.edu.cn/info/1014/1116.htm")|
|||**3.股票交易和财务相关数据**|
|月度|换手率|d_turn|1阶差分并滞后1阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|wind数据库|
|日度|板块资金流入强度|inflow_intensity|滞后1-5阶|-|wind数据库|
|日度|市盈率|pe|滞后1-5阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|wind数据库|
|日度|交易量|volume|滞后1-5阶|-|wind数据库|
|日度|封闭式基金折价率|d_discount|1阶差分并滞后1-5阶|-|wind数据库|
|日度|股息率|d_dividend_yield|1阶差分并滞后1-5阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|wind数据库|
|||**4. 相关股票指数**|
|日度|富时中国A50指数|FTSE|取对数收益率并滞后1-22阶|-|[英为财情](https://cn.investing.com/indices/ftse-china-a50 "https://cn.investing.com/indices/ftse-china-a50")|


[^1]: 在代码中的简称
[^2]: 原文说的是具有格兰杰因果关系。Granger causes of volatility
[^3]: 百度指数的合成主要参考这两篇文章的方法，这种合成形式和其他大部分文章**不一样的点**：一是较多的文章使用宏观经济或者热点等关键词，而我们使用的是投资者对股票简称的关键词，是一种关注度的研究；二是使用股票简称的文章通常对百度指数或其他指数合成是简单地加权平均，较少地介绍到不一样的方法，而我们的方法参考使用对过去样本进行正态化处理有再进行加权。


<!-- not in the paper -->
|频率|变量和指标名称|参考文献|数据来源|
|----|:--------:|--------------------------------|:-----:|
|daily|S&P500 Index (USA), Nikkei225 Index (Japan), FTSE100 Index (UK), CAC40 Index (France) and DAX Index (Germany)|Anonymous, 2023. Cross-market information transmission and stock market volatility Prediction[J]. The North American Journal of Economics and Finance, 68: 101977.|CSMAR database|

