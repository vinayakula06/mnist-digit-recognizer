# mnist-digit-recognizer
I'll update the README to reflect the use of the LeNet-5 model:

---

# MNIST Digit Recognizer

This project implements a handwritten digit recognition model using the classic LeNet-5 architecture on the MNIST dataset. The model is developed in PyTorch to classify images of digits (0-9).

## Table of Contents
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Code Components](#code-components)
- [Usage](#usage)
- [Results](#results)


## Requirements
To run this project, you’ll need the following libraries:
- `torch`
- `torchvision`
- `pandas`
- `numpy`

Install dependencies with:
```bash
pip install torch torchvision pandas numpy
```

## Project Structure
- `mnist-digit-recognizer.ipynb`: The main notebook implementing the MNIST digit recognition model.
- `README.md`: Project documentation (this file).

## Dataset
The MNIST dataset consists of 28x28 grayscale images of handwritten digits. Each image is reshaped to fit the input layer requirements of the LeNet-5 model.

## Code Components

### 1. **Custom Dataset Class**
The `CustomImageDataset` class processes and loads the MNIST data compatible with PyTorch’s dataset format, applying transformations if specified.

### 2. **LeNet-5 Model Architecture**
This project uses the LeNet-5 convolutional neural network (CNN) architecture, which is highly effective for image recognition tasks. The architecture includes:
- **Convolutional Layers** for feature extraction.
- **Pooling Layers** to reduce spatial dimensions.
- **Fully Connected Layers** to classify the extracted features.

### 3. **Training and Evaluation**
The training process involves:
- Data loading with PyTorch’s `DataLoader`.
- Loss computation and gradient updates for optimization.
- Evaluation on the test set to measure model accuracy.

## Usage
Run the notebook `mnist-digit-recognizer.ipynb` to:
1. Load the MNIST data.
2. Initialize, train, and evaluate the LeNet-5 model.

## Results
The model’s performance is measured in terms of accuracy and loss, providing insight into its effectiveness on the MNIST dataset.
