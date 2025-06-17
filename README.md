## **HR Employee Attrition Project: Use Case Analysis & Predictive Modeling**

This project focuses on analyzing employee attrition using an HR dataset and developing a predictive model to identify employees at risk of leaving the organization. The dataset includes various employee attributes such as job role, department, satisfaction levels, age, income, overtime status, and more.

## This project is divided into two parts.

## **Part One** : Explores HR attrition-related questions through data analysis.

## **Part Two** : Builds and compares machine learning models to predict employee attrition.
  The final Logistic Regression model was selected and saved for future use. Visualization was performed within Jupyter Notebook.


###**Project Files**

* `HR Employee analysis.ipynb` — Use case analysis and EDA (Part 1)
* `HR employee model.ipynb` — Feature engineering, SMOTE-enhanced modeling, model comparison (Part 2)
* `logistic_model.pkl` — Final Logistic Regression model
* `scaler.pkl` — Preprocessing scaler used for model inputs
* `Screenshot of the analysis.JPG` — Visual overview of the use case findings
* `README.md` — Project documentation



## **About the Dataset**

The dataset contains information about employees, including:

* Job Role
* Department
* Job Satisfaction
* Overtime
* Work-Life Balance
* Age, Salary, and other HR-relevant metrics

---

##  Project Objectives

###  Part One: Use Case Analysis

Key HR questions explored:

* **Which department has the highest attrition rate?**
* **Is there a strong relationship between job satisfaction and attrition?**
* **Does overtime or work-life balance correlate with attrition?**
* **Are certain roles, age groups, or salary bands more at risk of attrition?**

Tools:
Pandas, Seaborn, Matplotlib



### Part Two: Predictive Modeling

#### Goals

* Build a predictive model to identify employees at risk of attrition.
* Compare model performance using accuracy, recall, and precision.

#### 💡 Steps

1. **Data Preprocessing**

   * Encoding categorical features
   * Scaling numerical values
   * Addressing class imbalance using SMOTE
2. **Modeling**

   * Random Forest Classifier (SMOTE-enhanced)
   * Logistic Regression (balanced class weight)
3. **Model Evaluation**

   * Confusion Matrix
   * Accuracy Score
   * Classification Report
4. **Model Selection**

   * Final Model: Logistic Regression
   * Saved as `logistic_model.pkl`
   * Scaler saved as `scaler.pkl`



## Evaluation Summary

| Model                   | Accuracy         | Recall   | Precision |
| ----------------------- | ---------------- | -------- | --------- |
| Random Forest (SMOTE)   | Moderate         | Moderate | Moderate  |
| **Logistic Regression** | **Best Overall** | **High** | **High**  |

**Conclusion**:
Logistic Regression was chosen for its clarity, reliability, and balanced performance on key metrics.



## Getting Started

To run the project:

### Requirements

Install required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn joblib


### ▶Clone the Repository


git clone https://github.com/Ijeoma1179/HR-Employee-Attrition-Analysis.git
cd HR-Employee-Attrition-Analysis


### Load the Model

import joblib
model = joblib.load('logistic_model.pkl')
scaler = joblib.load('scaler.pkl')


### Insights for HR

* High attrition in specific departments and job roles
* Strong correlation between low job satisfaction, overtime, and attrition
* Younger employees with lower income more likely to leave



##  Visual Snapshot

A summary screenshot (`Screenshot of the analysis.JPG`) is included to provide a quick glance at key analytical insights.



## Author

Developed by **Nwadike Ijeoma Mary**,
A passionate **Data Scientist** dedicated to using analytics to solve real-world business problems.

Reach out: **[aijayij@gmail.com](mailto:aijayij@gmail.com)**





