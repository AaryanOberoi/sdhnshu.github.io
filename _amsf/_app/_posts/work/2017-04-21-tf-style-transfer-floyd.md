---
layout: post
title: Style transfer on FloydHub
tag: deep
plugin: lightense
---

Here I have implemented the first style transfer paper that came out in [2015 by Gatys et al.](https://arxiv.org/pdf/1508.06576.pdf) Implementing the project with tensorflow, I used a deep learning cloud service called [Floyd](https://www.floydhub.com/) to train it. Check them out, they give 100 hrs GPU usage for free on signup.

- airplane
- automobile
- bird
- cat
- deer
- dog
- frog
- horse
- ship
- truck

![BikeDataset](assets/img/bike-dataset.png){: .size-small}

*The first fifteen columns are features and the last one(cnt) is the label*

The model built in Tensorflow was able to classify images with an accuracy of 80%

And the label was the number of people who rented the bicycles in that hour in those conditions. The network would be trained to predict this number based on the features given.

After implementing a very basic __feedfowrard network__ in Tensorflow and training it on these datapoints an accuracy of 80% was achieved.

The dataset file is included in the repo and a detailed jupyter notebook letting you through the project.

Feel free to check it out *[github](https://github.com/sdhnshu/bike-rental)*