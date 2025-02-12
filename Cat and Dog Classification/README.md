
Cat and Dog Image Classification Using CNN

This repository contains a deep learning project to classify images of cats and dogs using a Convolutional Neural Network (CNN). The project includes training a model on labeled data, evaluating its performance, and making predictions on unseen images.


Overview

This project builds a binary image classification model to identify whether an image contains a cat or a dog. The dataset is preprocessed to improve generalization, and a CNN model is trained using TensorFlow and Keras.

Dataset

- Source: The dataset used for training consists of labeled images of cats and dogs. You can use publicly available datasets such as the [Kaggle Dogs vs. Cats Dataset](https://www.kaggle.com/c/dogs-vs-cats/data).

- Images are resized to 150x150 pixels for training.


Model Architecture

The Convolutional Neural Network (CNN) used for this project has the following structure:

1. Input Layer: Images of size (150, 150, 3).
2. Convolutional Layers: 5 blocks of Conv2D layers with ReLU activation and MaxPooling.
3. Batch Normalization: Added after each convolutional layer for stable training.
4. Fully Connected Layers:
   - Flatten layer to convert 2D feature maps to 1D.
   - Dense layers with 128 and 64 neurons.
   - Dropout layers to reduce overfitting.
5. Output Layer: Single neuron with a sigmoid activation function for binary classification.

Training

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Metrics: Accuracy
- Epochs: 25
- Validation: Separate validation data is used for performance tracking during training.
- Checkpointing: The best model weights are saved based on validation accuracy.


Evaluation

- Metrics:
  - Validation Accuracy
  - Validation Loss
- The trained model is evaluated on unseen test images.
- Plots of training vs. validation accuracy and loss are included for analysis.


Results

Performance
- Validation Accuracy: ~89.84%
- Validation Loss: ~0.4097





