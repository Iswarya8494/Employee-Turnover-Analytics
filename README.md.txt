# Employee Turnover Prediction

## Project Overview

Portobello Tech has developed a machine learning-driven approach to predict employee turnover by analyzing various factors like employee satisfaction, project involvement, evaluation ratings, and work hours. This project aims to predict which employees are most likely to leave and help the HR Department make data-driven decisions for employee retention.

## Problem Statement

The company evaluates employee data periodically, including factors like the number of projects an employee worked on, work satisfaction, monthly hours, and salary levels. This information is used to predict employee turnover, with the ultimate goal of reducing attrition by identifying at-risk employees.

## Steps Involved

### 1. **Data Quality Checks**
- Check for missing values and handle them.
- Identify and address data inconsistencies or errors.

### 2. **Exploratory Data Analysis (EDA)**
- Correlation heatmap of numerical features.
- Distribution plots for satisfaction level, evaluation scores, and monthly work hours.
- Bar plots to compare the project count between employees who left and stayed.

### 3. **Clustering Analysis**
- Perform K-means clustering on employees who left, using satisfaction and evaluation scores.
- Visualize and analyze the clusters to understand patterns in employee behavior.

### 4. **Handling Class Imbalance**
- Use the SMOTE technique to balance the class distribution in the dataset.

### 5. **Model Training and Evaluation**
- Train and evaluate models using 5-fold cross-validation.
  - Logistic Regression
  - Random Forest Classifier
  - Gradient Boosting Classifier
- Evaluate the models using metrics like ROC/AUC and confusion matrix.

### 6. **Retention Strategies**
- Use the best-performing model to predict employee turnover probabilities.
- Suggest retention strategies based on the predicted probability scores:
  - Safe Zone (Green): Low risk of leaving.
  - Low-Risk Zone (Yellow): Moderate risk, require attention.
  - High-Risk Zone (Red): High risk of leaving, consider immediate intervention.

## Dataset

The dataset is based on employee information collected by the HR department at Portobello Tech and is modified from [Kaggle's HR dataset](https://www.kaggle.com/liujiaqi/hr-comma-sepcsv). It includes the following columns:
- `satisfaction_level`: Employee job satisfaction level.
- `number_project`: Number of projects an employee worked on.
- `last_evaluation`: Rating between 0 and 1 from the employee's last evaluation.
- `average_monthly_hours`: Average hours worked per month.
- `time_spent_company`: Number of years spent in the company.
- `work_accident`: Whether the employee had a work accident (0 or 1).
- `left`: Whether the employee left the company (0 or 1).
- `promotion_last_5years`: Number of promotions in the last 5 years.
- `department`: Department the employee belongs to.
- `salary`: Employee's salary level.

## Technologies Used

- Python
- Libraries: Pandas, NumPy, Scikit-learn, imbalanced-learn (SMOTE), Matplotlib, Seaborn
- Machine Learning Models: Logistic Regression, Random Forest, Gradient Boosting Classifier
- Jupyter Notebooks

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Iswarya8494/Employee-Turnover-Analytics.git
