## 谷歌搜索引擎命令整理


---



### 搜索命令清单

| 命令 | 行为  | 例子|
| --- | --- | --- |
|link:URL | 列出到链接到目标URL的网页清单. | link:http://www.sina.com.cn/|
|related:URL | 列出于目标URL地址有关的网页. |related:http://www.sina.com.cn/ |
|inanchor:WORD | 搜索页面锚链接中包含关键字的网页. |inanchor:golang |
|site:Domain |搜索区域仅限于目标网站.|xueyuanpai site:baidu.com|
|allinurl:WORDS | 只显示在URL地址里有搜索结果的页面.多词用空格隔开|allinurl:xueyuanpai html |
|inurl:WORD | 跟allinurl类似,但是只在URL中搜索第一个词.| inurl:xueyuanpai|
|allintitle:WORD | 搜索网页标题.|allintitle:xueyuanpai html|
|intitle:WORD | 跟allintitle类似,但是只在标题里搜索第一个词.|intitle:xueyuanpai |
|cache:URL | 将显示关于URL的Google缓存(中国不可用).| cache:http://www.sina.com.cn/|
|info:URL | 将显示一个包含了这些元素的页面:类似结果的链接,反向链接,还有包括了这个URL的页面.在搜索框里直接输入URL会起到同样的效果.| info:http://www.sina.com.cn/|
|filetype:SOMEFILETYPE | 指定文件类型.|filetype:pdf  golang|
|-filetype:SOMEFILETYPE | 剔除指定文件类型.|-filetype:pdf  golang|
|allintext: | 搜索文本,但不包括网页标题和链接|allintext:xueyuanpai|
|allinlinks: | 搜索链接, 不包括文本和标题|allinlinks:http://www.sina.com.cn/|
|WordA OR WordB | 搜索包含两关键词之一的页面| xueyuanpai OR 学院派|
|“Word” OR “Phrase” | 精确的要求搜索单词或者句子| "xueyuanpai" OR "学院派"|
|WordA -WordB | 包含单词A但是不包含单词B| xueyuanpai  -学院派|
|WordA +WordB | 都包含| xueyuanpai  +学院派 | 
|~WORD | 寻找此单词和它的同义词| ~xueyuanpai | 
|~WORD-WORD | 只搜索同义词,不要原词| ~xueyuanpai -xueyuanpai | 
|WORD*WORD | 模糊搜索，*号代表任何词| xue*pai |
|time1..time2 | 只显示从time1到time2时间段内的内容| golang 2018..2019 |


### 来源
[https://www.zhihu.com/question/20161362]()

[http://blog.csdn.net/wei18359100306/article/details/50109203]()



> ##### 以上命令可混合使用使查找更精确。“link”不能与其他语法相混合操作，所以“link:”后面即使有空格，也将被GOOGLE忽略


百度也支持减号、site、inurl、intitle、filetype等命令