# Bird classification

This is a bird image classifcation project and in dataset we have around 300 different species images of birds and our task is to build a model using Deep Learning to classify birds into thier respective species.


## Architecture
##### We have used ResNet Architecture as backbone for our model and added some custom layers on top.

>### RESNET 50 Overview

This is an Image Classifier that follows the Residual Network architecture with 50 layers that can be used to classify objects from among 101 different categories with a high accuracy. In recent years, neural networks have become deeper, with state-of-the-art networks going from just a few layers (e.g., AlexNet) to over a hundred layers. The main benefit of a very deep network is that it can represent very complex functions. It can also learn features at many different levels of abstraction, from edges (at the lower layers) to very complex features (at the deeper layers). However, using a deeper network doesn't always help. A huge barrier to training them is vanishing gradients: very deep networks often have a gradient signal that goes to zero quickly, thus making gradient descent unbearably slow.


In ResNets, a "shortcut" or a "skip connection" allows the gradient to be directly backpropagated to earlier layers:


The "identity block" is the standard block used in ResNets, and corresponds to the case where the input activation (say a[l]) has the same dimension as the output activation (say a[l+2]):


Next, the ResNet "convolutional block" is the other type of block. You can use this type of block when the input and output dimensions don't match up. The difference here is that there is a CONV2D layer in the shortcut path.

## Sample Images from dataset

![birds](https://user-images.githubusercontent.com/82788246/143440163-8d2d1f80-a3de-4ec9-a454-a5bd74bed067.png)

## Results
```bash
training accuracy: 0.9097 
validation accuarcy:0.9071
```
>![2021-11-25](https://user-images.githubusercontent.com/82788246/143470256-4bb75d89-5d96-4f40-9859-d4aa33d15471.png)
