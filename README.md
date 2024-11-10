![GithubProjectBanner](https://github.com/user-attachments/assets/961492cf-00a0-4d96-bb32-efef1f320d54)
# Musician Classifier Model
This project explores various machine learning techniques for facial recognition to classify images of my favorite classical musicians.

## Table of Contents
- [Introduction](##introduction)
- [Features](#features)
- [Packages](#packages)
- [Data](#data)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)

## Introduction

The **Musician Classifier Model** is designed to classify images of musicians by utilizing different machine learning approaches, including image processing and model fine-tuning. The project focuses on facial recognition accuracy by applying and comparing the following techniques:
- **Haar Cascade** for feature detection.
- **Wavelet Transform** for image transformation.
- **Data Cleaning** for quality control.
- **Model Fine-tuning** to improve performance.

This project was developed using images collected from Google Images, with the **Fatkun Batch Image Downloader** Chrome extension.

## Features

- **Facial Detection**: Uses Haar Cascade to detect facial features.
- **Image Transformation**: Wavelet Transform is applied to preprocess the images.
- **Model Fine-Tuning**: Optimizes model parameters to enhance classification accuracy.

## Packages

To run this project, you need the following dependencies:

- Pandas
- NumPy
- OpenCV
- Matplotlib
- Seaborn

## Data
- Images of 6 classical musicians were gathered from Google Images.
- For each musician, 100 initial images were collected.
- These images were then cropped to show only the face and scanned for facial features. 
- After data cleaning, each musician had roughly 80-90 images.
- The images were then transformed using wavelet transform into a numpy array of RGB values.

<img src="https://github.com/user-attachments/assets/3156b957-1c14-4fd8-97e2-c78cf1ff6dc9" width=30% height=30%>
<img src="https://github.com/user-attachments/assets/c939177c-082c-42a8-9c06-3410ec041ab2" width=30% height=30%>
<img src="https://github.com/user-attachments/assets/5492e7ef-20bf-400a-81b0-6a56ede5bc57" width=30% height=30%>

## Model Training and Evaluation
Models tested:
- Support Vector Machines
- Random Forest
- Logistic Regression
- K-Nearest Neighbors

The hyperparameters were all fine-tuned using a GridSearch CV. 

## Results
- The best-performing model (logistic regression) had an average cross-validation score of 0.877.
- Other metrics considered were:
  - Precision
  - Recall
  - F1-Score
  - Support
    
## Sources
https://pywavelets.readthedocs.io/en/latest/
