# 基于XGBoost的新闻网页内容抽取方法数据集

### 数据说明
本数据集用于训练新闻网页内容抽取的机器学习模型，其中的数据来源于以下几个网站的新闻：
- economy.caijing.com.cn
- news.hexun.com
- www.eeo.com.cn
- www.nbd.com.cn
- finance.people.com.cn
- new.qq.com
- finance.sina.com.cn
- money.163.com
- www.xinhuanet.com
- www.yicai.com

##### 具体数据情况

| :Domains: |:Pages:| :Nodes:|:Clean:|:Dirty:|
| --- | --- | --- | --- | --- |
| economy.caijing.com.cn | 102|11782|2060|9722|
|news.hexun.com|103|6074|2162|3912|
|www.eeo.com.cn|102|7166|2437|4729|
|www.nbd.com.cn|146|4873|1651|3222|
|finance.people.com.cn|107|6230|1585|4645|
|new.qq.com|103|2274|2118|156|
|finance.sina.com.cn|108|8332|2497|5835|
|money.163.com|115|19425|2139|17286|
|www.xinhuanet.com|102|5515|750|4765|
|www.yicai.com|105|6423|1962|4461|
|Total|1093|78094|19361|58733|

> Pages是网页的数量，Nodes是数据预处理后得到的html节点数量，Clean是干净的节点数量（包含正文的节点），Dirty是噪声节点数量（不包含正文的节点） 

### 文件说明
- source_html: 存放的是每个网站的原始的HTML文件
- label_content: 存放的是人工标注的HTML对应的新闻内容
- website_data: 数据清洗和特征抽取后的数据集（每个网站的数据存储在不同的csv文件中）
- test_data.csv和train_data.csv：数据清洗和特征抽取后所有网站的混合在一起的数据集


