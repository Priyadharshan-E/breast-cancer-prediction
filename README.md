# breast-cancer-prediction
Machine learning project that predicts whether a breast tumor is malignant or benign using the Breast Cancer Wisconsin dataset. Compares Logistic Regression (98.25% accuracy) and Random Forest (95.61%) with feature scaling, confusion matrix and feature importance plot. Python, scikit-learn.
# Breast Cancer Prediction using Machine Learning

## Problem Statement
Predict whether a breast tumor is malignant (cancerous) or benign (non-cancerous) using measurements taken from patient tumor cells. Early and accurate detection can support doctors in diagnosis.

## Dataset
- Breast Cancer Wisconsin (Diagnostic) dataset, built into scikit-learn
- 569 samples, 30 numeric features (radius, texture, perimeter, area, smoothness, etc.)
- Target: 0 = Malignant, 1 = Benign

## Tools Used
Python, Pandas, Scikit-learn, Matplotlib, Google Colab, GitHub

## Approach
1. Loaded the dataset and created a DataFrame
2. Split data into 80% training and 20% testing (stratified)
3. Applied StandardScaler to scale features
4. Trained two models: Logistic Regression and Random Forest
5. Compared the models using accuracy, classification report and confusion matrix
6. Plotted the top 10 important features

## Results
|       Model         | Accuracy |
|---------------------|----------|
| Logistic Regression | 98.25%   |
| Random Forest       | 95.61%   |

**Confusion Matrix (Logistic Regression):**

|  | Predicted Malignant | Predicted Benign |
|------------------|----|----|
| Actual Malignant | 41 | 1  |
| Actual Benign    | 1  | 71 |

Logistic Regression gave the best result, with precision and recall of about 98% for both classes.

## Real-world Applications
AI is already used in healthcare for early cancer detection. This project is a simplified version using tabular data. Real systems use medical images with deep learning and need clinical validation before use.

## Project Plan
| Phase | Task | Time |
|-------|------|------|
| 1 | Problem selection and dataset study | 1 hr |
| 2 | Coding and model training | 2 hrs |
| 3 | Testing, comparison and documentation | 1 hr |

## Conclusion
Logistic Regression with feature scaling performed best (98.25%) on this dataset, showing that even simple models can predict tumor type accurately. This project demonstrates the complete ML workflow: data loading, preprocessing, training, evaluation and visualization.

## Limitation
The dataset is small (569 samples). The model is for learning purposes only and must not be used for real medical decisions.
