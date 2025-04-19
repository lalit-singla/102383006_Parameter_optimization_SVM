# Parameter-optimization-of-Support-vector-machine-SVM-

# Abalone Age Prediction Using SVR

This project aims to predict the **age of abalone** using **Support Vector Regression (SVR)** on physical measurements. The age of an abalone is traditionally determined by counting the number of rings in its shell—a labor-intensive process. This project explores how machine learning can be used to predict age using measurable attributes such as length, diameter, height, and weight.

## Dataset Information

- **Dataset Name**: Abalone
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/abalone)
- **Number of Instances**: 4177  
- **Number of Attributes**: 8 (excluding the target variable)

### 🎯 Target
- **Rings**: Number of rings in the abalone shell, used as a proxy for age.


## 📊 Problem Statement

> Predict the age of abalone using physical features to avoid the manual and tedious task of ring counting. The goal is to use SVR with kernel tuning and hyperparameter optimization to maximize prediction accuracy.

---

## 🛠️ Methodology

### 📌 Steps Followed:
1. **Data Preprocessing**:
   - Encoded categorical features (e.g., `Sex`)
   - Normalized feature values
2. **Modeling**:
   - Used **Support Vector Regression (SVR)**
   - Kernels tested: `linear`, `poly`, `rbf`, `sigmoid`
3. **Hyperparameter Tuning**:
   - Optimized **nu** and **epsilon** for SVR
   - Grid Search or Random Search methods used to find optimal values
4. **Evaluation**:
   - Accuracy measured per sample
   - Best kernel and parameter combination recorded for each run

---

## 🔍 Results

| Sample | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
|--------|----------------|--------------|----------|----------------|
| 1      | 0.26           | rbf          | 9.29     | 8.41           |
| 2      | 0.28           | rbf          | 8.94     | 3.67           |
| 3      | 0.27           | rbf          | 7.19     | 1.47           |
| 4      | 0.27           | rbf          | 9.98     | 4.00           |
| 5      | 0.27           | rbf          | 5.35     | 5.27           |
| 6      | 0.27           | rbf          | 6.52     | 9.33           |
| 7      | 0.27           | linear       | 2.06     | 2.63           |
| 8      | 0.26           | rbf          | 2.75     | 4.60           |

> 🔎 **Observation**: The **RBF kernel** consistently performed the best across most samples.

---

## 📈 Convergence Graph

A convergence graph was generated to visualize how accuracy changed during the optimization process. *(Insert your convergence plot here in the README)*

---

## 🧠 Technologies Used

- Python 🐍
- scikit-learn 🤖
- NumPy 📊
- Matplotlib 📉
- Pandas 📁

---



![image](https://github.com/user-attachments/assets/4bdc5cd8-9174-44ad-a4bf-a80f83e53243)
