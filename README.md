# Sampling Techniques and Model Evaluation

## Overview

This project demonstrates the implementation of various sampling strategies and machine learning models to address class imbalance and evaluate model performance. The primary focus is on analyzing how different sampling techniques influence model accuracy.

## Steps Implemented

### 1. Dataset Balancing
- **Minority Class Upsampling**: The minority class was upsampled using `sklearn.utils.resample` to balance the dataset and reduce bias in predictions.

### 2. Sampling Techniques
Five sampling techniques were applied to create varied subsets:
- **Random Sampling**: 20% of the dataset selected randomly.
- **Stratified Sampling**: Split the dataset while preserving class distribution using `train_test_split` with the `stratify` parameter.
- **Systematic Sampling**: Every 5th record selected.
- **Cluster Sampling**: One sample selected from each group based on the `Time` feature.
- **SMOTE**: Synthetic samples generated for the minority class.

### 3. Machine Learning Models
The following models were trained and evaluated across all samples:
- Random Forest Classifier
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)

### 4. Model Evaluation
Models were evaluated using **Accuracy**, the primary metric for comparing performance across sampling techniques.

### 5. Results Analysis
Performance (accuracy) was analyzed for each combination of sampling technique and model to identify the best-performing combination.

## Results

- Accuracy scores for each model across all sampling techniques.
- Identification of the optimal sampling and model combination.

## Conclusion

This project demonstrates the importance of balancing datasets and evaluates the effect of various sampling techniques on model accuracy, providing insights into the most effective strategies for handling class imbalance.

## Dependencies

- Python 3.x
- Pandas
- Scikit-learn
- Imbalanced-learn
