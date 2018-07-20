# 周一
>1. 下载了UNB的数据，找到了一个解析PCAP的工具，看了Tor[^tor]数据的论文
>2. 实现了xgboost的特征比较，得到两张图

**计划：**

- 对unb数据进行训练，看看效果
- 看一下VPN[^vpn]数据的论文
- 看有关ISCX数据的论文
- 进一步进行特征比较

[^tor]: 2017 Characterization of Tor Traffic using Time based Features

# 周二
>1. 今天没干啥，随便看了点文献，又下了好多，一天就这么过去了，没有什么方向，准备开始刷paper了，心无旁骛，就是干！

**计划：**

- 文献整理的还是不够精细，要把发表年份加到开头方便查找，写个脚本来改名吧，顺便复习一下，工欲善其事，必先利其器，这不光是做一个效率工具，也是磨炼一下技能，而且对以后工作肯定有用

# 周三

>1. 完成了论文日期修改工具
>2. 看了三篇中文论文，其中有一篇感觉比较水[^a]，另一篇没看懂在干啥，感觉也没啥用[^c]，最后一篇现在没条件做，下学期倒是可以考虑搞分布式[^b]
>3. 某外文论文看了一半[^elm]，2017年的，用的Moore set， 或许我也可以用，然后再用ISCX set[^vpn]，至少能出一篇论文，美滋滋
>4. 除了XGBoost之外，又发现了[lightGBM][lightgbm][^lightgbm]，2017年才出的算法，我只能说NB，这口肉我要先吃了，看老师的意见吧

**计划：**

- 感觉前三天就这么划水过去了，明天下午之前一定要开始下个实验了，争取周五做完，继续看论文
- 看老师意见，准备朝论文的方向走了，XGBoost，lightGBM，换个数据集打一套
- 看一下[Kaggle][kaggle]的教程，磨炼一下基础技能
- 统计学可能没那么多时间学了，有需要的地方就看一下吧，维基百科上的词条我都看不懂
- 用Jupyter Notebook写一下实验报告，这两周光吃饭了。。。
- 赶快搞一篇论文出来吧，这样就可以接着搞序列挖掘了

[^a]: 2018 基于深度卷积神经网络的网络流量分类方法
[^b]: 2016 基于 Spark 的大规模网络流量准实时分类方法
[^c]: 2016 基于行为特征学习的互联网流量分类方法
[^elm]: 2017 A new approach for internet traffic classification GA-WK-ELM
[^vpn]: 2016 Characterization of Encrypted and VPN Traffic Using Time-Related Features
[^lightgbm]: 2017 LightGBM: A Highly Efficient Gradient Boosting Decision Tree

[kaggle]: https://www.kaggle.com/
[lightgbm]: http://lightgbm.readthedocs.io/en/latest/

# 周四

>1. 最近效率奇低啊，又划水了，就到处瞎看了点东西（3.5小时）
>2. kaggle教程没看，又发现了kernel这个新坑
>3. 对Moore数据又有新理解，首先最重要的特征是1号，就是服务器端口，这其实是不合理的，因为端口本来就相对稳定，其次WWW的数据比例太大了，这些都是需要考虑的问题
>4. lightGBM安装失败了，感觉我的Macbook需要重置了。。。（2小时）
>5. 发现了一个[随机森林调参方法][randomforesttune]，标记一下，这个帖子里还是有些东西值得深究的
>6. 时间过得太快，而我走的太慢，今天又这样结束了，这周没有任何进展
>7. 感觉方向又不明确了，需要接着问老师
>8. 还好今天又跑了一下XGBoost， 有了点新结果，实在用不了LightGBM，就先用它了（2小时）

**计划：**

- 装好lightGBM
- 看kaggle教程和kernel
- 看论文，多做实验，感觉差不多能写论文了，这周马上结束，抓紧时间

[randomforesttune]: http://sofasofa.io/forum_main_post.php?postid=1000868

#周五
1. 今天不错，比较实在，复习了一下GBDT，大概了解了LightGBM[^lightgbm]
2. LightGBM自己就好了，我也是醉了
3. 看了一些实际操作的东西

**计划：**

1. 虽然没能按计划开始实验，但是也不错了，要做一次考虑全面，图表丰富的实验了，做完估计就能发表了，准确率什么的不存在的
2. 周六要出去浪啊，记得周日要立马找回状态
3. 接着学ML的知识吧，ML、Python怎么学也学不完，英语也要学，数学也要学，在学飞之前多学点。。。