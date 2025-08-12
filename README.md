# Predictive-Modelling-of-Distillation-Column-performance-using-sensor-data

## Overview
This project focuses on using artificial intelligence (AI) and machine learning (ML) to create a predictive model for a distillation column's performance. The model predicts key performance indicators, such as the mole fractions of TX and HX components, to improve process stability and efficiency. The research uses synthetic data from **Aspen HYSYS** to simulate real-time operating conditions for model training and testing.

***

## Problem Statement
Distillation column performance is critical for optimizing product quality and minimizing energy use. Current methods lack real-time adaptability, so this project developed a predictive model to estimate key component mole fractions under various conditions. The model is intended to enhance operational autonomy, allowing chemical plants to anticipate changes in performance and respond preemptively.

***

## Methodology
The methodology for this project involved several steps:
1.  **Data Collection & Preprocessing**: The data was sourced from Kaggle and included parameters such as pressure, temperature, and component concentrations. The data was cleaned, normalized, and missing values were handled to prepare it for model training.
2.  **Model Selection**: Several machine learning models, including regression models and neural networks, were evaluated. The **Random Forest model** was chosen for its superior accuracy in predicting `MoleFractionTX` and `MoleFractionHX`.
3.  **Training & Testing**: The Random Forest model was trained on the processed data and validated using a separate test set to ensure its predictive capability.
4.  **Evaluation**: The model's effectiveness was assessed using performance metrics such as accuracy.

***

## Results & Discussion
The Random Forest model showed high prediction accuracy for both target variables.
* `MoleFractionTX`: **Prediction Accuracy = 99.52%**
* `MoleFractionHX`: **Prediction Accuracy = 99.50%**

The project successfully developed a model that can forecast critical distillation column parameters, which helps in industrial process automation. The predictions allow operators to make timely adjustments, improving product quality, decision-making, and energy efficiency. The model also provides real-time monitoring and anomaly detection for enhanced safety.

## Challenges & Solutions
The project faced challenges that were addressed with the following solutions:
* **Data Quality**: The initial dataset lacked sufficient variability, so it was augmented with additional diverse data points to improve model robustness.
* **Model Overfitting**: Regularization techniques, such as dropout layers, were used to prevent overfitting and ensure the model generalized well to unseen data.
* **Computational Load**: The high computational demands were managed by optimizing code for efficiency and using batch processing to handle data in a memory-efficient manner.
