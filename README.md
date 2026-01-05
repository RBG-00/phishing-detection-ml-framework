# A Machine Learning-Based Framework for Phishing Website and URL Detection

This repository presents a unified machine learning framework for detecting phishing websites and phishing URLs using supervised learning models.  
The framework emphasizes **experimental consistency**, **robust evaluation**, and **model interpretability** through feature importance analysis.

---

## 📌 Overview

Phishing attacks remain one of the most critical cybersecurity threats, exploiting deceptive websites and malicious URLs to steal sensitive information.  
Traditional rule-based and blacklist-based approaches often fail to detect newly generated or obfuscated phishing content.

This project proposes a **consistent and interpretable machine learning framework** that:
- Applies the same experimental pipeline across multiple datasets
- Uses F1-score to address class imbalance
- Integrates feature importance analysis to enhance explainability

---

## 🧠 Methodology

The proposed framework follows a unified experimental pipeline applied consistently across both datasets:

1. Data preprocessing and cleaning  
2. Feature extraction (lexical, structural, and behavioral features)  
3. Feature selection and ranking  
4. Model training using supervised machine learning classifiers  
5. Model evaluation using stratified cross-validation  
6. Feature importance analysis using Random Forest  

---

## 📊 Machine Learning Models

The following classifiers were evaluated:

- Logistic Regression  
- Support Vector Machine (SVM)  
- k-Nearest Neighbors (kNN)  
- Naive Bayes  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- AdaBoost  
- Neural Networks  

All models were trained and evaluated using identical experimental settings to ensure fair and reproducible comparison.

---

## 🗂️ Datasets

Two datasets were used in this study:

- **Phishing Website Dataset**  
- **Phishing URL Dataset**

Each dataset contains both phishing and legitimate samples and was processed independently while following the same experimental pipeline.

> ⚠️ Datasets are not included in this repository due to usage restrictions.  
> Please refer to the original sources cited in the paper.

---

## 📈 Evaluation Strategy

- Stratified 10-fold cross-validation  
- Primary metric: **F1-score** (to handle class imbalance)  
- Additional metrics: accuracy and confusion matrices  

---

## 🔍 Feature Importance Analysis

Given the negligible performance differences among high-performing classifiers, **Random Forest** was selected for feature importance analysis due to its robustness and interpretability.

The analysis highlights the most influential features contributing to phishing detection, providing insights into common phishing patterns such as abnormal URL structures and suspicious lexical characteristics.

---

## 📄 Paper

The full research paper is available in the repository:

