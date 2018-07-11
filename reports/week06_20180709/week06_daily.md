#周一
>- 看完了A comprehensive survey on machine learning for networking: evolution, applications and research opportunities 
>- 看了一下python多进程，没能用上

**计划：**
- 在文献中寻找可用数据集和合适的算法，拟用Xgboost，因为目前还没人用过。 

#周二
>- 整理了一下文献，下到了能用的数据
>- 决定先从2005 Moore的论文开始做实验
>- 用sklearn完成了NB的训练
>- 简单试了一下，发现用前4个特征效果更好？

**计划：**
- 对NB算法做特征工程，先实现加n减r方法，之后利用MAWI数据开始其他算法的实验

#周三
>- 一波三折实现了加n减r，主要是自己死磕了半天排列组合，结果python自带库，数据大概30万条，程序速度还可以
>- 测试结果用两个特征就得到最佳准确率，可能需要进行全局搜索，再做结论

**计划：**
- 进行一次全局搜索，看结果是否可靠
- 将NB算法改进为NBKE，或用其他算法进行实验
- 准备处理PCAP数据
- 抽空写一下实验报告
