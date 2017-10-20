---
layout: post
title: Style transfer on FloydHub
tag: deep
plugin: lightense
scheme-bg: "#8A171A"
scheme-text: "#dddddd"
scheme-link: "#f92a2f"
scheme-hover: "#f92a2f"
scheme-code: "#f92a2f"
---

Here I have implemented the first style transfer paper that came out in [2015 by Gatys et al.](https://arxiv.org/pdf/1508.06576.pdf) in Tensorflow.

![Style](assets/img/style.gif){: .size-small}

The task here is to take __Mona Lisa__ and add the texture of a famous Japanese painting - __The Great Wave off Kanagawa__ on top of it. In other words, take the content from Mona Lisa and the style from The Wave and combine them.

I used a pretrained [VGG19](http://www.robots.ox.ac.uk/~vgg/research/very_deep/) network trained on the ImageNet dataset.

The main part of this project is the loss functions. We have 2 loss functions here: *content loss* (difference between the output and Mona Lisa) and *style loss* (difference between the output and The Wave)

I used a deep learning cloud service called [Floyd](https://www.floydhub.com/) to train it. Check them out, they give 100 hrs GPU usage for free on signup.

Feel free to check it out *[github](https://github.com/sdhnshu/artistic-style-transfer-on-floydhub)*

*PS. It was appriciated by the founder of Floyd on [twitter](https://twitter.com/FloydHub_/status/857688492574334976)*