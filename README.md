# COVID-19-Literature-Q&A
## 背景 - Background

> 为了应对 COVID-19 大流行，美国开源了COVID-19 开放研究数据集 (CORD-19)，它共包含超过 1,000,000 篇学术文章，其中包括超过 350,000 篇关于 COVID-19、SARS-CoV-2 和相关冠状病毒的全文。 CORD-19 数据集代表了迄今为止可用于数据挖掘的最广泛的冠状病毒文献集合。这使全球 AI 研究社区有机会应用文本和数据挖掘方法来找到问题的答案，以支持全球正在进行的 COVID-19 响应工作。
>
> 数据集的任务部分提供了最初的关键问题的列表。这些关键科学问题来自 NASEM 的 SCIED（国家科学院、工程院和医学院的新兴传染病和 21 世纪健康威胁常设委员会）研究课题和世界卫生组织的 COVID-19 研发蓝图。 其中许多问题都适合文本挖掘，我们鼓励研究人员开发文本挖掘工具来提供对这些问题的见解。 

更多有关该数据集的介绍请参考：[COVID-19 Open Research Dataset Challenge (CORD-19) | Kaggle](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge)

本项目使用2020-2022年发表的文献，不过要改的话代码改一行就行了。

## 环境 - Environment

- python3
- torch = 1.10.0+cu113

## 内容 - Content

尝试使用2个方向解决这个问题，分别是：
- [基于文本表示](https://github.com/Robin-WZQ/COVID-19-Literature-QA/tree/main/Word_Representation)
  - 使用局部哈希算法+biobert词嵌入
- [基于聚类](https://github.com/Robin-WZQ/COVID-19-Literature-QA/tree/main/Clustering)
  - 使用ego-splitting聚类

## 例子 - Example

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

## 参考 - Reference 

https://www.kaggle.com/code/maksimeren/covid-19-literature-clustering

https://www.kaggle.com/code/dgunning/cord-research-engine-search-and-similarity

https://www.kaggle.com/code/mlconsult/summary-page-covid-19-risk-factors

https://www.kaggle.com/code/nadergo/risk-factors-question-answering-biobert

https://www.kaggle.com/code/williamkaiser/using-citations-and-text-content-to-cluster

<!-- https://www.kaggle.com/code/jswxhd/risk-factor-mining-cord-19-articles-2021 （LDA参考的这篇） -->

https://www.kaggle.com/code/davidmezzetti/cord-19-analysis-with-sentence-embeddings/notebook
