# **Macro data CSI300**

## Have data
<!-- adding in the paper -->

|频率|变量和指标名称|变量和指标简称[^1]|处理方法|参考文献|数据来源|
|----|:--------:|:-------:|----------|--------------------------|:-----:|
|||**1.宏观层面数据**<br> |
|月度|中国经济政策不确定性指数| d_cn_epu| 1阶差分并滞后1阶|Liu L, Zhang T, 2015. Economic policy uncertainty and stock market Volatility[J]. Finance Research Letters, 15: 99--105. <br> Gong X, Zhang W, Xu W, 等, 2022. Uncertainty index and stock volatility prediction: evidence from international markets[J]. Financial Innovation, 8(1): 57.<br>Anonymous, 2023. Stock market volatility prediction: Evidence from a new bagging Model[J]. International Review of Economics & Finance, 87: 445–456.|[Economic Policy Uncertainty](https://www.policyuncertainty.com/global_monthly.html "https://www.policyuncertainty.com/global_monthly.html")|
|月度|货币供应量M1|d_m1|1阶差分并滞后1阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|[国家统计局](https://data.stats.gov.cn/easyquery.htm?cn=A01 "https://data.stats.gov.cn/easyquery.htm?cn=A01")|
|日度|上证国债指数历史数据|d_SSE_Treasury|1阶差分并滞后1-5阶|Paye B S, 2012. ‘Déjà vol’: Predictive regressions for aggregate stock market volatility using macroeconomic Variables[J]. Journal of Financial Economics, 106(3): 527–546.[^2]|wind数据库|
|||**2.投资者情绪与关注度**<br> |
|月度|投资者情绪|d_CICSI|1阶差分并滞后1阶|Deng S, Xiao C, Zhu Y, et al., 2022. Dynamic forecasting of the Shanghai Stock Exchange index movement using multiple types of investor Sentiment[J]. Applied Soft Computing, 125: 109132.|国泰安数据库|
|日度|卖方推荐指数|seller_recommand_index|滞后1-5阶|戴方哲, 尹力博, 2017. 证券分析师“变脸”行为会增加股票特质波动率吗?[J]. 管理评论, 29(5): 14-22+130.|wind数据库|
|日度|百度指数|bdi|滞后1-7阶|González-Fernández M, González-Velasco C, 2020. A sentiment index to measure sovereign risk using Google Data[J]. International Review of Economics & Finance, 69: 406–418. <br> 李星毅, 刘彦初, 朱书尚, 2023. 利用互联网搜索关注度预测期权隐含波动率变动：基于人工神经网络的分析[J]. 系统工程理论与实践, : 1–20.[^3]|[百度指数](https://index.baidu.com/v2/index.html#/ "https://index.baidu.com/v2/index.html#/")|
|日度|中国隐含波动率指数CIMV|df_vix|滞后1-22阶|Bekaert G, Hoerova M, 2014. The VIX, the variance premium and stock market Volatility[J]. Journal of Econometrics, 183(2): 181–192.|[清华五道口金融科技研究院](http://xyfintech.pbcsf.tsinghua.edu.cn/info/1014/1116.htm "http://xyfintech.pbcsf.tsinghua.edu.cn/info/1014/1116.htm")|
|||**3.股票交易和财务相关数据**<br> |
|月度|换手率|d_turn|1阶差分并滞后1阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|wind数据库|
|日度|板块资金流入强度|inflow_intensity<br>d_dividend_yield|滞后1-5阶<br>1阶差分并滞后1-5阶|-|wind数据库|
|日度|市盈率<br>股息率|pe|滞后1-5阶|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|wind数据库|
|日度|交易量|volume|滞后1-5阶|-|wind数据库|
|日度|封闭式基金折价率|d_discount|1阶差分并滞后1-5阶|-|wind数据库|
|||**4. 相关股票指数**<br> |
|日度|富时中国A50指数|FTSE|取对数收益率并滞后1-22阶|-|[英为财情](https://cn.investing.com/indices/ftse-china-a50 "https://cn.investing.com/indices/ftse-china-a50")|


[^1]: 在代码中的简称
[^2]: 原文说的是具有格兰杰因果关系。Granger causes of volatility
[^3]: 百度指数的合成主要参考这两篇文章的方法，这种合成形式和其他大部分文章**不一样的点**：一是较多的文章使用宏观经济或者热点等关键词，而我们使用的是投资者对股票简称的关键词，是一种关注度的研究；二是使用股票简称的文章通常对百度指数或其他指数合成是简单地加权平均，较少地介绍到不一样的方法，而我们的方法参考使用对过去样本进行正态化处理有再进行加权。

## No data
<!-- not in the paper -->
|频率|变量和指标名称|参考文献|数据来源|
|----|:--------------:|--------------------------------|:-----:|
|||**1.宏观层面数据**<br> |
|月度|M0,M1,M2增长率，通货膨胀率|郑振龙, 杨玉晓, 陈蓉, 2023. “好”“坏”方差与股票市场收益率预测[J]. 厦门大学学报(哲学社会科学版), 73(3): 54–66.|中国人民银行，国家统计局|
|||**2.投资者情绪与关注度**<br> |
|日度|“雪球关注度”指标的数据|孙书娜, 孙谦, 2018. 投资者关注和股市表现——基于雪球关注度的研究[J]. 管理科学学报, 21(6): 60–71.|[雪球网](http://www.xueqiu.com "http://www.xueqiu.com")|
|-|*网络沟通质量，股价同步性指标*[^4]，分析师相对乐观度，分析师相对推荐度，分析师相对预测数量分析师相对预测准确度|潜力, 龚之晨, 2021. 网络沟通对股票市场的影响——基于投资者有限关注视角的研究[J]. 金融论坛, 26(2): 47–58.|[雪球网](http://www.xueqiu.com "http://www.xueqiu.com")，WIND 数据库及国泰安数据库|
|-|股吧论坛投资者关注度、雪球网投资者关注度、新闻关注度和新闻情绪指数|石勇, 唐静, 郭琨, 2017. 社交媒体投资者关注、投资者情绪对中国股票市场的影响[J]. 中央财经大学学报, (7): 45–53.|[优矿金融量化平台](https://uqer.io/home "https://uqer.io/home")|
|daily|Microblogging sentiment and attention indicators[^5] (Bullish Ratio, Bearish Ratio, Bullishness Index, Variation, Agreement)|Anonymous, 2017. The impact of microblogging data for stock market prediction: Using Twitter to predict returns, volatility, trading volume and survey sentiment Indices[J]. Expert Systems with Applications, 73: 125–144.|[Twitter REST API](https://dev.twitter.com/docs/api "https://dev.twitter.com/docs/api")|
|||**3.股票交易和财务相关数据** <br> |
|daily|**every 1-min data of the SSEC Index** <br> (the open price, the high priceand low price,the close price, trading volumes and the valueof transactions)<br> $\to$ ***CS liquidity***|Anonymous, 2024. Liquidity and realized volatility prediction in Chinese stock market: A time-varying transitional dynamic Perspective[J]. International Review of Economics & Finance, 89: 543–560.|the China Center for Economic Research (CCER) high-frequency database|
|-|资产规模，账面市值比，资产负债率，换手率，成交量，净资产收益率，固定资产增长率|潜力, 龚之晨, 2021. 网络沟通对股票市场的影响——基于投资者有限关注视角的研究[J]. 金融论坛, 26(2): 47–58.|WIND 数据库及国泰安数据库|
|-|Momentum Factor, Portfolios formed on size, 10 Industry Portfolios|Anonymous, 2017. The impact of microblogging data for stock market prediction: Using Twitter to predict returns, volatility, trading volume and survey sentiment Indices[J]. Expert Systems with Applications, 73: 125–144.|Datastream|
|||**4. 相关股票指数**<br> |
|daily|S&P500 Index (USA), Nikkei225 Index (Japan), FTSE100 Index (UK), CAC40 Index (France) and DAX Index (Germany)|Anonymous, 2023. Cross-market information transmission and stock market volatility Prediction[J]. The North American Journal of Economics and Finance, 68: 101977.|CSMAR database|


[^4]: 不是数据库直接获得
[^5]: 研究美国股市
