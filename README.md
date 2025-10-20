# Tumor-Detection-Algorithm
My ML Algorithm to detect Malignant or Benign Tumors

This project uses a **Convolutional Neural Network (CNN)** to classify MRI brain scans
as **benign** or **malignant**. It was developed as part of my **Machine Learning Capstone Project**.

---

## Overview
Traditional tumor diagnosis is manual and error-prone.  
This project automates MRI tumor classification using deep learning to improve accuracy and speed.

---

## Dataset
The dataset is from Kaggle:  
[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

It contains labeled MRI images:
- **yes/** → malignant
- **no/** → benign

---

## Model Architecture
- 3 Convolutional Layers (32, 64, 128 filters)
- Max Pooling after each Conv layer
- Dropout (0.5)
- Fully Connected (Dense) layer with 128 units
- Sigmoid output for binary classification

---

## How to Run

**The notebook is still in training. A notebook that is appropriate for end users will be published once the model has been fine-tuned.**
TO RUN THE TRAINING NOTEBOOK:
- Open the notebook
- Enable GPU via *Runtime → Change runtime type → GPU*
- Upload your `kaggle.json` file
- Run all cells

### 2. Local Setup 
```bash
git clone https://github.com/<your-username>/brain-tumor-cnn.git
cd brain-tumor-cnn
pip install -r requirements.txt

