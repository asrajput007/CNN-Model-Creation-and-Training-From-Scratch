# CNN-Model-Creation-and-Training-From-Scratch
This repository contains scripts for creating Convolutional Neural Network (CNN) models from scratch, compiling them, training and testing them, and plotting performance curves. The models are created using the Keras library, with various layers such as Conv2D, MaxPooling2D, Dense, and Flatten.

## Libraries Used

The following libraries are imported for various tasks:

* **Keras**: Used for image preprocessing and model creation.
* **TensorFlow**: Provides backend support for Keras.
* **NumPy**: Used for numerical operations.
* **Matplotlib**: Used for visualization of images and performance curves.

## Model Creation

The CNN models are created using Keras layers such as Conv2D, MaxPooling2D, Flatten, and Dense. The model architecture is defined as follows:

1. Two convolutional layers with 3x3 filters and ReLU activation.
2. Max pooling layers with 2x2 filters.
3. Flatten layer to convert the 2D feature maps into a 1D vector.
4. Dense layers with ReLU activation.
5. Output layer with softmax activation for multiclass classification.

## Data Preparation

The input images are resized to 64x64 pixels. The dataset is split into training, validation, and test sets with the following proportions:

* Training Set: 70%
* Validation Set: 20%
* Test Set: 10%

The images are normalized to the range [0, 1] using the `ImageDataGenerator` class from Keras.

## Model Compilation and Training

The model is compiled using the Adam optimizer with a learning rate of 0.0001 and categorical cross-entropy loss. The accuracy metric is used to evaluate model performance during training.

The training process is visualized using Matplotlib, showing the training and validation accuracy and loss curves over epochs.

## Execution

To execute the script, run the provided Python script file. Ensure that you have the necessary libraries installed and the dataset available at the specified paths. Adjust the hyperparameters as needed for your specific task.

Feel free to explore the code and modify it according to your requirements!
