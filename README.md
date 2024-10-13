轴承故障预测数据：
# 轴承有3种故障：
外圈故障，内圈故障，滚珠故障，外加正常的工作状态。如表1所示，结合轴承的3种直径（直径1,直径2,直径3），轴承的工作状态有10类
因此可以将问题转为分类。

# 数据说明
1.train.csv，训练集数据，1到6000为按时间序列连续采样的振动信号数值，每行数据是一个样本，共792条数据，第一列id字段为样本编号，最后一列label字段为标签数据，即轴承的工作状态，用数字0到9表示。

2.test_data.csv，测试集数据，共528条数据，除无label字段外，其他字段同训练集。

总的来说，每行数据除去id和label后是轴承一段时间的振动信号数据，需要用这些振动信号去判定轴承的工作状态label。

# 预测结果
可对故障种类达到100%的预测准确率。
