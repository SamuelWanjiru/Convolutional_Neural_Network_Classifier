# Convolutional_Neural_Network_Classifier
Convolutional classifier in computer vision

The goal of this repo is to expound how a neural network can "understand" a natural image well-enough to solve the same kinds of problems the human visual system can solve.
The neural networks that are best at this task are called convolutional neural networks (Sometimes we say convnet or CNN instead.) Convolution is the mathematical operation that gives the layers of a convnet their unique structure.

We will apply these ideas to the problem of image classification: given a picture, can we train a computer to tell us what it's a picture of? You may have seen apps that can identify a species of plant from a photograph. That's an image classifier! In this course, you'll learn how to build image classifiers just as powerful as those used in professional applications.

## The Convolutional Classifier

A convnet used for image classification consists of two parts: a convolutional base and a dense head.
The base is used to extract the features from an image. It is formed primarily of layers performing the convolution operation, but often includes other kinds of layers as well. 
The head is used to determine the class of the image. It is formed primarily of dense layers, but might include other layers like dropout.
A feature could be a line, a color, a texture, a shape, a pattern -- or some complicated combination.

## Training the Classifier
The goal of the network during training is to learn two things:
* which features to extract from an image (base),
* which class goes with what features (head).

These days, convnets are rarely trained from scratch. More often, we reuse the base of a pretrained model. To the pretrained base we then attach an untrained head. In other words, we reuse the part of a network that has already learned to do 1. Extract features, and attach to it some fresh layers to learn 2. Classify.

Training the Classifier
The goal of the network during training is to learn two things:

which features to extract from an image (base),
which class goes with what features (head).
These days, convnets are rarely trained from scratch. More often, we reuse the base of a pretrained model. To the pretrained base we then attach an untrained head. In other words, we reuse the part of a network that has already learned to do 1. Extract features, and attach to it some fresh layers to learn 2. Classify.

Attaching a new head to a trained base.
Because the head usually consists of only a few dense layers, very accurate classifiers can be created from relatively little data.

Reusing a pretrained model is a technique known as transfer learning. It is so effective, that almost every image classifier these days will make use of it.

To learn how this works, kindly go through the jupyter notebook.
