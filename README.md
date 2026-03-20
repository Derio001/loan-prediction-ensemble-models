# 🏦 Enhancing Loan Approval Accuracy through Ensemble-Based Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8+-blue)](https://www.python.org/)
[![Conference](https://img.shields.io/badge/Published-CSCT%202025%20%40%20NIT%20Sikkim-red)](https://scrs.in/conference/csct2025)
[![Publisher](https://img.shields.io/badge/Publisher-Springer-brightgreen)](https://www.springer.com/)
[![Models](https://img.shields.io/badge/Models-10%20Ensemble%20Algorithms-orange)](https://scikit-learn.org/)
[![Best Accuracy](https://img.shields.io/badge/Best%20Accuracy-LightGBM%2089%25-success)]()

> **Research paper presented at the 4th Congress on Smart Computing Technologies (CSCT 2025)**
> hosted by National Institute of Technology, Sikkim, India — December 13–14, 2025.
> Published under Springer.

*Authors: Mahamat Hanga Derio, Chaitra P C, Sujatha Arun Kokatnoor*
*Christ University, Bangalore, India*

---

## 📌 Research Objective

Loan approval decisions in financial institutions are often inconsistent, biased, or slow when
handled manually. This study systematically benchmarks **10 ensemble machine learning algorithms**
to identify the most accurate and reliable model for automated loan approval prediction —
with implications for microfinance institutions in data-scarce economies.

---

## 📊 Dataset

- **Source**: [Kaggle — Loan Status Prediction](https://www.kaggle.com/datasets/bhavikjikadara/loan-status-prediction)
- **Features**: Gender, Marital Status, Dependents, Education, Employment, Income,
  Co-applicant Income, Loan Amount, Loan Term, Credit History, Property Area
- **Target**: Loan Status (Approved / Rejected)
- **Preprocessing**: Mode imputation (categorical), median imputation (numerical),
  IQR-based outlier removal, Label Encoding

---

## 🤖 Models Benchmarked (10 Algorithms)

| Model | Accuracy |
|-------|----------|
| **LightGBM** | **89%** ✅ Best |
| Random Forest | 88% |
| CatBoost | 87% |
| XGBoost | 86% |
| Extra Trees | 86% |
| AdaBoost | 85% |
| Gradient Boosting | 84% |
| Bagging Classifier | 84% |
| Stacking Classifier | 82% |
| Voting Classifier | 79% |

**Key finding**: Gradient boosting variants (LightGBM, CatBoost, XGBoost) consistently
outperform bagging-based and meta-ensemble approaches on this tabular financial dataset.
LightGBM's leaf-wise tree growth gives it an edge in handling the income skew and
categorical feature interactions present in loan data.

---

## 🔬 Methodology
```
Raw Loan Dataset (Kaggle)
    ↓
Preprocessing — Imputation + Outlier Removal + Label Encoding
    ↓
Train/Test Split (80/20, random_state=42)
    ↓
Feature Importance Analysis (Random Forest)
    ↓
10 Ensemble Models Trained & Evaluated
    ↓
Accuracy + Confusion Matrix + Classification Report per model
    ↓
Final Comparison — Bar chart visualization
```

---

## 📌 Key Features Used

Credit History emerged as the strongest predictor of loan approval, followed by
Applicant Income and Loan Amount — consistent with lending theory and prior literature.

---

## 🚀 How to Run
```bash
# Clone
git clone https://github.com/Derio001/loan-prediction-ensemble-models.git
cd loan-prediction-ensemble-models

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost kagglehub

# Run notebook
jupyter notebook The_Project_Implementation.ipynb
```

> Dataset is auto-downloaded via `kagglehub` — no manual download needed.

---

## 🏛️ Conference & Publication

| Detail | Info |
|--------|------|
| Conference | 4th Congress on Smart Computing Technologies (CSCT 2025) |
| Venue | National Institute of Technology, Sikkim, India |
| Dates | December 13–14, 2025 |
| Paper ID | 872 |
| Publisher | Springer |
| Certificate | Presented by Mahamat Hanga Derio |

---

## 👤 Authors

**Mahamat Hanga Derio** — M.Tech Data Science, Christ University, Bangalore
**Chaitra P C** — Christ University, Bangalore
**Dr. Sujatha Arun Kokatnoor** — Department of AIML & DS, Christ University, Bangalore

🔗 [GitHub](https://github.com/Derio001) | [LRI Health Project](https://github.com/Derio001/lri-prediction-chad) | [GDP Intelligence Project](https://github.com/Derio001/exploratory-predictive-gdp-analysis)

---

*Part of ongoing research in applied machine learning for financial and development contexts.*
