# 🐱🐶 Cats vs Dogs Classification

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images of cats and dogs. The dataset was sourced from Kaggle, and the pipeline includes custom preprocessing, grayscale conversion, and image standardization — followed by model training and evaluation.

## 📦 Dataset
The dataset can be found on Kaggle: [(Cats-vs-Dogs)](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset) \
Contains labeled images of cats and dogs. \
Originally in color (RGB) with varying resolutions.

## 🧹 Data Processing Pipeline
A custom function was created to handle the image loading and preprocessing:
- **Load Images**: Read images from local directories.
- **Padding**: Add borders to make images square without distortion.
- **Resize**: All images resized to a consistent shape.
- **Grayscale Conversion**: Reduced image complexity for faster training.
- **Dataset Split**: Images split into training and testing sets.
- **Saving**: Final processed data saved in .npz format for efficient reloading.

## 🔧 Model & Training (PyTorch)
Implemented a simple CNN architecture using PyTorch.
Used standard layers: Conv2D, MaxPooling, ReLU, and Fully Connected layers.
Trained on the preprocessed grayscale images.
Evaluated performance using accuracy on the test set.

## 🧪 Future Improvements
- Add data augmentation (flipping, rotations, etc.).
- Improve performance through hyperparameter tuning.
- Add evaluation metrics (precision, recall, F1-score, confusion matrix).
