# COVID-19-Literature-Q&A
针对百万级新冠肺炎文献的检索与问答系统

> 仅学习使用

## Content - 内容

尝试使用3个方向解决这个问题，分别是：
- [基于文本表示](https://github.com/Robin-WZQ/COVID-19-Literature-QA/tree/main/Word_Representation)
  - 使用局部哈希算法+biobert词嵌入
- [基于聚类](https://github.com/Robin-WZQ/COVID-19-Literature-QA/tree/main/Clustering)
  - 使用ego-splitting聚类
- [基于主题建模]()
  - 使用LDA模型(文件太大这里放不下，放到[网盘了](). 提取码:)

## Dataset - 数据集

数据集来源：https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge .

本项目使用2020-2022年发表的文献，不过要改的话代码改一行就行了。

## Example - 例子

**Question**: What do we know about risk factors?

**Answer(Top 10)**:

1. an exposure history , greater age , abnormal radiologic and laboratory findings , and the development of complications

2. existing mental disorders , female sex , and concerns about getting infected were repeatedly reported

3. facility ( public vs private ) , age , gender , duration of illness prior to and / or during hospitalizations

4. the knowledge of the impact of comorbidities on adverse clinical outcomes

5. 30 - day mortality was associated with male sex ( odds ratio 1 ¡¤ 75 [ 95 % ci 1 ¡¤ 28 - 2 ¡¤ 40 ] , p < 0 ¡¤ 0001 ) , age 70 years or older versus younger than 70 years ( 2 ¡¤ 30 [ 1 ¡¤ 65 - 3 ¡¤ 22 ] , p < 0 ¡¤ 0001 )

6. higher troponin , il - 6 and d - dimer values

7. age , insurance , prepregnancy body mass index , and parity

8. our understanding of the association of coronavirus disease 19 ( covid - 19 ) and preterm or early term birth among racially and ethnically diverse populations and those with chronic medical conditions is limited

9. sex , onset month , age group , city of residence

10. there has not been evidence suggesting the link between covid - 19 and asthma exacerbation

## Reference - 参考文件

比较好的资源：

https://www.kaggle.com/code/maksimeren/covid-19-literature-clustering

https://www.kaggle.com/code/dgunning/cord-research-engine-search-and-similarity

https://www.kaggle.com/code/mlconsult/summary-page-covid-19-risk-factors

https://www.kaggle.com/code/nadergo/risk-factors-question-answering-biobert

https://www.kaggle.com/code/williamkaiser/using-citations-and-text-content-to-cluster

https://www.kaggle.com/code/jswxhd/risk-factor-mining-cord-19-articles-2021

https://www.kaggle.com/code/davidmezzetti/cord-19-analysis-with-sentence-embeddings/notebook
