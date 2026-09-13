# AI-Based Phishing Website Screenshot Detection Using Computer Vision

## Project Overview

This project presents an AI-based computer vision system for detecting whether a website screenshot is **legitimate** or **phishing**.

The system processes website screenshots, extracts visual features using **Histogram of Oriented Gradients (HOG)**, and uses a **Support Vector Machine (SVM)** classifier to predict the class of the website.

The project is designed as a lightweight, CPU-friendly command-line application.

---

## Problem Statement

Phishing websites are designed to imitate legitimate websites and deceive users into entering sensitive information such as usernames, passwords and financial details.

Traditional URL-based detection methods may not always identify visually deceptive websites. This project explores a computer vision-based approach that analyzes the visual appearance of website screenshots to classify them as legitimate or phishing.

---

## Objectives

- Detect phishing websites using website screenshots.
- Apply image preprocessing techniques to standardize input images.
- Extract visual features using HOG.
- Train an SVM-based machine learning classifier.
- Evaluate the classification performance using standard metrics.
- Provide a simple command-line interface for prediction.

---

## Main Features

### 1. Image Preprocessing

- Loads website screenshots.
- Resizes images to a fixed size.
- Converts images to grayscale.
- Normalizes image values.

### 2. HOG Feature Extraction

- Extracts Histogram of Oriented Gradients features.
- Represents visual structures and edge information numerically.

### 3. SVM Classification

- Uses a Support Vector Machine with an RBF kernel.
- Uses balanced class weights to handle class imbalance.

### 4. Model Evaluation

- Calculates accuracy, precision, recall and F1-score.
- Generates a confusion matrix.

### 5. Command-Line Prediction

- Accepts a website screenshot as input.
- Predicts whether it is legitimate or phishing.
- Displays prediction confidence.

---

## Technologies Used

- Python
- OpenCV
- NumPy
- Scikit-image
- Scikit-learn
- Joblib
- Matplotlib
- Seaborn
- Pytest
- Git and GitHub

---

## Dataset

The project uses the **Phishing Sites Screenshot** dataset available on Kaggle.

Dataset source:

https://www.kaggle.com/datasets/zackyzac/phishing-sites-screenshot

The dataset contains screenshots belonging to two classes:

- `legitimate`
- `phishing`

### Dataset Distribution

| Class | Number of Images |
|---|---:|
| Legitimate | 1,147 |
| Phishing | 550 |
| Total | 1,697 |

The dataset is not included in this GitHub repository because of its large size.

### Dataset Setup

After downloading the dataset, organize the images in the following structure:

```text
dataset/
├── legitimate/
└── phishing/
---

## Project Workflow

```text
Website Screenshot
        ↓
Image Preprocessing
        ↓
Resize + Grayscale + Normalization
        ↓
HOG Feature Extraction
        ↓
SVM Classifier
        ↓
Prediction
        ↓
Legitimate / Phishing
        ↓
Confidence Score
