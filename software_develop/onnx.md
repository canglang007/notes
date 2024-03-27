### onnx 相关知识

#### 1.

`InferenceSession` 是`onnxruntime`库提供的一个类，用于创建一个推理会话。这个推理会话将加载一个预训练或自定义的 ONNX 模型，以便进行模型推理。

```python
ort_session = onnxruntime.InferenceSession('resnet18_imagenet.onnx')
```
