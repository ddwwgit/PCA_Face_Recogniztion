# PCA-Based Face Recognition

## Overview
This project applies Principal Component Analysis (PCA) to implement a face recognition system. By extracting the most significant features from face datasets, the system creates eigenfaces and uses them to recognize faces in test images.

## Structure
data/: Directory for storing face images.
src/: Python scripts for the PCA transformation and face recognition.
models/: Trained PCA models and any other saved models.
requirements.txt: List of dependencies for the project.

## Requirements
- Python 3.7+
- Libraries: NumPy, Matplotlib, scikit-learn

## Dataset
The dataset used is the Labeled Faces in the Wild (LFW), which has been preprocessed to align and resize images for the PCA.

## Usage
1. Load the dataset: Adjust `min_faces_per_person` and `resize` to configure the dataset according to your requirements.
2. Train the PCA model: Run PCA on the training data to find the principal components.
3. Transform data: Project both training and testing data onto the PCA space to get their reduced representations.
4. Classification: Use a nearest neighbor approach to classify test images based on the Euclidean distance in PCA space.



