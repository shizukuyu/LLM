## 两种常见Finetune
- 增量预训练微调，加新知识
- 指令跟随微调，一问一答有监督的标注

![41](image/41.png)

对话模板XTuner框架里都包含了，最后的增量预训练微调只对答案部分进行损失计算

![42](image/42.png)

## LoRA & QLoRA
lora的adapter参数量远小于原来的linear，减少了显存开销

qlora 4-bit量化模式加载base model，没有那么精确，减少了显存开销

![43](image/43.png)

![44](image/44.png)

## XTuner
- High-level，轻量级，适配多种生态和硬件

![45](image/45.png)

## XTuner快速上手

![46](image/46.png)

![47](image/47.png)

![48](image/48.png)

- 支持工具类模型对话，内置了数据引擎（数据集映射参数）

![49](image/49.png)

![491](image/491.png)

## 8GB显存LLM

- XTuner内置的两种优化技巧，Flash Attention，DeepSpeed ZeRO

![492](image/492.png)

## 多模态LLM

- 原理

![493](image/493.png)

- 文本单模态LLM + image projector，LLaVA模型

![494](image/494.png)

### 快速上手多模态LLM

給LLM增加视觉能力即训练image projector，两个阶段：Pretrain + Finetune

![495](image/495.png)





