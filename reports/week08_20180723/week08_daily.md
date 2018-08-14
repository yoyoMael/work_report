#周一
>1. 今天就是跑程序啊，太水了
>2. 虽然有点难受，不过还好弄得东西不难，把结果跑出来了，果然状态不好的时候没有动力啊，数据都没好好整理，后续处理可麻烦了
>3. 发现画图还是有点麻烦的

**计划：**

- 整理数据，看看故事怎么讲

#周二
>1. 今天在家休息，实在是不能吹空调
>2. 早上起来看了半小时数据，什么也没想出来，打了一天联盟，不过机会难得，现在不打以后不一定什么时候有机会了，还有4个月回学校，加油干吧

**计划：**

- 画图、分析数据、找创新点

#周三
>1. 画个图折腾了三天，今天终于弄好了，柱状图样式也弄好了
>2. 画完图发现创新点不够什么鬼，还得接着弄
>3. 反复看了几篇用相关数据集的论文，对比一下自己的好像不太行

**计划：**

- 看论文，找创新点，继续实验

#周四

>1. 今天又看了一篇中文[^sxbfeature]，和一篇外文[^gawkelm]，还有挂名Moore的一篇长文[^moorenn]
>2. 发现用ELM的那篇[^gawkelm]其实算法也是照搬别人的，只不过用了GA做参数调整、但没做特征选择。中文的[^sxbfeature]，用了多种特征选择方法做比较，但没有调参，分类器简单。且这三篇都用了port number特征，且流量分类中还没人用过resample
>3. 现在考虑我的论文大致组成为：主要：LightGBM、Resample（SMOTETomek和Simple方法）次要：特征选择、去除prot number
>4. 我只能说我的方法都没有那么高大上，小笔记本跑不动，但是只要证明方法的有效性就可以
>5. 不知道SMOTETomek那么难跑，下午2点就把电脑跑没电了，而且还没跑出来，今天就多做些paper阅读吧，说不定可以找到支持我的方法东西
>6. 今天还把数据指标完善了，之前的指标单一、不符合主流标准，现在可以了，有时间再跑跑程序

**计划：**

- 把SMOTETomek数据保存下来，做对比实验，看看结果，好的话可以给老师看了
- 还是不能太着急，但是要有紧迫感
- 特征选择方面，用增l减r方法做出来的结果与XGBoost分析的重要性顺序有些不同，要么讲故事，要么再跑两次，感觉要跑的东西太多，时间都不够用了呢，好想有个助手来给我弄

[^sxbfeature]: 2017 面向多类不均衡网络流量的特征选择方法
[^gawkelm]: 2017 A new approach for internet traffic classification: GA-WK-ELM
[^moorenn]: 2017 Network traffic classificationvia neural networks

#周五

>1. 今天疯狂跑程序啊，电脑又是半天就没电了，这几天辛苦的不是我，是我的Macbook，第一次突然黑了，以后要好好爱护，毕竟离我能买的起新的还有好长时间。。。
>2. 还好找到突破口了，用SMOTETomek和ROS还有原始数据训练LGBM作对比，嗯。。。，发现了SMOTETomek的效果比较好，接下来要继续对多个分类器作对比，用来迷惑敌人
>3. 这次采集的指标可以说很全面了，一定要好好弄，真的要给老师看一下了，从结果上看，这下真的有戏了，不是像之前只是设想的很好
>4. 事实证明我的特征选择并没有什么优越性，所以干脆就用10个特征来做，不然别人还要嫌我的方法太捞，特征选择什么的，就随他去吧哈哈哈
>5. 今天真不错，看了几篇论文[^wycnn]，特别是一篇瑞士的硕士论文[^videotraffic]，又找到了可以完善的地方

**计划：**

- 之后可以考虑用序列浮动特征选择来做特征，但是这玩意电脑玩不动啊，我这私人渣配置电脑可舍不得弄这个，回学校找老师申请高配，嘿嘿嘿
- 这个做完先闲一下，随便看看文献什么的，后续可以收集点数据，到时候再来一篇，嘿嘿嘿，这样下学期说不定还可以接着去实习，稳稳的
- 接下来要做的是完善树结构的选择工作，论文大概这样就算成型了


[^videotraffic]: 2017 An Evaluation of Video Traffic Classification using Random Forests and Gradient Boosted Trees
[^wycnn]: 基于深度卷积神经网络的网络流量分类方法