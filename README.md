# Credit Card Fraud Detection

![image](https://user-images.githubusercontent.com/88694623/236975512-6c75d83a-3e45-43b7-a5dd-e0691a7ff5ee.png)

This project aims to create a model to detect fraudulent transactions in credit card transactions.

## Getting Started
### Prerequisites
- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, sklearn, scipy, imblearn

### Installation
- Clone the repository
```
git clone https://github.com/username/project.git
```
- Install required libraries
```
pip install pandas numpy matplotlib seaborn sklearn scipy imblearn
```

## Usage
Run the following command in the terminal to execute the project:
```
python main.py
```

## Overview of the Code

### 1. Exploratory Data Analysis

- Loading data
- Printing random sample of 10 rows to check data loading
- Printing data overview
- Printing numerical summary for Time and Amount columns
- Plotting distribution of Time feature
- Plotting distribution of Amount feature
- Counting number of fraud vs non-fraud transactions and displaying them with their ratio
- Plotting count of fraud vs non-fraud transactions in a bar chart

### 2. Data Processing

- Plotting heatmap to find any high correlations between variables

### 3. Modeling

- Drop the 'Class' column to prepare data for splitting
- Get the target variable
- Split data into training, validation and test sets, ensuring the class distribution is maintained
- Initialize the `StandardScaler` object and fit it to the training data
- Scale the training, validation, and test sets using the scaler
- `Undersampling` will be utilized to address the issue of imbalanced classes.

## Modeling Techniques

### 1. Logistic Regression

- Run CV with 5 folds (logit)
- Instantiate RandomUnderSampler

### 2. Naive Bayes
- Fit a Naive Bayes Model

