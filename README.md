# Traffic Sign Detection

## Description

This project implements a traffic sign classifier using the German Traffic Sign Recognition Benchmark (GTSRB) dataset. The primary goal is to build a neural network using TensorFlow that can classify images of traffic signs into one of 43 categories. The project involves working with computer vision techniques and experimenting with neural network architectures.

## Overview

The implementation consists of two key functions:
1. load_data: Processes the dataset by loading images and their corresponding labels, resizing the images to a consistent size, and preparing them for training.
2. get_model: Defines and compiles a Convolutional Neural Network (CNN) to classify the images based on the provided categories.

The project includes:
- Preprocessing the data using OpenCV to ensure all images are the same size.
- Experimentation with CNN architectures, including layers for convolution, pooling, dense connections, and dropout.
- Training and evaluation of the model to achieve high accuracy on the dataset.

### Technologies used:
- TensorFlow: For building and training the neural network.
- OpenCV: For image processing (loading and resizing images).
- NumPy and Scikit-learn: For data handling and splitting.

### Challenges faced:
- Balancing model complexity to prevent overfitting or underfitting.
- Achieving efficient preprocessing for thousands of images.

### Future implementations:
- Data Augmentation: Add transformations like rotation or brightness adjustment.
- Hyperparameter Tuning: Experiment with learning rates, batch sizes, and optimizers.
- Real-Time Deployment: Integrate the model with live video feeds for real-world use.

## Installation

1. Clone the repository:
    ```
    git clone https://github.com/yourusername/traffic.git
    ```
2. Navigate to the project directory:
    ```
    cd traffic
    ```
3. Setup the virtual environment:
    ```
    python3.9 -m venv venv
    source venv/bin/activate
    ```
4. Upgrade pip:
    ```
    pip install --upgrade pip
    ```
5. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

## Usage

1. Train the model:
```
python3 traffic.py gtsrb model.h5
```
2. Use the model:
```
from tensorflow.keras.models import load_model
model = load_model("model.h5")
```
3. Deactive virtual environment:
```
deactivate
```