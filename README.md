# Handwritten Digit Classification Using CNN

A Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify handwritten digits from the MNIST dataset. This project explores convolutional neural networks for image feature extraction and multiclass classification.

## Project Overview

The MNIST dataset contains 70,000 grayscale images of handwritten digits (0–9), including 60,000 training images and 10,000 test images.

The goal of this project is to develop a CNN that learns visual patterns from handwritten digits and predicts the corresponding digit class.

## Model Architecture

The CNN consists of the following layers:

1. **Convolutional Layer 1:** 32 filters with a 3 × 3 kernel and ReLU activation.
2. **Convolutional Layer 2:** 64 filters with a 3 × 3 kernel and ReLU activation.
3. **Max Pooling:** Reduces the spatial dimensions of the feature maps.
4. **Dropout:** Dropout rate of 0.5 to help reduce overfitting.
5. **Flatten:** Converts feature maps into a one-dimensional vector.
6. **Dense Layer:** 250 neurons with sigmoid activation.
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
| Training Loss | Approximately 1.25 |
| Training Accuracy | Approximately 66% |

These results provide a baseline for the current model. Further optimization of the architecture, activation functions, and input preprocessing may improve classification performance.

*Note: These are training metrics, not test-set results.*


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

## Future Work

The next step is to improve the model's performance and evaluate its accuracy on the unseen MNIST test set.
