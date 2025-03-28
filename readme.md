下载的模型代码分别放在对应的模型为名的目录（如下）：
```
bge
├── Dockfile
├── api.py
├── docker-compose.yml
├── readme.md
└── requirements.txt
├── bge-reranker-base-onnx-o4
│   ├── README.md
│   ├── config.json
│   ├── gitattributes
│   ├── model.onnx
│   ├── ort_config.json
│   ├── sentencepiece.bpe.model
│   ├── special_tokens_map.json
│   ├── tokenizer.json
│   └── tokenizer_config.json
├── bge-m3
│   ├── 1_Pooling
│   │   └── config.json
│   ├── README.md
│   ├── colbert_linear.pt
│   ├── config.json
│   ├── config_sentence_transformers.json
│   ├── gitattributes
│   ├── imgs
│   │   ├── imgs_.DS_Store
│   │   ├── imgs_bm25.jpg
│   │   ├── imgs_long.jpg
│   │   ├── imgs_miracl.jpg
│   │   ├── imgs_mkqa.jpg
│   │   ├── imgs_nqa.jpg
│   │   └── imgs_others.webp
│   ├── long.jpg
│   ├── modules.json
│   ├── pytorch_model.bin
│   ├── sentence_bert_config.json
│   ├── sentencepiece.bpe.model
│   ├── sparse_linear.pt
│   ├── special_tokens_map.json
│   ├── tokenizer.json
│   └── tokenizer_config.json
```
3. 安装依赖
```
cd ./bge
## 执行此命令时,需切换至bge目录下
pip install -r requirements.txt
```

4. 运行代码
```
python api.py
```
这里的 http://127.0.0.1:50001 就是请求地址。


docker 本地部署


## 切换至bge目录下
```
cd bge
## 先下载模型文件到当前目录,然后执行下面命令
docker-compose up -d
```
