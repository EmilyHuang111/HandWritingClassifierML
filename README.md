# Handwritten Letter Recognition with CNNs

This project aims to classify handwritten letters (A-Z) from images using a Convolutional Neural Network (CNN). The project involves preprocessing image data, training machine learning models, and tuning hyperparameters to improve model accuracy.

## Features
- Predict handwritten letters (A-Z) from images.
- Preprocessing pipeline to standardize image data:
  - Normalize and binarize images.
  - Resize images to 250x250 pixels.
  - Apply focal cropping and noise addition.
- Implemented two models for comparison:
  - Support Vector Machine (SVM)
  - Convolutional Neural Network (CNN)
- Hyperparameter tuning with RandomizedSearchCV for CNNs.

## Project Workflow
1. **Data Preprocessing**:
   - Standardized all images to JPEG format with `.jpg` extensions.
   - Cropped images to focus on handwritten letters.
   - Resized images to uniform dimensions of 250x250.
   - Converted to binary black-and-white format.
   - Added random noise and normalized pixel values.

2. **Model Development**:
   - Initial implementation of SVM and CNN models.
   - Evaluated CNN model performance pre- and post-hyperparameter tuning.

3. **Hyperparameter Tuning**:
   - Explored various combinations of learning rates, optimizers, dropout rates, kernel sizes, and number of filters.
   - Improved CNN accuracy through RandomizedSearchCV.

5. **Inference**:
   - The model predicts the letter from an image using the trained CNN.

## Limitations
- Small dataset size led to overfitting and poor generalization.
- Variability in handwriting styles, lighting, angles, and image quality reduced performance.
- The current preprocessing and cropping methods might not effectively focus on the handwritten letters.

## Potential Improvements
- Expand the dataset with diverse handwriting styles and better-quality images.
- Explore advanced image augmentation techniques like Gaussian blur and Canny edge detection.
- Optimize preprocessing steps to better align letters in the input images.
- Test alternative CNN architectures and hyperparameter combinations.

## Setup Instructions
1. Clone this repository.
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
