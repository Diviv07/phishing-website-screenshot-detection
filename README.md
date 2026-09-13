# AI-Based Phishing Website Screenshot Detection Using Computer Vision

## 1. Project Overview

This project detects whether a website screenshot is likely to be a legitimate website or a phishing website using computer vision and machine learning.

The system takes a website screenshot as input, preprocesses the image, extracts visual features using Histogram of Oriented Gradients (HOG), and classifies the screenshot using a Support Vector Machine (SVM).

## 2. Problem Statement

Phishing websites are designed to visually imitate legitimate websites and trick users into entering sensitive information. Traditional detection methods may depend on URLs or manually maintained lists.

This project explores a computer-vision-based approach that analyzes the visual appearance of a website screenshot to classify it as legitimate or phishing.

## 3. Objectives

- Detect phishing websites from screenshots.
- Apply computer vision techniques for visual feature extraction.
- Use HOG features to represent website screenshots.
- Train an SVM-based machine learning classifier.
- Provide a simple command-line interface for prediction.
- Evaluate the model using accuracy, precision, recall and F1-score.

## 4. Main Features

- Website screenshot preprocessing
- HOG feature extraction
- SVM-based classification
- Legitimate/phishing prediction
- Prediction confidence
- Model evaluation
- Automated preprocessing test
- CSV-based evaluation results

## 5. Technologies Used

- Python 3.12
- OpenCV
- NumPy
- Scikit-image
- Scikit-learn
- Joblib
- Pytest

## 6. System Workflow

```text
Website Screenshot
        |
        v
Image Preprocessing
        |
        v
HOG Feature Extraction
        |
        v
SVM Classifier
        |
        v
Legitimate / Phishing
        |
        v
Prediction Confidence