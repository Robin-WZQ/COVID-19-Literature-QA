### **Text Mining by Word Representation**

> ipynb中图片显示不出来的话，将本文件夹下载到本地即可看到

#### 文件说明

| pic # ipynb里面的图片

|biobert_v1.1_pubmed_pytorch_model # biobert模型文件

|pdf_json # 带标注的文献全文

metadata.csv # 原始数据

anwser.txt 问题的答案 （Top200）

1120190892.ipynb 代码+报告

requirements.txt 配置文件

stopwords.txt 英文停词词典

#### 配置文件说明

除了常规第三方库外，需要说明biobert_embedding这个库：

首先正常pip install biobert-embedding，由于该库在使用时会首先下载放在google drive上的预训练模型文件（通过request这个库下载），但是由于网络原因下载不下来。因此需要首先挂梯子，在[biobert_v1.1_pubmed_pytorch_model.tar.gz (dropbox.com)](https://www.dropbox.com/s/hvsemunmv0htmdk/biobert_v1.1_pubmed_pytorch_model.tar.gz?dl=0) 中下载所有文件至目录biobert_v1.1_pubmed_pytorch_model/中，之后注释掉../site-packages/biobert_embedding/downloader.py中第44-75行的内容即可。

