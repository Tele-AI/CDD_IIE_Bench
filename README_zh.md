# CDD-IIE-Bench 📊
[📄 Report](https://link.springer.com/content/pdf/10.1007/s44336-026-00034-3.pdf) | [🤗 HuggingFace](https://huggingface.co/datasets/zangxh/CDD_IIE_Bench)


## 最新进展 🚀
- [x] 2026.03.31 开源 CDD-IIE-Bench 评估集及评估标准
- [x] 2026.03.31 当前最新开源模型的人工评估结果
- [ ] 当前最新闭源模型的人工评估结果正在评估中...

## 数据集介绍 📚
很高兴分享我们的最新研究成果——CDD-IIE-Bench v1.0！
这是一个针对指令式图像编辑任务（Instruct-based Image Editing）的开源评测集，致力于提供全面、深入、具有诊断能力（Comprehensive, in-Depth, and Diagnostic）的评估标准。该数据集共包含2 个大类、5 个中类、21 个小类、33 个细分类别，共 1341 张测试用例。
![Data](assets/data.png)

# 评估标准 ⭐ 
为确保评估准确性，我们采用人工评估（Golden Metric），共有12 位视觉专家，对同一指令下不同模型的生成图像随机排列，对 21 项评估任务，每项任务设定3 个特定评估维度，5 分评级（其中 1 分=差，5 分=优秀），每级均有明确标准，如"添加（Object Addition）"任务共有三个评估维度"指令遵循度"、"  视觉自然度"、"物理细节一致性"。其中"指令遵循度"的 5 分评估标准如下：
* 1分：  未添加任何内容，或添加内容损坏无效。
* 2分：  添加对象类别错误，或与提示无关。
* 3分：  类别正确，但关键属性（位置、颜色、尺寸、数量等）错误。
* 4分：  主要属性正确；仅细节存在轻微偏差或缺少1-2个小特征。
* 5分：  所有指定属性均正确且场景逻辑合理；仅存在微观瑕疵。

更多具体标准参见 [评估标准详细说明（中文）](evalMetrics/metrics_zh.md)

# 评估对象 🎯 
我们对当前最新的开源指令编辑模型进行了人工评估，结果如下
![Benchmark](assets/benchmark.png)


# 参考文献 📖
```python
@article{zang2026instruction,
  title={Instruction-based image editing: a survey on data, models, evaluation, and applications},
  author={Zang, Xianghao and Jiang, Zijian and Cheng, Jiarong and others},
  journal={Vicinagearth},
  volume={3},
  number={1},
  pages={3},
  year={2026},
  publisher={Springer} 
} 
```