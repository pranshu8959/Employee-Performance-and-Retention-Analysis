# 🧠 Employee Performance and Retention Analysis

This project aims to analyze employee performance and attrition trends using a blend of **statistical analysis**, **machine learning**, and **deep learning** techniques. It follows a real-world HR analytics use case and is structured into four comprehensive phases.

---

## 📌 Objective

- Understand key drivers of employee performance.
- Predict employee attrition (who is likely to leave).
- Recommend data-driven HR strategies to improve retention and engagement.

---

## 📂 Dataset Description

The dataset includes 100 employees with the following features:
- **Demographics**: Age, Department
- **Financials**: Salary
- **Tenure**: Years at Company
- **Performance**: Performance Score
- **Attrition Status**: Yes / No

---

## 🔍 Project Workflow

### ✅ Phase 1: Exploratory Data Analysis (EDA) & Statistics
- Cleaned missing values and duplicates.
- Standardized department names.
- Visualized feature relationships using:
  - Pairplots
  - Correlation heatmaps
  - Boxplots for outlier detection
- Statistical insights:
  - **Bayes’ Theorem** was used to estimate attrition likelihood given low performance.
  - **ANOVA test** showed whether performance varies by department.

### ✅ Phase 2: Predictive Modeling
- **Feature Encoding**: Label Encoding & Min-Max Scaling.
- **Attrition Classifier**: Built using **Random Forest**, evaluated on Accuracy, F1-Score, Confusion Matrix.
- **Performance Regressor**: Used **Linear Regression**, evaluated using **R²** and **MSE**.

### ✅ Phase 3: Deep Learning Models
- **Performance Prediction**: Feedforward Neural Network trained on scaled features.
- **Attrition Classification**: Binary neural network using sigmoid output for classification.

### ✅ Phase 4: Reporting & Insights
- Identified **high-attrition departments**.
- Visualized:
  - Attrition by department (bar chart)
  - Salary vs performance (scatter plot, color-coded by attrition)
- Summarized insights and action points.

---

## 🧾 Final Report – Findings & Conclusions

### 📌 Key Findings:
- Employees with **low performance scores** are significantly more likely to leave.
- Departments like **Sales and Marketing** have **higher attrition rates**.
- There is **positive correlation between salary and performance**, but not strong enough to guarantee retention.
- **Years at company** and **age** show moderate impact on attrition.

### 💡 Business Recommendations:
- **Targeted performance improvement programs** for underperformers.
- **Department-specific retention strategies** for Sales and Marketing.
- **Incentive alignment** with performance to reduce attrition.
- Use **predictive models periodically** to flag high-risk employees early.

---

## 🧰 Tools & Libraries Used

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow/Keras
- Scipy (for statistical testing)

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**.
2. Upload your CSV using:
   ```python
   from google.colab import files
   uploaded = files.upload()


