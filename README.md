[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

Welcome to the Convolutional Neural Network (CNN) project! In this project, you will learn how to build an algorithm that processes real-world images provided by users. Given an image of a dog, your algorithm will identify and estimate the breed of the dog. If the image is of a human, the code will predict the closest dog breed.


![Sample Output][image1]

While learning about state-of-the-art CNN models for classification, you will also make important design decisions for the user experience. Our goal is that, by the end of this project, you will understand the challenges of creating a data processing pipeline by combining a series of models to perform various tasks. Each model has its own advantages and limitations, and when designing real-world applications, you will often face problems with no optimal solutions. Although your solution might not be the best, your design will provide a great user experience!


## Project Guide

### Steps

1. Clone the repository and open the downloaded folder.


2. Download the [dog dataset](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/dogImages.zip) and extract it into the repository at `project_path/dogImages`.

3. Download the [human dataset](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/lfw.zip) and extract it into the repository at `project_path/lfw`.

4. Download the [VGG-16 bottleneck features](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd101/v4-dataset/DogVGG16Data.npz) for the dog dataset and place them in the repository at `project_path/bottleneck_features`.

5. Install the necessary Python dependencies.

For __Mac/OSX__:

```bash
conda env create -f requirements/dog-mac.yml
source activate dog-project
KERAS_BACKEND=tensorflow python -c "from keras import backend"
```

For __Windows__:

```bash
conda env create -f requirements/dog-windows.yml
activate dog-project
set KERAS_BACKEND=tensorflow
python -c "from keras import backend"
```

6. Open the notebook:

```
jupyter notebook dog_app.ipynb
```

__Note:__ While we have implemented some code to help you get started quickly, you will still need to implement additional functionality to answer all the questions in the notebook. 
__Do not modify any of the provided code unless specified otherwise.__

---
