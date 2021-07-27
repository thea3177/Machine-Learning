# sklearn机器学习 scikit learn

0.1 什么是sklearn? 一个开源的基于python的机器学习工具包,通过numpy,scipy和matplotlib等库实现高效的算法应用,涵盖了几乎所有主流机器学习算法

0.2 sklearn建模基本流程

![sklearn](/Users/yejingwen/Desktop/python/python_bilibili/deep_learning/sklearn/sklearn.png)

```python
from sklearn import tree 							#导入需要的模块

clf = tree.DecisionTreeClassifier		  #实例化
clf = clf.fit(X_train,Y_train) 				#用训练数集训练模型
result = clf.score(x_test,y_test) 		#导入测试集,从接口中调用需要的信息 
```



0.3 课程结构

| 主题                         | 案例 | 设计的模块                      |
| ---------------------------- | ---- | ------------------------------- |
| 决策树                       |      | tree                            |
| 随机森林                     |      | ensemble                        |
| 数据预处理和特征工程         |      | preprocession,feature_selection |
| 主成分分析PCA与奇异值分解SVD |      | decomposition                   |
| 逻辑回归                     |      | linear_model                    |
| 聚类算法与K-Means            |      | cluster                         |
| SVM                          |      | svm                             |
| 线性回归,岭回归与Lasso       |      | linear_model                    |
| XGBoost                      |      | sgboost                         |

1. 决策树

   1. 概述

      1. 决策树是如何工作的

      2. sklearn中的决策树

         | tree.DecisionTreeClassifier | 分类树                       |
         | --------------------------- | ---------------------------- |
         | tree.DecisionTreeRegressor  | 回归树                       |
         | tree.export_graphviz        | 决策树导出到DOT格式,画图专用 |
         | tree.ExtraTreeClassifier    | 高随机版本的分类树           |
         | tree.ExtraTreeRegressor     | 高随机版本的回归树           |

   2. decisionTreeClassifier和红酒数据集

      1. 重要参数
         1. criterion 不纯度
            - 不纯度: 为了将表格转化成一棵树,决策树需要找出最佳节点和最佳的分枝方法,衡量这个“最佳”标准的指标
            - 不纯度越低,决策树对训练集的拟合越好
         2. 
      2. 重要属性和接口

   3. DecisionTreeRegressor

      1. 重要参数,属性及接口
      2. 实例:一维回归的图像绘制

   4. 决策树的优缺点
