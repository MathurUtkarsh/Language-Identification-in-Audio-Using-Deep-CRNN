# Language Identification Using Deep Convolutional Recurrent Neural Networks

## Introduction

This project contains the code for the paper "Language Identification Using Deep Convolutional Recurrent Neural Networks", which will be presented at the 24th International Conference on Neural Information Processing (ICONIP 2017).

## Problem Statement

The problem at hand is to develop a language identification system that can accurately predict the language of a given audio recording from among six international languages, namely English, German, French, Spanish, Chinese, and Russian. The system will take audio recordings of the specific language as input from the user and output the predicted language. The challenge lies in designing a robust and efficient system that can accurately identify the language despite variations in dialects, accents, and background noise.

## Description Overview

The aim of this project is to create an accurate language identification system for six international languages using deep learning techniques. The system will analyze speech recordings and identify the spoken language based on unique phonetic and acoustic properties. The proposed solution will use a tailored deep convulutional recurrent neural network architecture for speech recognition to perform robustly under varying acoustic conditions. This project aims to provide a practical solution for automated language identification with potential applications in areas such as speech recognition, language translation, and language learning.

## Technology Use

Here we will be using Anaconda Python 3.6, Keras 2.2.4 using TensorFlow GPU 1.14.0 backend CUDA 10 with CuDNN 10. 

## Installation

Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

**In Pycharm it’s easy **

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using conda with python3.6
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from requirements.txt file using the command pip install -r requirements.txt


**In Conda also it’s eay**

1. Create a new virtual environment using the command
    conda create -n your_env_name python=3.6
2. Navigate to the project directory.
3. Install the necessary packages from requirements.txt file using the command         
pip install -r requirements.txt

## WorkFlow Diagram

![Picture1](https://user-images.githubusercontent.com/78642104/202015195-c0d8b584-0bcc-43c5-8728-faa51118e50e.jpg)


![Picture2](https://user-images.githubusercontent.com/78642104/202015270-f4bd6edf-db42-40da-a7bc-9f21c7a31ae5.png)

This above picture is of the project directory if we open the project folder using Pycharm. 

**2. SpectrogramGenerator.py**

![Picture3](https://user-images.githubusercontent.com/78642104/202015467-09581a24-6d44-442e-8a91-8b79fb45bad3.jpg)

This file is present in the dataloaders folder. SpectrogramGenerator.py is used to convert our .wav speech recored files to spectrogram images which will be used for training.

**3. train.py**

![Picture4](https://user-images.githubusercontent.com/78642104/202015578-4761cbed-3d0f-4aea-b15a-4992e6e3e1a9.jpg)

This file is used to do the training of the dataset and finally we will get the trained model which will be used for prediction.

**4. predict.py**

![Picture5](https://user-images.githubusercontent.com/78642104/202015750-b7ff9e89-0e72-4c9b-b0ab-082a69e07e6a.jpg)

This file is used to do the prediction of the given user input with two other argument parameters.

**5. clientApp.py**

![Picture6](https://user-images.githubusercontent.com/78642104/202015815-acaf5fbd-f775-4201-b3aa-d984c14384e4.jpg)

This file is the flask server file and entry point of application.

## Conclusion

In this project we have successfully built a language identification which can classify and identify six internatonal languages.

## Comparision

Here we can do a lot of improvements. We can go with pre trained models like BERT , GPT2 etc to increase the accuracy. We can also increase the size of the training data.








