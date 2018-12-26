---
layout: post
title: "A winter break project: classifying and analyzing telemetry data using convolutional neural nets and TensorFlow"
data: 2018-12-26 15:00:00
categories: jekyll update
---

I always like to pick a project or two to try to finish during my break 
from teaching in December and January. 
Ideally, this will be something where I can learn a new skill/area which 
I haven't had time to dig into over the course of the previous year.
Earlier this year I played around with TensorFlow, doing some obligatory tutorials.
However, I have been wanting to try something a little more interesting.
One of my next projects is going to be analyzing telemetry data from mice. 
For this initial work then, I chose to work with a much easier (but structurally similiar) 
data set, UCI's ['Activity Recognition from Single Chest-Mounted Accelerometer Data Set](https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+from+Single+Chest-Mounted+Accelerometer). 
This data set consists of time series with 3-dimensional coordinate values for acceleration of a sensor mounted on the chest of one of 16 individuals.
There have been major advances in image classification over the last 15 years, 
so it makes sense to try to use some of those advances to improve our
understanding of non-image data.

To this end I coverted each set of three time series (x,y,z) into an image using 
a continuous wavelet transform and then trained a CNN on 
a training set of such images. The algorithm performed well with a
classification rate of 94.5%. 

Check out the code on [GitHub](https://github.com/hkvinge/classifying_telemetry_data_with_cnns).
