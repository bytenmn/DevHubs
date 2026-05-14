# Iris Dataset — Task Summary

## Task objective

Summarize and demonstrate classification of the Iris dataset: explore feature distributions, build and compare supervised models to predict flower species, and identify which features are most informative.

## Dataset used

- Dataset: Fisher's Iris dataset (built-in in sklearn)
- Samples: 150
- Features: sepal length, sepal width, petal length, petal width
- Classes: setosa, versicolor, virginica

## Models applied

The notebook experiments with standard classification models, for example:

- Logistic Regression
- k-Nearest Neighbors (k-NN)
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

(See the notebook for exact model configurations and any additional models tried.)

## Key results and findings

- Models achieve strong performance on this dataset; typical accuracies are high (often >90%) with ensemble or SVM methods performing best.
- Petal length and petal width are the most discriminative features for separating species.
- Simple models (e.g., k-NN, logistic regression) perform well after basic preprocessing; ensembles improve stability.

For precise metrics, confusion matrices, and plots, open the notebook Iris_dataset.ipynb in this folder.

---
Notebook: Iris_dataset.ipynb
