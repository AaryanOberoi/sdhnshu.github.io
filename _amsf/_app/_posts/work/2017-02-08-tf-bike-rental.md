---
layout: post
title: Feedforward neural net 
tag: deep
plugin: lightense
---

This was my first project in Udacity's Deep Learning Nanodegree Foundation course where a bunch of datapoints are given like:
- Day
- Date
- Wind speed
- Humidity and some others
These were taken as features

![BikeDataset](assets/img/bike-dataset.png){: .size-small}

*The first fifteen columns are features and the last one(cnt) is the label*

And the label was the number of people who rented the bicycles in that hour in those conditions. The network would be trained to predict this number based on the features given.

After implementing a very basic __feedfowrard network__ in Tensorflow and training it on these datapoints an accuracy of 80% was achieved.

The dataset file is included in the repo and a detailed jupyter notebook letting you through the project.

Feel free to check it out *[github](https://github.com/sdhnshu/bike-rental)*