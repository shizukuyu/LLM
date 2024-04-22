## RAG概述

- 简单来说rag就是在已训练好大模型的基础上增加一个外部数据库，使llm生成的内容在垂直领域达到相应的效果
- 主要目的是降本增效

![31](image/31.png)

### 可以解决的问题

- 幻觉
- 过时知识
- 缺乏透明和可追溯的推理过程


### 基础效果对比

![32](image/32.png)


## RAG工作原理

![33](image/33.png)

- Indexing
    - docs to Vetor-DB
    Similarity check: cosine distance, dot product

![34](image/34.png)

- Retrieval
- Generation

## RAG发展历程

![35](image/35.png)

- Naive
- Advanced
- Modular

## RAG常见优化方法

![36](image/36.png)

## RAG vs Fine-Tuning

总的来说RAG更加灵活和动态，Fine-tuning高度专业化

![37](image/37.png)

## RAG总结

这个图做的可真好，赏心悦目呢！

![38](image/38.png)

