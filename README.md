# Tumor-Detection-Algorithm
Welcome to my Machine Learning Passion Project!

This is ML Algorithm to detect Malignant or Benign Tumors

This project uses a **Convolutional Neural Network (CNN)** to classify MRI brain scans
as **benign** or **malignant**. It was developed as part of my Machine Learning class at Virginia Tech but since been transformed and improved upon for my own satisfaction.


**THIS PROJECT IS A CONTINUOUS WORK IN PROGRESS - Check back for updates!**


---

## Overview

My goal with this project is to automate MRI tumor classification using deep learning to improve accuracy. The main idea I wanted to focus on was building an algorithm from scratch that has a high accuracy as well as a low loss rate. 

---

## Dataset
The dataset is from Kaggle:  
[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
*NOTE: You will need a JSON key from Kaggle to be able to run my notebook. Although, an already compiled .keras file is uploaded with pre-loaded weights ready to be tested.* 

---

## Model Architecture
The model is a deep CNN consisting of 4 convolutional blocks followed by fully connected layers, designed for 4 way classification of MRI images.
In total, the network contains 25 layers, including convolutional layers, batch normalization, pooling, dropout, and dense layers.

Each convolutional block follows the pattern:

- Conv2D 
- Batch Normalization
- Conv2D 
- Batch Normalization
- MaxPooling2D (2×2)
- Dropout 

The depth block follows the pattern:
- Conv2D
- Batch Normalization
- MaxPooling2D
- Dropout

The head block follows the pattern:
- GlobalAveragePooling2D
- Dropout
- Dense
  
---

## How to Run
- Open the notebook (Google Colab is preferred)
- Enable GPU via *Runtime → Change runtime type → GPU* (Recommend using the A1000 GPU)
- Upload your `kaggle.json` file to gain access to the dataset
- Run all cells
*Note: The notebook does not need to be run, the .keras model is uploaded to be tested*

# Results
*Note: This project is still a work in progress.*
- Best Training Accuracy: 99.67%
- Best Validation Accuracy: 92.46%

- Best Training Loss: 0.3192
- Best Validation Loss: 0.5062

- Testing Accuracy: 93.75%
- Testing Loss: 0.4490



