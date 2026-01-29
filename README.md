# 📊 Credit Risk Prediction System – Home Credit Project

<div align="center">

![Credit Risk](https://img.shields.io/badge/Credit%20Risk-Analytics-2563eb?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Statistics](https://img.shields.io/badge/Statistical%20ML-Explainable-16a34a?style=for-the-badge)
![Finance](https://img.shields.io/badge/Finance-Regulator%20Friendly-7c3aed?style=for-the-badge)

*A statistically validated and interpretable credit risk prediction framework*

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Results](#-results--analysis) • [Contributing](#-contributing)

</div>

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Technology Stack](#-technology-stack)
- [Project Structure](#-project-structure)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Usage](#-usage)
- [Results & Analysis](#-results--analysis)
- [Statistical Validation](#-statistical-validation)
- [Future Scope](#-future-scope)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Overview

This project presents a **hybrid and interpretable credit risk prediction system** built using the **Home Credit Default Risk dataset**. The goal is to accurately predict borrower default risk while maintaining **statistical rigor, transparency, and auditability**, which are essential in regulated financial environments.

Unlike black-box machine learning approaches, this system integrates **classical statistical techniques** with machine learning to provide **explainable and reliable credit risk scores**.

---

## ✨ Features

### 📉 Dimensionality Reduction
- Principal Component Analysis (PCA) to handle high-dimensional financial data
- Reduces 100+ correlated features to 23 orthogonal components
- Retains approximately 90% of total variance

### 🧩 Borrower Segmentation
- Hierarchical (Agglomerative) Clustering on PCA-transformed data
- Identifies meaningful borrower groups with shared risk characteristics
- Dendrogram-based cluster selection

### 📊 Statistical Validation
- One-way ANOVA to validate cluster separability
- Cronbach’s Alpha to assess feature reliability
- Ensures statistical significance and internal consistency

### 📐 Interpretable Risk Models
- Linear Discriminant Analysis (LDA)
- Quadratic Discriminant Analysis (QDA)
- Logistic Regression as a baseline comparison

### 📈 Bayesian Risk Estimation
- Gaussian Naïve Bayes for probabilistic default prediction
- Outputs posterior probability of default
- Enables threshold-based risk decisions

---

## 🛠 Technology Stack

### Core Technologies
- **Python** – Primary programming language
- **NumPy & Pandas** – Data manipulation and analysis
- **Scikit-Learn** – PCA, clustering, and classification models
- **SciPy** – Statistical testing (ANOVA)
- **Matplotlib / Seaborn** – Data visualization

### Development Environment
- Jupyter Notebook / Google Colab
- Conda / pip for dependency management

---

## 📁 Project Structure

