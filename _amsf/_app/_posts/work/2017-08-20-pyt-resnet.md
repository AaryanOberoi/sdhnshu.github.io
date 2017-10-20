---
layout: post
title: ResNet in PyTorch
tag: deep
plugin: lightense
scheme-bg: "#8A171A"
scheme-text: "#dddddd"
scheme-link: "#f92a2f"
scheme-hover: "#f92a2f"
scheme-code: "#f92a2f"
---

This is the first of the collection of deep learning models I am building in PyTorch. Its the ResNet 2015 by Microsoft [(arxiv link).](https://arxiv.org/pdf/1512.03385.pdf)

The new concept of __Residuals__ was introduced with ResNet. It helps training very deep networks train faster. The paper proposed by Microsoft had 33 convolution layers and is able to train in the same amount of time as a normal network with a greater accuracy than a normal network. It won the ImageNet 2015 image classification challenge.

The Structure of a Residual block is:
```
Conv with batch norm
Relu
Conv with batch norm
Downsample if present
Resisual
Relu
```

The ResNet structure implemented in this project is:
```
Conv with batch norm
Relu

Residual Block
Residual Block

Residual Block with downsampling
Residual Block
Residual Block 

Residual Block with downsampling
Residual Block
Residual Block 

Avg pool
Fully connected
```

Feel free to check it out *[github](https://github.com/sdhnshu/pytorch-model-zoo/tree/master/resnet)*