# Chapter 2

第二章用房价预测的例子，完整的介绍了一个机器学习项目的流程。特别的，它注重对于数据的认识，对于特征工程的重视，虽然例子简单，但有很多总结、经验值得学习。

一个项目的主要流程:

- 项目概述

- 数据获取

- 探索数据、可视化数据，发现规律

- 数据预处理

- 选择模型、训练模型

- 模型微调

- 给出解决方案

- 部署、监控、维护系统

## 项目概述

包括设计解决问题的架构，选择评价指标，检查确认一些假设等等。

## 数据获取

获取所需数据。

对数据有一个快速的了解，比如数据的组成、结构、特征数目、样例数目、数据缺失情况、数据大致分布情况等等。

一个重要的提醒：在对数据进一步探索、处理前，我们要创建一个测试集，并且确保不再触碰它。这里对于创建测试集，还有一些思考：随机创建并不是可靠的，因为多次运行之后，我们的机器学习算法可能会得到全部的数据集；这可以通过保存测试集、设定随机数生成器的种子、使用样本实例示例的识别码等方法改善或解决。

另外，如有必要，需要进行分层采样。

## 探索数据、可视化数据，发现规律

对数据进行可视化，可以帮助我们直观的发现一些规律。

对于合适大小的数据集，可以查看特征之间的相关情况。

对于特征进行组合实验，可能会发现更为有效的特征。

## 数据预处理

缺失值处理：去掉对应样本实例、去掉整个特征、赋值（0、均值、中值等等）

文本标签的数字化处理：直接映射、onehot编码等等

特征缩放，解决特征量度差别过大的问题：归一化、标准化等

使用`scikit-learn`的`Pipeline`功能，更加方便、快速的处理问题，尽可能多的实现自动化。

## 选择模型、训练模型

数据预处理做好之后，模型训练反而更为简单。可以选择不同的模型，了解下大致效果。可以在训练集上进行交叉验证。

## 模型微调

手动经验调参、网格调参、随机搜索

集成模型提高准确率

分析模型、误差

在测试集上进行评测

## 部署、监控、维护系统




