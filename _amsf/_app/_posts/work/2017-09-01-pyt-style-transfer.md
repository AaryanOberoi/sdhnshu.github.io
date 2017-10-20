---
layout: post
title: Style transfer in PyTorch
tag: deep
plugin: lightense
scheme-bg: "#FFB60F"
scheme-text: "#000000"
scheme-link: "#a57d22"
scheme-hover: "#a57d22"
scheme-code: "#a57d22"
---

A VGG19 model, readily provided by the PyTorch was used for this project. The output from its 0, 5, 10, 19 and 28 layers was used as the style and content components.

Here is an example passed through the network:

![emma](assets/img/style-emma.jpg)

Feel free to check it out *[github](https://github.com/sdhnshu/pytorch-model-zoo/tree/master/artistic%20style%20transfer)*