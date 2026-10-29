# MNIST Handwritten Digit Classification — PCA Comparison

## Project Overview

This project uses Python and Scikit-learn to classify handwritten digits from the MNIST dataset. It compares Logistic Regression models trained with and without Principal Component Analysis (PCA) to examine how dimensionality reduction affects classification accuracy and execution time.

## Technologies Used

- Python
- Scikit-learn
- Jupyter Notebook
- Logistic Regression
- Principal Component Analysis (PCA)
- StandardScaler

## Project Features

- Loaded the MNIST dataset containing handwritten digit images.
- Split the data into training (80%) and testing (20%) sets.
- Standardized features using StandardScaler.
- Trained a Logistic Regression model without PCA.
- Applied PCA to retain 95% of the training data's variance.
- Trained a second Logistic Regression model using PCA-transformed features.
- Compared classification accuracy and model training/prediction time.

## Results

| Metric | Without PCA | With PCA |
|---|---|---|
| Accuracy | 91.54% | 92.20% |
| Timed execution | 73.44 seconds | 61.67 seconds |
| Features/components | 784 | 330 |

In this experiment, the PCA-based model achieved slightly higher accuracy with a shorter measured training and prediction time. The PCA transformation time was not included in the timing comparison.

## How to Run

1. Open `Homework5_MNIST.ipynb` in Google Colab or Jupyter Notebook.
2. Ensure Python, Scikit-learn, and the required dependencies are available.
3. Run the notebook cells in order. Internet access may be needed to retrieve the MNIST dataset from OpenML.

## Project Background

This project was completed as part of my Computer Science coursework. I independently implemented the assignment using course materials and textbook references.
