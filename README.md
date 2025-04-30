# Brain Tumor Classification Using Convolutional Neural Networks (CNN)

This project implements a machine learning-based solution for classifying brain tumors from MRI scans using Convolutional Neural Networks (CNN). The goal of this project is to automatically classify MRI images into different tumor types to aid in early diagnosis and treatment.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation Instructions](#installation-instructions)
- [How to Run the Project](#how-to-run-the-project)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)

## Introduction

Brain tumor detection is an important field in medical imaging, as early detection can significantly impact patient outcomes. This project uses a Convolutional Neural Network (CNN) to classify brain MRI images into one of four categories:
- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

The model is trained on a labeled dataset of MRI images and uses transfer learning to improve performance.

## Features

- **Four-Class Classification**: Classifies MRI images into 4 categories.
- **Encrypted Dataset**: Ensures privacy by encrypting images before processing.
- **Memory Efficient**: Optimized for handling large datasets without consuming excessive memory.
- **Transfer Learning**: Can be extended with pre-trained models for improved accuracy.
- **Model Visualization**: Provides tools to visualize model architecture and performance metrics.

## Technologies Used

- **Python**: Main programming language.
- **TensorFlow & Keras**: For building and training the CNN model.
- **Scikit-learn**: For model evaluation and metrics.
- **Matplotlib & Seaborn**: For visualizations of results and training history.
- **Cryptography**: For encrypting and decrypting images.
- **Google Colab**: Utilized for training the model on GPU.

## Installation Instructions

To run this project on your local machine, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Nischal0904/brain-tumor-classification.git
2.Navigate to the project directory:
  cd brain-tumor-classification
  
3.Install the required dependencies:
  pip install -r requirements.txt

If you don’t have the requirements.txt file, you can manually install the required libraries:
  pip install tensorflow pandas numpy matplotlib seaborn scikit-learn cryptography

## How to Run the Project

### 1. Prepare the Dataset
Ensure that the MRI dataset is organized into directories with the following class labels:
- **glioma**
- **meningioma**
- **pituitary_tumor**
- **no_tumor**

### 2. Run the Model

1. Open the Jupyter notebook `brain_tumor_classification.ipynb`.
2. Run all the code cells. This will:
   - Load the dataset
   - Preprocess the data
   - Train the CNN model
   - Save the trained model to `brain_tumor_classifier.h5`.

### 3. Evaluate the Model

The model will be evaluated on a test set, and you will see the following evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-Score

Additionally, the notebook will display visualizations like:
- Loss and accuracy curves
- Confusion matrix

## Model Architecture

The model consists of the following layers:
- **Conv2D Layers**: Used for feature extraction from MRI images.
- **MaxPooling2D Layers**: Reduces the dimensionality of the data.
- **Dense Layers**: Classifies the extracted features into respective tumor categories.
- **Dropout Layer**: Prevents overfitting during training.

### Model Summary:
- Input: MRI images (256x256 px, RGB)
- Output: 4 classes (Glioma, Meningioma, Pituitary Tumor, No Tumor)

## Results

- **Test Accuracy**: 95%
- **Precision, Recall, F1-Score**: Provided in the evaluation section of the notebook.
- **Confusion Matrix**: Provides a visual representation of the classification results.
- **Training Curves**: Visualizes the accuracy and loss during training.

## Contributing

Contributions are welcome! If you'd like to improve this project, you can:
- Experiment with different CNN architectures.
- Implement data augmentation techniques.
- Add more advanced evaluation metrics or visualizations.

Feel free to fork the repository, make changes, and submit a pull request.

  
