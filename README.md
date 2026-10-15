# Heart Disease Data Preparation & Classification

Machine learning project investigating how different data preparation techniques affect heart disease classification performance.

## Project Overview
This project compares multiple data preparation strategies before building a Logistic Regression model for heart disease classification.

The experiments focus on:
- Missing-value handling
- Feature scaling
- Feature subset selection

## Data Preparation
The preprocessing workflow included:
- Missing-value checking
- Duplicate checking and removal
- Median imputation for numerical features
- Mode imputation for categorical features
- One-hot encoding for categorical variables
- Train/test splitting
- Feature scaling

## Experimental Design

### Round 1: Data Preparation
Compared combinations of:
- Missing-value handling
  - Drop missing observations
  - Median/Mode Imputation
- Feature scaling
  - No Scaling
  - Standardization
  - Normalization

The best data-preparation configuration from Round 1 was then used as the baseline for the next experiment.

### Round 2: Feature Selection
Recursive Feature Elimination (RFE) was used to compare different feature subset sizes:

- 16 features
- 13 features
- 9 features

Logistic Regression was used as the classification model throughout the experiments.

## Results

The best configuration was:

- Missing-value handling: Median/Mode Imputation
- Scaling: Standardization
- Feature selection: RFE
- Selected features: 13
- Training Accuracy: 86.21%
- Testing Accuracy: 86.00%
- Train-Test Gap: 0.21%

Reducing the number of features too aggressively resulted in lower classification performance.

## Tools
- Python
- pandas
- NumPy
- scikit-learn

## Key Learning
This project strengthened my understanding of:
- data preprocessing
- missing-value handling
- feature scaling
- feature selection
- Recursive Feature Elimination (RFE)
- Logistic Regression
- experimental comparison
- avoiding data leakage
