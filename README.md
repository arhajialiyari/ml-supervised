# Supervised Machine Learning

This repository contains Jupyter notebooks demonstrating supervised machine learning classification methods and ROC curve analysis.

## Notebooks

### 1. Drug Classification
`drug_knn_nb_log_svm.ipynb`

**Goal:** Compare supervised learning models for multiclass drug classification.

- **Preprocessing:** Exploratory data analysis, feature encoding, standardization, and class balancing with SMOTE.
- **Models:** K-Nearest Neighbors (KNN), Gaussian Naive Bayes, Logistic Regression, and Support Vector Machine (SVM).
- **Evaluation:** Accuracy, macro-averaged Precision, Recall, F1-score, Confusion Matrix, and Classification Report.
- **Additional analysis:** KNN hyperparameter comparison, cross-validation, and multiclass ROC-AUC.

### 2. Binary ROC Curve
`ROC_Curve.ipynb`

**Goal:** Understand ROC curves and evaluate binary classification.

- **Model:** Gaussian Naive Bayes on synthetic data.
- **Evaluation:** Accuracy, Precision, Recall, Confusion Matrix, and ROC-AUC.
- **Techniques:** Probability-based ROC curves, threshold analysis, and comparison with hard-label predictions.

### 3. Multiclass ROC Curve
`ROC_Curve_Multiclass.ipynb`

**Goal:** Evaluate ROC-AUC for multiclass classification.

- **Model:** Random Forest on synthetic data.
- **Evaluation:** Per-class ROC-AUC and macro-averaged ROC-AUC.
- **Techniques:** One-vs-Rest (OvR), One-vs-One (OvO), probability distributions, and ROC visualization.

## Dataset

The drug classification notebook uses a dataset containing 200 records and 6 columns.

Source: [Drug Classification Dataset - Kaggle](https://www.kaggle.com/datasets/prathamtripathi/drug-classification)

The dataset is not included in this repository.

Download the dataset, save it as `drug_classification.csv`, and place it in the project root alongside the notebook.

The notebook expects the target column to be named `Drug_Type`. Rename the original `Drug` column if necessary.

The two ROC notebooks generate synthetic datasets and do not require external CSV files.

## Environment

- Python 3.12
- Jupyter Notebook
- scikit-learn
- imbalanced-learn
- NumPy, Pandas, Matplotlib, Seaborn

## Installation

Create a virtual environment and install the dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

Open the notebooks in Visual Studio Code and select the project's `.venv` Python interpreter.

## Disclaimer

This is an educational machine learning project. Its drug classification results are not medical advice and must not be used for clinical prescribing decisions.