**HR Employee Attrition Analysis & Prediction**
This project analyzes employee attrition in an organization using data-driven insights and builds predictive models to identify employees likely to leave. The final model aids HR teams in making informed decisions to improve employee retention.

**Project Structure**

HR-Employee-Attrition-Analysis/
 Part1_Use_Case_Analysis.ipynb     # Exploratory data analysis and insights

Part2_Model_Building.ipynb        # Model building and comparison

logistic_model.pkl                # Final saved logistic regression model

scaler.pkl                        # Scaler used in model preprocessing

analysis_screenshot.png           # Screenshot of key use case insights

README.md                         # Project documentation

**Part 1: Use Case Analysis**
The first notebook (Part1_Use_Case_Analysis.ipynb) explores the following key HR questions:

Which department has the highest attrition rate?

Is there a strong relationship between job satisfaction and attrition?

Does overtime or work-life balance correlate with attrition?

Are certain roles, age groups, or salary bands more at risk?

These questions were answered using data visualization and descriptive statistics to support HR decision-making.

**Part 2: Model Building**
The second notebook (Part2_Model_Building.ipynb) focuses on predictive modeling:

Model 1: Random Forest with SMOTE
A Random Forest classifier trained with SMOTE to address class imbalance.

Model 2: Logistic Regression (Final Model)
After comparison, Logistic Regression with class_weight='balanced' provided better interpretability and practical accuracy for HR use.

**Final Model Selection:**
Chosen Model: Logistic Regression

Reason: Balanced performance in accuracy, recall, and simplicity for deployment.

Saved Artifacts:

logistic_model.pkl – Trained logistic regression model

scaler.pkl – Scaler for preprocessing test data

**Tools & Libraries**
Python (Jupyter Notebook)

pandas, numpy, matplotlib, seaborn

scikit-learn (LogisticRegression, RandomForestClassifier, SMOTE)

joblib (for model serialization)

**Insights for HR Decision Making**
Job satisfaction and overtime are strong predictors of attrition.

Certain job roles and age groups showed higher risk.

Department-level analysis helps prioritize retention strategies.

**How to Use**
Clone the repository
git clone https://github.com/your-username/HR-Employee-Attrition-Analysis.git
cd HR-Employee-Attrition-Analysis
Open the Jupyter notebooks to view the analysis and model training.

**Load the model with:**

python
import joblib
model = joblib.load('logistic_model.pkl')
scaler = joblib.load('scaler.pkl')
**Screenshot Preview**
A screenshot showing part of the use case analysis is included for quick reference.

📧 Contact
For questions or collaboration, feel free to reach out via GitHub Issues or email.

