# SP25-690-Thotamatam

# Driver Drowsiness Detection

A deep learning project that classifies driver facial images as Alert or Drowsy 
using a Convolutional Neural Network (CNN), with Logistic Regression as a baseline.

## Problem
Drowsy driving is a major cause of road accidents. This project builds a binary 
image classifier to detect drowsiness from driver facial images in real time.

## Dataset
- Source: [Driver Drowsiness Dataset (DDD)](https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd)
- 2 classes: Alert, Drowsy
- Downloaded via Kaggle API

## Models
- CNN (3 convolutional blocks + dense layers)
- Logistic Regression (baseline)

## Results
- CNN Validation Accuracy: 64.3% (overfitting observed — 99.4% train vs 64.3% val)
- Logistic Regression Test Accuracy: 98%

## How to Run
1. Clone the repo
2. Open `Drowsiness.Detection.ipynb` in Google Colab
3. Add your Kaggle API credentials
4. Run all cells (Runtime → Run all)

## Dependencies
See `requirements.txt`

## Key Hyperparameters
- Image size: 224x224
- Batch size: 32
- Epochs: 3
- Optimizer: Adam
- Loss: Binary Crossentropy
- Dropout: 0.5
