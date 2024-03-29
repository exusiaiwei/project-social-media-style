
###  语料库概述
本研究构建的是一个自建的网络语料库，主要用于控制主题和平台。本语料库着重于以下几个方面的数据：

- **平台选择**：选择了B站、贴吧、微博这些大众平台，这些平台使用人数众多，且涵盖多个主题领域。
- **主题分类**：基于政论、文艺、科技、事务的分类法，本研究选择了Film,Gaming,Learning,Literature,Politics,Technology六个领域。总共包含19个典型关键词。



###  语料库所包含的主题和领域

| 领域 | 主题（关键词） | 领域 | 主题（关键词） |
|------|----------------|------|----------------|
| 影视 | 流浪地球       | 科技 | 人工智能（ai） |
|      | 满江红         |      | chatgpt        |
|      | 易烊千玺       | 文学 | 道诡异仙       |
|      |                |      | 东野圭吾       |
|      |                |      | 三体           |
|      |                | 政治 | 彩礼           |
| 游戏 | 明日方舟       |      | 俄亥俄         |
|      | 少女前线       |      | 俄乌战争       |
|      | 星际争霸2      |      | 人口           |
|      | 星穹铁道       |      | 疫情           |
|      | 原神           |      | 航空母舰       |

- 语料库总量：61.2MB
- 总字数：约2100万字

### 语料来源
本研究使用的语料均通过开源爬虫项目或软件从公开平台爬取。具体方法如下：

- **微博语料**：使用开源项目`WeiboSpider-master`进行搜集。
- **贴吧语料**：使用开源项目`Tieba_Spider-master`进行搜集，并进行了一定的修改和配置。
- **B站语料**：使用数据抓取软件`八爪鱼采集器`进行搜集，主要针对视频下方的评论信息。

### 语料清洗和预处理
由于不同的抓取工具和平台特性，我们对语料进行了必要的清洗和预处理，以确保数据的一致性和准确性。具体操作包括：

- **链接移除**：使用Python程序批量删除了语料中的图片链接和表情符号链接。
- **分词处理**：针对中文语料的特点，使用`NLPIR-Parser`软件进行了新词提取和分词处理。

以上是对本研究中使用的语料库的详细介绍。欢迎在GitHub上查看和使用这些数据。
