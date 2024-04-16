### 1. 运用相关库获取上市公司A的股票基本数据、计算相应的衍生变量数据、通过相关性分析选取合适的衍生变量、可视化呈现数据、并生成Excel工作簿。
1) 运用 Tushare 库获取上市公司 A 从 2023-01-01 至 2023-03-31 的股价变化`price_change`和成交量`volume`数据。
2) 根据以下两种方法计算从 2023-01-01 至 2023-03-31 的成交量涨跌幅：
  - a) 采用当日交易量和昨日交易量的方法
  - b) 采用当日交易量和多日交易量的平均值的方法
3) 通过皮尔逊相关系数分别进行两种成交量涨跌幅与股价变化的相关性分析，并选择出更优的成交量涨跌幅。
4) 在进行简单数据优化后，绘制成交量涨跌幅与股价变化的可视化图表（2个Y轴的形式）。
5) 运用 `xlwings` 库将优化后的数据以及可视化图表导出至 Excel 工作簿。

### 2. 运用相关库从搜狗资讯（https://news.sogou.com/china.shtml） 获取上市公司A的网页源代码，提取相应的标题、网址、来源和发布日期信息，进行简单的数据清洗，并生成文本文件。
1) 运用 `requests` 库从搜狗资讯中获取上市公司 A 的第 1 页网页源代码。
2) 编写正则表达式获取新闻标题、网址、 来源和发布日期信息。
3) 对获取的新闻信息进行简单的数据清洗。
4) 尝试从搜狗资讯中获取上市公司 A 的前 3 页网页源代码，同时完成(2)和(3)中的内容（新闻信息的提取和简单数据清洗）。
5) 将(4)中的数据信息保存到一个文本文件中。

### 3. 运用相关库从东方财富网个股股吧（https://so.eastmoney.com/TieZi/s?keyword=） 中获取A公司的网页源代码，提取相应的标题、网址、来源和发布日期等信息，进行简单的数据清洗，并生成文本文件。
1) 运用 `selenium` 库从东方财富个股吧中获取上市公司 A 的第 1 页网页源代码。
2) 编写正则表达式获取新闻标题、网址、 来源和发布日期等信息。
3) 对获取的新闻信息进行简单的数据清洗。
4) 将数据信息保存到一个文本文件中。

### 4. 运用相关库获取上市公司A和深证成指的股票价格数据，分析其基本特征，进行正态性检验，并实施贝叶斯回归。
1) 运用 `Tushare` 库获取 A 公司和深证成指(399001)从 2022-01-01 至 2022-12-31 的股票价格数据(收盘价)。
2) 将 A 公司和深证成指的股票价格数据规范化， 并绘制股票规范化价格数的线图和散点图。
3) 计算 A 公司和深证成指的对数收益率，并进行正态性检验（3种方法选其中2种）。
4) 运用 `pymc3` 库对 A 公司和深证成指的股票价格实施贝叶斯回归（A公司的股票规范化价格为 x 值，上证指数的股票规范化价格为 y 值），输出统计结果，并绘制后验分布及轨迹图，和贝叶斯回归线。
