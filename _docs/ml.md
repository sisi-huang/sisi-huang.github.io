---
permalink: /docs/ml/
title: "Machine Learning Notes"
---

Master thesis 
Abstract: Labelling massive datasets consisting of images from webpages manually is quite time-consuming and also exhausting.
If there was a tool which can help us to classify those unlabeled images automatically, it would not
overwhelm us nearly as much. In this thesis we aim to extract significant features from images and to
automate the annotation of unlabeled images.

Due to the variety of images, we focus our 
attention on solving the problem of chart image classification. Chart images are
frequently presented in documents and used as a common tool for visualizing relationships within the data.
Especially, they are able to distinguish themselves by their patterns or shapes.
To deal with
this problem we propose machine learning models that 
can extract the images' features automatically, and predict their labels. 
Convolutional neural networks are the popular models for solving such problem of image classification.
Thus, it is our goal to bridge the relationship between chart images and neural networks. 

In this thesis we attempt two directions to implement convolutional neural networks:
transfer learning and self-training models.
On a set of testing data a model using transfer learning based on the VGG-16 pre-trained model, 
achieves a test accuracy of up to 0.65. 
Self-training models are LeNet-5, Alex blocks and VGG blocks, which are grounded by 
AlexNet and VGG. 
However, performances of self-training models are sightly 
worse than transfer learning, the highest prediction accuracy of 
the self-training models is only 0.47. 
%Hence, transfer learning is a great approach for 
%labeling imbalanced chart images.

\noindent\textbf{Key words:} Image Labelling, Convolutional Neural Network, 
Transfer learning, Machine Learning 



- CNN
- Transfer learning