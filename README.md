# Job Recruitment Analysis - Part 2

This project involves a detailed analysis of a dataset related to job recruitment, focusing on data preprocessing, exploratory data analysis (EDA), and the application of machine learning models for prediction tasks.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Key Features](#key-features)
4. [Machine Learning Models](#machine-learning-models)
5. [Results](#results)
6. [Usage](#usage)
7. [Requirements](#requirements)
8. [Contributing](#contributing)
9. [License](#license)

---

## Introduction
This project demonstrates various steps in a data science workflow, including:
- Data cleaning and preprocessing.
- Feature engineering.
- Exploratory Data Analysis (EDA).
- Implementation and evaluation of machine learning models for prediction.

The analysis was performed in a Google Colab environment.

---

## Dataset
The dataset includes details of individuals such as:
- Age
- Education Level
- Employment Status
- Previous Salary
- Computer Skills
- Technical Expertise in Programming Languages, Frameworks, and Databases

The target variable is **Employed**, indicating the employment status of individuals.

---

## Key Features
1. **Data Preprocessing**:
   - Handled missing values.
   - Encoded categorical variables using Label Encoding.
   - Removed outliers using the IQR method.

2. **EDA**:
   - Visualized distributions of key variables.
   - Explored relationships between features and the target variable.
   - Checked for correlations between attributes.

3. **Feature Engineering**:
   - Grouped countries into continents.
   - Extracted technical expertise categories from a multi-valued field.

4. **Machine Learning Models**:
   - Logistic Regression
   - Decision Tree
   - XGBoost Classifier
   - Random Forest Classifier

---

## Machine Learning Models
Several models were trained and optimized using hyperparameter tuning (GridSearchCV). Performance metrics such as accuracy, precision, recall, F1-score, and ROC-AUC were used to evaluate each model.

---

## Results
Key findings from the model evaluation:
- **Logistic Regression**: AUC (Train) = 0.8652, AUC (Test) = 0.7699.
- **Decision Tree**: AUC (Train) = 0.9047, best parameters: `max_depth=10, min_samples_leaf=4, min_samples_split=10`.
- **XGBoost**: AUC = 0.8934, best parameters: `learning_rate=0.1, max_depth=3, n_estimators=200`.
- **Random Forest**: AUC = 0.9040, best parameters: `max_depth=10, min_samples_split=10, n_estimators=300`.

---

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/job-recruitment-analysis.git
