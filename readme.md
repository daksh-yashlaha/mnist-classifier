# MNIST Classifier

## Project Description

MNIST Classifier is a CNN based model that is used to classify the MNIST dataset (handwritten digits by Yan Lecun). It is one of the basic projects of CNN.
We have made 3 basic CNN architectures to compare the accuracies of different models as the layers are changed.

## Modules Required

This module makes use of the following modules with specified versions : 

| Module           | Version          |
|------------------|------------------|
| numpy            | version 1.13.3   |
| tensorflow       | version 1.4.1    |

## Software Requirements

| Anaconda          | Version           |
| ----------------- | ----------------- |
|anaconda-client    | version 1.6.5     |
|anaconda-navigator | version 1.6.12    | 
| anaconda-project  | version 0.8.0     |

## Setting Up

Please follow the following steps for setting up and running the CNN model :
1. Download the cnn model files from the main branch.
2. Open Anaconda Navigator
3. Select Spyder
4. Open any project file <model_name>.py
5. Run the program

## Dataset Description

The MNIST dataset has been imported from the dataset present in tensorflow tutorials. It consists of a total pf 55000 gray-scaled images with pixel values between 0 and 255.
Each image is of dimensions 28*28*1 and is represented as a vector of dimensions [,784]. Some sample images are as follows :

![Sample Dataset Images](/images/Figure_1.png)
![Sample Dataset Images](/images/Figure_2.png)
![Sample Dataset Images](/images/Figure_3.png)
![Sample Dataset Images](/images/Figure_4.png)
![Sample Dataset Images](/images/Figure_5.png)

## Model Architecture

There are three different architectures present : 
1. The first architecture makes use of the following layers : 
	Input -> Conv1 -> Relu -> Max_Pool1 -> Conv2 -> Relu -> Max_Pool2 -> FC1 -> Output
2. The second architecture further deepens the first one by introducing additional convolutional layers :
	Input -> Conv1 -> Relu -> Conv2 -> Relu -> Max_Pool1 -> Conv3 -> Relu -> Conv4 -> Relu -> Max_Pool2 -> FC1 -> Output
3. The third architecture removes the max_pool layer and downsamples using conv layers :
	Input -> Conv1 -> Relu -> Conv2 -> Relu -> Conv3 -> Relu -> Conv4 -> Relu -> FC1 -> Output

![Model 1 Accuracy](/images/cnn_model_1.png)
![Model 2 Accuracy](/images/cnn_model_2.png)
![Model 3 Accuracy](/images/cnn_model_3.png)
