﻿# 自如聚类分析与可视化
爬取自如所有上海房源，进行k-means聚类分析，将房源划分为不同等级。将对数据进行进一步分析。

---

## 数据

- **全部数据都在data文件夹中。**

![data](pic/data.png)

---

## 聚类后的dataframe结果

![kmeans](pic/housingdata.PNG)

---

## 可视化图表

- 堆叠柱状图

![barchart](pic/barchart.PNG)

- 饼图

![piechart](pic/浦东不同类别房源.png)

- 3D柱状图

![3d](pic/3d.PNG)

- 结果
![result](pic/图表分析结果.PNG)

---

# 机器学习部分

## 数据

- 机器学习的数据：用**'metro_num', 'S', 'density', '聚类类别'**预测**每月租金**

![dataset](pic/机器学习数据.PNG)

---

## 线性回归模型

- 训练集上误差约为：**621.4**

![lin](pic/线性回归模型.PNG)

---

## 决策树模型

- 训练集上误差约为：**57.68**，推测为**过拟合**了。

![tree1](pic/决策树1.PNG)

- 使用交叉检验得出误差约为：**577.89**

![tree2](pic/决策树2.PNG)

---

## 随机森林模型

- 训练集上误差约为：**201.6**，推测应该也为**过拟合**了。

![forest1](pic/随机森林1.PNG)

- 使用交叉检验得出误差约为：**479.15**

![forest2](pic/随机森林2.PNG)

### 最优微调模型
- **max_features: 2, n_estimators: 30**时，效果最好，误差为**451.98**

---



