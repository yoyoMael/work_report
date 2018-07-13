#周一
>- 看完了一篇厉害的综述[^comprehensivesurvey]
>- 看了一下python多进程，没能用上

[^comprehensivesurvey]: A comprehensive survey on machine learning for networking: evolution, applications and research opportunities

**计划：**

- 在文献中寻找可用数据集和合适的算法，拟用Xgboost，因为目前还没人用过。 

#周二
>- 整理了一下文献，下到了能用的[数据][MAWI]
>- 决定先从2005 Moore[^moorenb]的论文开始做实验
>- 用[sklearn][sklearn]完成了GaussianNB的训练
>- 简单试了一下，发现用前4个特征效果更好[^discriminators]？

**计划：**

- 对NB算法做特征工程，先实现加n减r方法，之后利用MAWI数据开始其他算法的实验

[MAWI]: http://mawi.wide.ad.jp/mawi/
[sklearn]: http://scikit-learn.org/stable/

[^moorenb]: Internet traffic classification using Bayesian analysis techniques
[^discriminators]: Discriminators for use in flow-based classification

#周三
>- 一波三折实现了加n减r[^nr]，主要是自己死磕了半天排列组合，结果python自带库，[数据][mooredata]大概30万条，程序速度还可以
>- 测试结果用两个特征（0, 82）就得到最佳准确率，可能需要进行全局搜索，再做结论

[^nr]: An SVM-based machine learning method for accurate internet traffic classification

[mooredata]: http://www.cl.cam.ac.uk/research/srg/netos/projects/archive/nprobe/data/papers/sigmetrics/index.html

**计划：**

- 进行一次全局搜索，看结果是否可靠
- 将NB算法改进为NBKE[^moorenb]，或用其他算法进行实验
- 准备处理PCAP数据
- 抽空写一下实验报告

#周四
>- 看了一下画图工具，顺便对库的内容了解了更多
>- 先看[Gradient Tree Boosting][Boostingtree]（GBM，Gradient Boosting Machine；GBRT，Gradient Boosted Regression Tree），再看[XGboost][xgboost][^xgboost]
>- 不想写代码，[MAWI][MAWI]数据太大，还不知道怎么处理，需要看RTC[^RTC]
>- 又跟家里人闹矛盾了，不知道我还能坚持多久

**计划：**

- 以后地铁上看kindle，不看手机了

[^xgboost]: XGBoost: A Scalable Tree Boosting System
[^RTC]: Robust Network Traffic Classification

[Boostingtree]: http://xgboost.readthedocs.io/en/latest/model.html
[xgboost]: http://xgboost.readthedocs.io/en/latest/

#周五
>- 使用XGBoost，在Moore数据集上进行训练，正确率较高
>- 对XGBoost使用加n减r，得到效果最好的特征为5个，但貌似XGboost内嵌了特征选择过程
>- 两次对比说明加n减r并不一定有效，需要使用其他特征工程方法
>- 给[UNB]重发了邮件，等待回复中，成功了就不用操心数据了
>- 简单了解了[Scapy][scapy]解析PCAP文件，不行的话就自己用[QPA][qpa]搞点数据

**计划：**

- 对GaussianNB采用其他特征工程，对比结果
- 如果UNB给数据，就用他们的数据；如果不给，就自己弄数据测试
- 研究XGBoost内嵌特征选择
- 改进一下子串匹配

[unb]: http://www.unb.ca/cic/datasets/index.html
[scapy]: https://scapy.net/
[qpa]: http://protocol.sinaapp.com/