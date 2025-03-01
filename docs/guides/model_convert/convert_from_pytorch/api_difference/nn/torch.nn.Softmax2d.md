## [ paddle 参数更多 ]torch.nn.Softmax2d

### [torch.nn.Softmax2d](https://pytorch.org/docs/stable/generated/torch.nn.Softmax2d.html?highlight=softmax2d#torch.nn.Softmax2d)

```python
torch.nn.Softmax2d()
```

### [paddle.nn.Softmax](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/nn/Softmax_cn.html#softmax)

```python
paddle.nn.Softmax(axis=-1)
```

其中 Paddle 并没有 torch.nn.Softmax2d 此 api ，可通过 paddle.nn.Softmax 设置参数 axis 为 -3 实现同样的效果：

### 参数映射

| PyTorch | PaddlePaddle | 备注                           |
| ------- | ------------ | ------------------------------ |
| -       | axis         | 指定对输入 Tensor 进行运算的轴。 |

### 转写示例

```python
# PyTorch 写法
cri = torch.nn.Softmax2d()
cri(input)

# Paddle 写法
cri = paddle.nn.Softmax(axis=-3)
cri(input)
```
