# Geometric Shape Recognition

This project explores the use of Machine Learning techniques for the automatic classification of geometric shapes represented as sequences of 2D points.

The goal is to develop and evaluate classifiers capable of recognizing four different geometric shapes:
- **Ellipses**
- **Rectangles**
- **Line segments**
- **Crosses** (two orthogonal intersecting segments)

## Dataset

A synthetic dataset is generated programmatically, with each shape represented as an ordered sequence of 2D points describing its contour. Gaussian noise is introduced to simulate imperfect observations and evaluate the robustness of the classification models.

## Methodology

The project investigates different approaches to feature representation and dimensionality reduction:

- **Feature Engineering:** extraction of geometric properties, including angles, distances and perimeter-related features.
- **Feature Selection:** identification of the most relevant features for classification.
- **Principal Component Analysis (PCA):** dimensionality reduction of the explicit coordinate representation.

Several Machine Learning models are implemented and compared:
- Support Vector Machines (SVM)
- Random Forest
- Logistic Regression
- Multi-Layer Perceptron (MLP)

Model selection and hyperparameter optimization are performed using Grid Search and cross-validation.

## Robustness Analysis

The models are further evaluated under different experimental conditions, investigating the impact of:
- Dataset size
- Number of points used to represent each shape
- Noise level

## Binary Classification

The project also explores a simplified binary classification task, distinguishing between shapes with a non-zero area (ellipses and rectangles) and shapes without area (line segments and crosses).

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Seaborn
