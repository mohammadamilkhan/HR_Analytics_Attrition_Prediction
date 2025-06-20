#  Project Report: HR Analytics Prediction

## 1. Objective
The primary goal of this project is to analyze employee data to understand factors that influence **employee attrition** — the departure of employees from an organization. The analysis aims to:
- Uncover hidden patterns and correlations in HR data.
- Build predictive models to forecast which employees are likely to leave.

## 2. Dataset Overview
- The dataset `HR-Employee-Attrition.csv` contains various features such as age, department, distance from home, job satisfaction, monthly income, performance rating, etc.
- The target variable is **Attrition**, indicating whether an employee left the company.

## 3. Exploratory Data Analysis (EDA)
EDA was performed on both **categorical** and **numerical** features:

### Categorical Analysis (via count plots):
- Departments like **Sales** and **R&D** showed higher attrition.
- Job roles like **Sales Executive** and **Lab Technician** had high attrition.
- Employees who **work overtime** or have **low job involvement** show higher attrition.

### Numerical Analysis (via histograms):
- **Younger employees** (25–35 years) are more likely to leave.
- **Lower monthly income** and **less working experience** are strong indicators of attrition.

## 4. Data Preprocessing
- Encoding categorical variables using mapping and one-hot encoding.
- Dropping columns with no variance or relevance (`EmployeeCount`, `StandardHours`, etc.).
- Handling imbalanced dataset using **SMOTE** oversampling technique.

## 5. Model Building
Two classification models were implemented:
- **Decision Tree Classifier**
  - Simple, interpretable, and provides moderate performance.
- **Random Forest Classifier**
  - Higher accuracy and robustness due to ensemble learning.

## 6. Evaluation Metrics
Used metrics:
- **Accuracy**, **Precision**, **Recall**, **F1-Score**
- **Confusion Matrix** visualization for both models

 **Random Forest** outperformed **Decision Tree** in both training and testing accuracy.

---

#  Conclusion
The analysis effectively highlights critical factors impacting employee attrition. Key insights include:
- Employees with **low income**, **less experience**, and **low job satisfaction** are more likely to leave.
- **Overtime work** and **lack of growth opportunities** also correlate with higher attrition.
- Predictive modeling using **Random Forest** gave satisfactory results in predicting attrition trends.

---

#  Recommendations
- Improve employee engagement by addressing concerns in job roles with high attrition.
- Provide career growth opportunities to reduce attrition among younger and low-level employees.
- Enhance compensation for low-income employees to improve retention.
- Regularly monitor job satisfaction and work-life balance.

---

#  Future Work
- Deploy the model in an HR dashboard to flag high-risk attrition cases in real time.
- Integrate real-time employee feedback data to improve prediction.
- Explore deep learning models or **XGBoost** for improved performance.
- Conduct **survival analysis** to estimate the time before an employee leaves.
