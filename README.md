# Tumor-Detection-Algorithm
My ML Algorithm to detect Malignant or Benign Tumors

This project uses a **Convolutional Neural Network (CNN)** to classify MRI brain scans
as **benign** or **malignant**. It was developed as part of my **Machine Learning Capstone Project**.

---

## Overview
Traditional tumor diagnosis is manual and error-prone.  
This project automates MRI tumor classification using deep learning to improve accuracy and speed. The project tracks the progress of implementing a CNN algorithm from scratch using limited enthusiast level resources. 

---

## Dataset
The dataset is from Kaggle:  
[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)


---

## Model Architecture
The model is a deep CNN consisting of 4 convolutional blocks followed by fully connected layers, designed for binary classification of MRI images resized to 128 × 128 × 3.
In total, the network contains over 30 layers, including convolutional layers, batch normalization, pooling, dropout, and dense layers.

Each convolutional block follows the pattern:

- Conv2D 
- Batch Normalization
- Conv2D (32 filters, 3×3, ReLU)
- Batch Normalization
- MaxPooling2D (2×2)
- Dropout (0.25)

---

## How to Run
- Open the notebook
- Enable GPU via *Runtime → Change runtime type → GPU*
- Upload your `kaggle.json` file to gain access to the dataset
- Run all cells



