# 🛡️ Support Vector Classifier (SVC) Implementation

This repository contains a comprehensive implementation and evaluation of the **Support Vector Classifier (SVC)** using Scikit-Learn. The project explores the impact of different mathematical kernels and the regularization parameter (C) on model accuracy.

## 🚀 Project Overview

Support Vector Machines (SVM) are powerful supervised learning models used for classification. This project demonstrates how to implement an SVC and fine-tune its hyperparameters to achieve the best possible decision boundary.

### Key Highlights:
* **Kernel Exploration:** Compared the performance of **RBF (default)**, **Linear**, **Polynomial**, and **Sigmoid** kernels.
* **Hyperparameter Tuning:** Conducted a manual search over various `C` values (Regularization parameter) to observe the trade-off between margin width and misclassification.
* **Feature Scaling:** Optimized model performance by using scaled training and testing data (`X_train_scaled`, `X_test_scaled`).

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy
* **Algorithm:** Support Vector Classifier (SVC)

---

## 📊 Performance Analysis

The model was evaluated using standard metrics including Accuracy, Precision, Recall, and F1-Score.

### 1. Kernel Comparison
| Kernel | Accuracy |
| :--- | :--- |
| **RBF (Default)** | **93.33%** |
| **Linear** | 91.11% |
| **Sigmoid** | 91.11% |
| **Polynomial** | 86.67% |

### 2. Tuning the Regularization Parameter (C)
By adjusting the `C` value with the RBF kernel, the following accuracies were observed:
* **C=1.0, 4.0, 5.0:** Achieved the peak accuracy of **93.33%**.
* **C=0.5, 2.0, 3.0:** Achieved an accuracy of **91.11%**.

### 📝 Classification Report (Best Model)
```text
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        15
           1       0.88      0.93      0.90        15
           2       0.93      0.87      0.90        15

    accuracy                           0.93        45
