# **Text Mining by Clustering**


## 使用说明 - Usage

1. 安装环境

```
pip install -r requirements.txt
```

特别的，除了常规第三方库外，需要说明biobert_embedding这个库：

首先正常pip install biobert-embedding，由于该库在使用时会首先下载放在google drive上的预训练模型文件（通过request这个库下载），但是由于网络原因下载不下来。因此需要首先挂梯子，在[biobert_v1.1_pubmed_pytorch_model.tar.gz (dropbox.com)](https://www.dropbox.com/s/hvsemunmv0htmdk/biobert_v1.1_pubmed_pytorch_model.tar.gz?dl=0) 中下载所有文件至目录biobert_v1.1_pubmed_pytorch_model/中，之后注释掉../site-packages/biobert_embedding/downloader.py中第44-75行的内容即可。

2. 下载相关文件

我放到百度网盘了, https://pan.baidu.com/s/1LLQtVqnGtKfMKIoaqKyr1Q ,提取码: dlmd

保证最终的目录如下所示：

```
| pic2 # ipynb里面的图片
| -----1.png
| -----2.png
| biobert_v1.1_pubmed_pytorch_model # biobert模型文件
| -----config.json
| -----pytorch_model.bin
| -----vocab.txt
| pdf_json # 带标注的文献全文
metadata.csv # 原始数据
anwser.txt # 问题的答案 （Top200）
clustering.ipynb # 代码+报告
requirements.txt # 配置文件
id2paper.json # 文献题目转ID
paper2id.json # ID转文献题目
position.json # 关键簇结果
paper_edges.csv # 文献关系图
paper_cluster_memberships.json # 聚类结果 
```

3. 运行

```
run clustering.ipynb 
```

