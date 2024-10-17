QUANTUM_MY_WORK 
---------------

# Detection of Sensitive Data Exposure in Images

This project builds a Convolutional Neural Network (CNN) to classify images as either sensitive or non-sensitive. The model is trained on a dataset of images and includes functionalities for data augmentation, early stopping, and model deployment for web applications.

## Table of Contents
- [1. Library Imports and Dataset Download](#1-library-imports-and-dataset-download)
- [2. Dataset Overview](#2-dataset-overview)
- [3. Image Visualization](#3-image-visualization)
- [4. Model Callbacks](#4-model-callbacks)
- [5. CNN Model Architecture](#5-cnn-model-architecture)
- [6. Model Compilation](#6-model-compilation)
- [7. Data Augmentation and Image Generation](#7-data-augmentation-and-image-generation)
- [8. Model Training](#8-model-training)
- [9. Plotting Accuracy and Loss](#9-plotting-accuracy-and-loss)
- [10. Confusion Matrix Calculation](#10-confusion-matrix-calculation)
- [11. Model Saving and Conversion](#11-model-saving-and-conversion)
- [12. Testing the Model with Uploaded Images](#12-testing-the-model-with-uploaded-images)
- [Conclusion](#conclusion)

## 1. Library Imports and Dataset Download
Import the necessary libraries for model creation, data processing, and visualization.

```python
import tensorflow as tf
import numpy as np
import os
from matplotlib import pyplot as plt

# Clone the dataset repository
git_folder = "/content/Detection-of-Sensitive-Data-Exposure-in-Images"
!git clone https://github.com/DhilipSanjay/Detection-of-Sensitive-Data-Exposure-in-Images.git
