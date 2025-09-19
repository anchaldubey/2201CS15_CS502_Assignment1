# Breast Cancer Prediction Using Support Vector Machine (SVM)

## Project Overview
This project uses a Support Vector Machine (SVM) model with a polynomial kernel to predict breast cancer malignancy. The model is trained on the Breast Cancer Wisconsin (Original) dataset and tuned for high classification accuracy.

## Dataset
- Breast Cancer Wisconsin (Original) dataset from UCI Repository.
- Contains 699 samples with 11 features describing cell nuclei characteristics.
- Target labels: 4 = malignant, 2 = benign.

## Data Preprocessing
- Dropped non-feature columns (`id` and `Class`).
- Converted `Bare Nuclei` column to numeric; missing values imputed with mean.
- Normalized features using z-score scaling.
- Binary encoding of target: malignant = 1, benign = 0.

## Model Training and Evaluation
- Train-test split: 70% training, 30% testing.
- Hyperparameter tuning using GridSearchCV over polynomial degree and penalty `C`.
- Best model parameters: `C=0.1`, degree `1`.
- Model achieved ~96.19% accuracy on the test set.
- Confusion matrix and feature correlation heatmap generated for analysis.
