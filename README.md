# 项目内容解释

[AprioriAlgorithm.ipynb](./AprioriAlgorithm.ipynb)为使用Apriori算法分析Groceries data的代码，与网页实例教学代码基本一致
，并按作业要求增加了Japan和Iceland的分析。

[FP-growth.ipynb](./FP-growth.ipynb)是老师提供的网页的示例代码。

[FP-onlineRetail.ipynb](./FP-onlineRetail.ipynb)是利用FP-growth算法分析Groceries data的代码，
大体上与Apriori中的代码一致，
但算法函数由使用***apriori()*** 改为使用 ***fpgrowth()***

**！注意！** 为了能顺利在机器上运行 ***（主要是Apriori算法的开销）***，调整了部分国家的 ***min_support*** 参数，包括

1. UK，由0.01调整到0.02
2. Japan，设置为0.11
3. Iceland，设置为0.29

尽管FP-growth算法更为高效，开销更小，但为了做***对照分析***，依然采用了上述的min_support值。

数据集保存在data文件夹，相对代码的路径为:
`./data/Online_Retail.xlsx`



