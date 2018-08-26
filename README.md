# Basketball Reference Crawler

To crawl a full season you need to use match_generator script. 
```
  python match_generator.py --league nba --seasons 2003-2004
  python match_generator.py --league nba --seasons 2003-to-2015 (will crawl every season from 2003 to 2015)
  python match_generator.py --league ncaa --seasons 2006-2007 2007-2008
```  

Individual matches are represented as a json in which every information from basketball-reference is scraped, including essential information for safely identifying players


## 其他说明：

* 机器学习需要从建立模型开始，这些模型通过历史数据计算各属性权重与属性之间的关系，进而通过这些模型预测结果。需要了解你想要预测的运动，知道哪些变量可以影响预测结果，进而建立一个可以包含这些信息的数据库，最后运行机器学习算法分析历史数据从而计算这些变量的权重。
* 这里已经建立了NBA与NCAA的爬虫，这个爬虫可以下载NBA与NCAA全赛季的的比赛。
* 抓取篮球比赛中表现优秀的球员，并将信息用复杂的json格式表示出来：https://github.com/haochuang/basketball-analytics

* 先具备爬虫数据，才能进行数据分析。
* 用SQLAlchemy编写模型，可以建立数据库并建立分析系统：https://github.com/haochuang/basketball-analytics
* 后续再来优化和补充.TBD...
