# MASI-Boy: Credit Risk Modeling & Data Imputation Assignment

## 🧠 Overview
This project notebook (`masi-boy.ipynb`) demonstrates a complete workflow for **data preprocessing, missing value imputation, and credit risk modeling** using the **UCI Credit Card Default dataset**.  
It was designed as part of an academic assignment to test understanding of **data wrangling**, **statistical imputation**, and **predictive modeling**.

---

## 📂 Dataset
**Source:** [UCI Default of Credit Card Clients Dataset (Kaggle)](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)  
**File used:** `UCI_Credit_Card.csv`

The dataset contains demographic and financial information for over 30,000 credit card clients in Taiwan, including repayment history and default status.

---

## 🧰 Environment Setup
Make sure the following Python libraries are installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels missingno
```

---

## 🪜 Notebook Structure

### **Part A: Data Preprocessing and Imputation [20 points]**
- Handling missing values and exploring missingness patterns  
- Simulating **MAR (Missing At Random)** mechanism  
- Comparing data **distribution before and after missingness**  
- Implementing and evaluating multiple imputation strategies:
  1. **Simple Imputation (Mean / Median)**
  2. **Linear Regression Imputation**
  3. **Non-Linear Regression Imputation (e.g., Random Forest, KNN, etc.)**

### **Part B (if applicable): Modeling and Evaluation**
- Training baseline models for credit default prediction  
- Performing feature selection and scaling  
- Evaluating model performance (Accuracy, ROC-AUC, Precision, Recall)  
- Visual diagnostics and interpretability checks  

---

## 📊 Visualizations
- Distribution comparisons before and after imputation  
- Missingness heatmaps (using `missingno`)  
- Regression residual analysis for imputation diagnostics  
- Feature importance and prediction metrics (if modeling is included)

---

## ✅ Key Insights
- Demonstrates that **regression-based imputation** maintains feature relationships better than simple statistical methods.  
- Highlights the **impact of imputation strategy** on downstream predictive modeling.  
- Offers reproducible visual comparisons to assess imputation bias.

---

## 💡 Extensions
To go beyond the assignment, you can:
- Integrate **multiple imputation by chained equations (MICE)**  
- Add **automated hyperparameter tuning**  
- Compare **tree-based vs. linear imputations**  
- Incorporate **SHAP / LIME explainability** for model interpretability  

---

## 🧾 License
This project is intended for educational use under IIT Madras’ MS (DS & AI) coursework.  
All dataset rights belong to the original UCI/Kaggle data providers.

---

## 👤 Author
**Akshay [MS DS & AI @ IIT Madras]**  
Focus: Practical, reproducible, and explainable data science pipelines.
