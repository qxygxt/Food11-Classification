# Food11-Classification
Using pretrained DenseNet-121 for image classification

## 1 Environment:

In this experiment, Google Colab is used to utilize GPU acceleration and achieve better training results in a shorter time. 

The source code is in notebook format and can be directly opened on the Google Colab platform by running each code block sequentially.

## 2 Program Workflow

**(1) Data Processing**

First, downloading [food images dataset](https://www.kaggle.com/datasets/trolukovich/food11-image-dataset) from Kaggle, and upload zip to Google Drive (compression speeds up the upload process), and then extract it.

Next, define some data augmentation operations, such as cropping and rotation. 

Finally, extract the labels and put all the data into dataloaders.

**(2) Model Building**

The model consists of a pretrained DenseNet121 and a fully connected layer.

**(3) Model Training**

The loss function is cross-entropy, and the Adam optimizer is used.

![f45a7d139a05776aa863360d36ebcd8](https://user-images.githubusercontent.com/98147306/227771795-228606be-f796-4020-ab49-2e657744ad27.png)

**(4) Model Testing**

![ba19b1260fa66a4b337757ca68ace8e](https://user-images.githubusercontent.com/98147306/227771832-dffa3212-d769-43d3-9d57-0a4a5b42a600.png)
