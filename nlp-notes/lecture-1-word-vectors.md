# Lecture 1: Introduction & Word Vectors

> CS224n Winter 2019 | 学习日期：2026-07-05

## 核心概念

### 分布式假设（Distributional Hypothesis）
一个词的含义由它经常出现的上下文决定。
> "You shall know a word by the company it keeps." — J.R. Firth (1957)

### 为什么需要词向量？
- 计算机只能处理数字，不能直接理解文字
- One-hot 编码：维度灾难 + 无法表达语义关系
- 词向量：将词映射到低维稠密实数向量空间

### Word2Vec
- **CBOW**：用上下文词预测中心词
- **Skip-gram**：用中心词预测上下文词

### 词向量的性质
- 语义相近的词，向量空间中距离近
- 可以做语义运算：king - man + woman ≈ queen
- 用余弦相似度衡量词语义接近程度

## 代码验证

```
king 和 queen 的相似度:   0.992
king 和 apple 的相似度:   0.420
apple 和 banana 的相似度: 0.999
king - man + woman → queen (匹配度 1.000)
```

## 待补基础
- 损失函数与梯度下降 → 需补吴恩达机器学习前 3 课
