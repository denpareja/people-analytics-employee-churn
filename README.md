# Employee Churn Prediction – People Analytics

## Project Overview

This project focuses on predicting employee attrition using machine learning techniques. The goal is to analyze HR data and build a predictive model capable of identifying employees who are at risk of leaving the company.

The analysis follows a complete data science workflow including:

- Data preprocessing  
- Exploratory data analysis  
- Feature engineering  
- Model training  
- Model evaluation  

---

## Dataset

The dataset used in this project is the **IBM HR Analytics Employee Attrition Dataset**, which contains demographic, job-related, and performance-related information about employees.

### Target Variable

- **Attrition**: Indicates whether an employee left the company  
  - Yes = 1  
  - No = 0  

---

## Technologies Used

The project was developed using the following technologies:

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  
- Git and GitHub  

---

## Repository Structure

```
people-analytics-employee-churn/
│
├── data/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── notebooks/
│   └── churn_analysis.ipynb
│
├── outputs/
│
├── src/
│
└── README.md
```

---

## How to Run the Project

### 1. Clone the repository

Open a terminal and run:

```bash
git clone https://github.com/denpareja/people-analytics-employee-churn.git
cd people-analytics-employee-churn
```

### 2. Install required dependencies

```bash
pip install -r requirements.txt
```

If you do not have a requirements file, you can manually install the main libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### 3. Open the notebook

```bash
jupyter notebook notebooks/churn_analysis.ipynb
```

---

## Modeling Approach

The project follows these main steps:

1. **Data Preprocessing**
   - Handling categorical variables  
   - Dropping non-informative features  
   - Standardizing numerical variables  

2. **Model Training**
   - Logistic Regression was used as the primary model  
   - Train-test split with stratification  
   - StandardScaler applied to features  

3. **Evaluation Metrics**
   - ROC-AUC  
   - Classification report  
   - Confusion matrix  

---

## Key Results

The Logistic Regression model achieved:

- **ROC-AUC Score:** approximately 0.80  
- Good performance identifying non-attrition cases  
- Moderate recall for employees who actually left  

These results indicate that the model can be useful as a first step in identifying potential churn risks within an organization.

---

## Future Improvements

Possible enhancements for future iterations:

- Testing additional models (Random Forest, XGBoost)  
- Hyperparameter tuning  
- Handling class imbalance with techniques like SMOTE  
- Building an interactive dashboard for HR teams  

---

## Author

**Denisse Pareja**

Data Scientist – TripleTen  
Miami, Florida  

---

## License

This project is for educational purposes.

