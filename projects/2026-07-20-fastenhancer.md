\# FastEnhancer 语音增强模型跑通



&#x20; > 日期：2026-07-20 | 方向 4：空间感知语音增强



&#x20; ## 做了什么

&#x20; - 下载 FastEnhancer T 版 ONNX 模型（0.1MB）

&#x20; - 成功运行 ONNX Runtime 推理

&#x20; - 验证强噪场景降噪效果



&#x20; ## 跑通记录

&#x20; - 模型：FastEnhancer-T (ONNX)

&#x20; - RTF：0.07

&#x20; - 依赖：numpy + scipy + librosa + onnxruntime

&#x20; - 输入：带噪语音 → 输出：干净人声



&#x20; ## 下一步

&#x20; - 了解 FastEnhancer 与方向 4 多通道主动降噪的结合方式

&#x20; - 探索 ONNX → RKNN 部署可能性

