---
runme:
  id: 01HFXK7034X1XD8BF1KKAM40AE
  version: v2.0
---

# Tumor Classification Project

## Project Overview

This project aims to classify brain tumor images into four categories: glioma_tumor, meningioma_tumor, no_tumor, and pituitary_tumor. The classification is performed using machine learning algorithms from the scikit-learn library.

## Training Dataset

The training dataset consists of brain tumor images categorized into the following classes:

- glioma_tumor
- meningioma_tumor
- no_tumor
- pituitary_tumor

The images are preprocessed by resizing them to a fixed size of 64x64 pixels and converting them to grayscale.

## Classification Algorithm

The scikit-learn library is utilized for implementing the tumor classification. Three classifiers are considered in this project:

1. **Support Vector Machine (SVM)**: A powerful classification algorithm suitable for both linear and non-linear data.

2. **Logistic Regression**: A simple and efficient linear classification algorithm.

3. **Random Forest**: An ensemble learning method that constructs a multitude of decision trees and outputs the class that is the mode of the classes.

## Hyperparameter Tuning

Grid search is employed to find the best hyperparameters for each classifier. The hyperparameters tuned include:

- For SVM: The choice of kernel ('linear' or 'rbf') and the regularization parameter 'C'.
- For Logistic Regression: The regularization parameter 'C'.
- For Random Forest: The number of trees in the forest ('n_estimators').

The grid search is performed using cross-validation to find the combination of hyperparameters that results in the highest accuracy on the training dataset.

## Reproducibility

To ensure reproducibility, a fixed random seed of 42 is set where applicable. This ensures that the random processes involved in the training and evaluation of the models are consistent across different runs.

## How to Use

1. Ensure that the required libraries are installed:

```sh
pip install scikit-learn scikit-image matplotlib numpy
```

Copyright and Licensing Information
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact Information
For questions or inquiries, please contact:

Valentin Durieux

valentin.durieux@epitech.eu

50231621