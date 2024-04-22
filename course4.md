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


## 作业

### 一. 环境安装和前期准备

#### 1. 克隆XTuner 的源码，并把相关的配套库也通过 pip 的方式进行了安装

![496](image/496.png)

#### 2. 根据自己想要做的事情，利用脚本准备好了一份关于调教模型认识自己身份弟位的数据集

![497](image/497.png)

#### 3. 根据自己的显存及任务情况确定了使用 InternLM2-chat-1.8B 这个模型，并且将其复制到我们的文件夹里

![498](image/498.png)

#### 4. 在 XTuner 已有的配置文件中，根据微调方法、数据集和模型挑选出最合适的配置文件并复制到我们新建的文件夹中。

![499](image/499.png)

### 二. 配置文件修改

![4991](image/4991.png)

### 三. 模型训练

![4992](image/4992.png)

### 四. 模型转换、整合、测试及部署

#### 1. 模型转换



#### 2. 模型整合

#### 3. 对话测试

#### 4. Web demo 部署




