# Employee Churn Prediction – People Analytics

## Project Overview

This project focuses on predicting employee attrition using machine learning techniques. The goal is to analyze HR data and build a predictive model that identifies employees who are likely to leave the company.

The analysis follows a complete data science workflow including data preprocessing, feature engineering, model training, and evaluation.

---

## Dataset

The dataset used in this project is the **IBM HR Analytics Employee Attrition Dataset**, which contains demographic, job-related, and performance-related information about employees.

Target variable:

- **Attrition**: Indicates whether an employee left the company (Yes = 1, No = 0)

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-Learn  
- Matplotlib / Seaborn  
- Jupyter Notebook  
- Git & GitHub  

---

## Project Structure

people-analytics-employee-churn/
│
├── data/
│ └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── notebooks/
│ └── churn_analysis.ipynb
│
├── src/
│
└── README.md


---

## Methodology

The project followed these main steps:

1. **Data Cleaning and Preprocessing**
   - Removal of non-informative columns
   - Encoding of categorical variables
   - Standardization of numerical features

2. **Exploratory Data Analysis**
   - Distribution of the target variable
   - Identification of key patterns related to attrition

3. **Model Training**
   - Train/Test split with stratification
   - Logistic Regression model
   - Feature scaling with StandardScaler

4. **Model Evaluation**
   - AUC-ROC score
   - Precision, Recall, F1-score
   - Confusion Matrix

---

## Model Results

The final model achieved the following performance:

- **AUC-ROC:** 0.80  
- **Accuracy:** 0.87  

Key observations:

- The dataset is imbalanced (more employees stayed than left)
- The model performs well identifying non-attrition cases
- Recall for attrition class can be improved in future iterations

---

## Feature Importance

The most influential factors associated with attrition included:

- Overtime  
- Years since last promotion  
- Department  
- Years with current manager  
- Job satisfaction  

These insights can be useful for HR decision-making and retention strategies.

---

## How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/denpareja/people-analytics-employee-churn.git
Install dependencies:

pip install -r requirements.txt
Open the notebook:

jupyter notebook notebooks/churn_analysis.ipynb
Future Improvements
Possible enhancements for future versions:

Try additional models such as Random Forest or XGBoost

Apply techniques to handle class imbalance

Hyperparameter tuning

Build an interactive dashboard

Author
Denisse Pareja

Data Science Student – TripleTen
Miami, FL
