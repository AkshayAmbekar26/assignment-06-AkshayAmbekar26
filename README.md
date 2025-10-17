# Credit Default Prediction — Imputation via Regression

### 📘 Overview
This notebook implements **multiple imputation strategies** to handle missing data in the **UCI Credit Card Default dataset**, followed by a **classification analysis** using Logistic Regression.  
The goal is to compare imputation techniques—**Simple Median**, **Linear Regression**, **Non-linear Regression**, and **Listwise Deletion**—and evaluate their impact on downstream model performance.

---

### 🧩 Contents
1. **Data Loading & Cleaning** — Preprocessed demographic and financial variables; encoded categorical fields.  
2. **Missingness Simulation (MAR)** — Artificially introduced controlled missingness (≈6%) in key numeric columns (`AGE`, `BILL_AMT1`, `PAY_AMT1`).  
3. **Imputation Strategies**  
   - **Model A:** Median Imputation  
   - **Model B:** Linear Regression Imputation  
   - **Model C:** Non-linear (KNN/Decision Tree) Imputation  
   - **Model D:** Listwise Deletion  
4. **Model Evaluation** — Logistic Regression with standardization and cluster-based resampling; full performance metrics (Accuracy, ROC-AUC, Precision, Recall, F1).  
5. **Results Comparison & Discussion** — Quantitative tables, radar plots, F1 analysis, and conceptual discussion of trade-offs.

---

### 📊 Key Findings
- **Median Imputation (Model A)** achieved the most **balanced and generalizable performance**, with the best F1-score for the minority class (defaulters).  
- **Listwise Deletion (Model D)** showed slightly higher accuracy but suffered from information loss and bias.  
- **Linear Regression Imputation** marginally outperformed **Non-linear**, indicating predominantly **linear dependencies** between `BILL_AMT1` and other predictors.

---

### 🧠 Conclusion
For MAR-type missingness in structured financial data, **Median Imputation** provides the optimal trade-off between **simplicity**, **robustness**, and **predictive reliability**—making it the recommended approach for real-world credit scoring applications.

---

### ⚙️ Dependencies
- Python 3.10+  
- Libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`

---

**Author:** Akshay Ambekar (DA25S007)
**Institution:** IIT Madras — MS in Data Science & AI  
**Course:** DA5401 — Data Analytics Laboratory  
**Assignment:** A6 — *Imputation via Regression*
