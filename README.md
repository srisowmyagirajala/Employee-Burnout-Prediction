# 🧑‍💼 Employee Burnout Prediction

## 📌 Overview
This project predicts the **burnout level of employees** using machine learning.  
It leverages workplace, demographic, and mental health factors to estimate an employee’s **Burn Rate**, enabling organizations to proactively address risks of burnout and improve employee well-being.

The workflow includes **data cleaning, exploratory data analysis (EDA), preprocessing, and predictive modeling**.  
A **Linear Regression model** was used as a baseline, with performance evaluated using error metrics.

---

## 📂 Dataset
The dataset contains employee details with the following features:

| Feature              | Description |
|----------------------|-------------|
| Employee ID          | Unique identifier (removed in preprocessing) |
| Gender               | Male / Female |
| Company Type         | Service / Product |
| WFH Setup Available  | Yes / No |
| Designation          | Job level / seniority |
| Resource Allocation  | Task allocation measure |
| Mental Fatigue Score | Numerical score of fatigue |
| Burn Rate            | Target variable (burnout level) |
| Date of Joining      | Employee joining date (removed after feature extraction) |

📎 **Dataset file:** `employee_burnout_analysis-AI (1).xlsx`

---

## 🔄 Data Preprocessing
- Handled missing values by removing null records.  
- Dropped irrelevant features: `Employee ID`, `Date of Joining`.  
- Converted `Date of Joining` into a derived numerical feature (**Days since 2008**) before removal.  
- Encoded categorical variables (`Gender`, `Company Type`, `WFH Setup Available`).  
- Standardized numerical features using **StandardScaler**.  

---

## 🤖 Models Used
- **Linear Regression** → Baseline regression model for burnout prediction.  

---

## 📊 Model Performance
| Metric | Value |
|--------|-------|
| **Mean Squared Error (MSE)** | Low error observed |
| **Mean Absolute Error (MAE)** | Stable performance |

📈 Visualizations of **Actual vs Predicted Burnout values** were plotted to evaluate accuracy.

---

## 🛠 Tech Stack
- **Python**
- **Pandas, NumPy** → Data handling  
- **Matplotlib, Seaborn** → Data visualization  
- **Scikit-learn** → Preprocessing, Modeling, Evaluation  

---

## 🚀 Future Improvements
- Implement advanced models (**Random Forest, XGBoost, Neural Networks**).  
- Perform **hyperparameter tuning** for improved accuracy.  
- Introduce new engineered features

---
