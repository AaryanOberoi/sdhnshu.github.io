---
layout: post
title: Image classifier
tag: deep
plugin: lightense
---

This was my second project in Udacity's Deep Learning Nanodegree Foundation course where we took the *[CIFAR 10 database](https://www.cs.toronto.edu/~kriz/cifar.html)*, a classic image classification dataset and trained a basic __Convolutional Neural Network__ to classify between the 10 categories specified:
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