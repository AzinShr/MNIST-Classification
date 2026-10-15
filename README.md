# Handwritten Digit Classification Using CNN

A Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify handwritten digits from the MNIST dataset. This project explores convolutional neural networks for image feature extraction and multiclass classification.

## Project Overview

The MNIST dataset contains 70,000 grayscale images of handwritten digits (0–9), including 60,000 training images and 10,000 test images.

The goal of this project is to develop a CNN that learns visual patterns from handwritten digits and predicts the corresponding digit class.

## Model Architecture

The CNN consists of the following layers:

1. **Convolutional Layer 1:** 32 filters with a 2 × 2 kernel and ReLU activation.
2. **Convolutional Layer 2:** 64 filters with a 2 × 2 kernel and ReLU activation.
3. **Max Pooling:** Reduces the spatial dimensions of the feature maps.
4. **Dropout:** Dropout rate of 0.5 to help reduce overfitting.
5. **Flatten:** Converts feature maps into a one-dimensional vector.
6. **Dense Layer:** 250 neurons with ReLU activation.
7. **Output Layer:** 10 neurons with softmax activation, representing the probability of each digit class.

## Training Configuration

- **Dataset:** MNIST
- **Framework:** TensorFlow / Keras
- **Optimizer:** Adadelta
- **Loss Function:** Sparse Categorical Cross-Entropy
- **Evaluation Metric:** Accuracy
- **Epochs:** 12
- **Batch Size:** 500

## Results

After 12 training epochs, the model achieved the following training metrics:

| Metric | Result |
|---|---:|
| Training Loss | ~0.005 |
| Training Accuracy | ~99.85% |
| Test Loss | ~0.041 |
| Test Accuracy | ~98.9% |


## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Learning Objectives

- Understand convolutional neural networks for image classification.
- Explore convolution, pooling, dropout, and dense layers.
- Understand multiclass classification using softmax.
- Investigate loss functions, optimization, and model evaluation.
- Visualize training loss and accuracy across epochs.


