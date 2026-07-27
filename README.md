[README .md](https://github.com/user-attachments/files/30399523/README.2.md)
# Breast Cancer Classification using Neural Networks

A simple Artificial Neural Network (ANN) built with **TensorFlow / Keras** that classifies breast tumors as **Malignant** or **Benign**, based on 30 diagnostic measurements from digitized images of a fine needle aspirate (FNA).

---

## Overview

| | |
|---|---|
| Dataset | Breast Cancer Wisconsin (Diagnostic) — via `sklearn.datasets.load_breast_cancer()` |
| Samples | 569 (212 malignant / 357 benign) |
| Features | 30 numeric measurements (radius, texture, perimeter, area, smoothness, etc.) |
| Model | `Flatten → Dense(20, ReLU) → Dense(2, Sigmoid)` |
| Optimizer / Loss | Adam / Sparse Categorical Crossentropy |
| Epochs | 10 |
| **Test Accuracy** | **96.5%** |

---

## Repository Contents

```
├── Breast_Cancer_Classification_with_Neural_Network.ipynb   # full notebook (code + outputs)
├── Breast_Cancer_Classification_Report.docx                 # project report
└── Breast_Cancer_Classification_Presentation.pptx           # 10-slide summary deck
```

---

## Project Workflow

1. Load the dataset and convert it into a Pandas DataFrame
2. Explore the data — shape, missing values, class balance
3. Split features (X) from the target label (Y)
4. Train/test split — 80% / 20%
5. Standardize features using `StandardScaler`
6. Build and train the neural network
7. Evaluate on the test set
8. Build a predictive system for classifying a single new sample

---

## How to Run

No manual dataset download needed — it loads directly from scikit-learn.

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
jupyter notebook Breast_Cancer_Classification_with_Neural_Network.ipynb
```

Run all cells top to bottom (Kernel/Runtime → Run all).

---

## Result Summary

- **Training accuracy:** ~97.2%
- **Validation accuracy:** ~95.7%
- **Test accuracy:** ~96.5%
- **Test loss:** ~0.11

The model performs comparably to classical baselines (e.g. logistic regression) on this dataset, with feature standardization being the key preprocessing step for good performance.

> **Note:** This model is intended as a decision-support demonstration and is not a substitute for professional medical diagnosis.

---

## Stack

`Python` · `TensorFlow / Keras` · `scikit-learn` · `Pandas` · `NumPy` · `Matplotlib`

---

*Submitted as part of an internship program, July 2026.*
