# ML Assignment 1 — BITS F464 Machine Learning

**Course:** BITS F464 | **Semester:** 1, 2025–26 | **Campus:** BITS Pilani, Hyderabad  
**Deadline:** March 1, 2026, 11:59 PM | **Demo:** Week of March 2, 2026

---

## Team Overview

| Person   | Module                     | % Done | Status         |
|----------|----------------------------|--------|----------------|
| Kartik   | Data & Utilities           | 100%   | ✅ Complete     |
| Gursidak | EDA                        | 100%   | ✅ Complete     |
| Tushya   | Linear Models              | 100%   | ✅ Complete    |
| Jayesh   | Advanced Models            | 0%     | 🔴 Not Started |

---

## Task 1 — Data Loading & Preprocessing *(Kartik)*

| Sub-task | Status |
|---|---|
| Load dataset; inspect shape & dtypes | ✅ Done |
| Identify missing values | ✅ Done |
| Define target variable (`Total_GHG_kgCO2e`) | ✅ Done |
| Identify numerical and categorical features | ✅ Done |
| Justify selection of numerical input features | ✅ Done |
| Z-score normalisation (from scratch) | ✅ Done |
| 80/20 train-test split (from scratch) | ✅ Done |
| Shared metric helpers (`mae`, `mse`, `r2_score`) | ✅ Done |


---

## Task 2 — Exploratory Data Analysis *(Gursidak)*

| Sub-task | Status |
|---|---|
| Descriptive statistics (`df.describe()`) | ✅ Done |
| Histograms for all numerical features | ✅ Done |
| Boxplots + outlier analysis | ✅ Done |
| Scatter plots — each feature vs `Total_GHG_kgCO2e` (Task 2c) | ❌ Pending |
| Correlation heatmap | ✅ Done |
| ≥3 insights in markdown | ✅ Done |
| Scatter plots — each feature vs `Total_GHG_kgCO2e` (Task 2c) | ✅ Done |
| Bar chart of descriptive stats (min/max/mean/median/std) | ✅ Done |



---

## Task 3 — Linear Regression *(Tushya)* ✅

| Sub-task | Status |
|---|---|
| Feature selection + justification | ✅ Done |
| Z-score normalisation (from scratch) | ✅ Done |
| 80/20 train-test split (from scratch) | ✅ Done |
| Metric helpers: `mae()`, `mse()`, `r2_score()`, `denorm_y()` | ✅ Done |
| Batch Gradient Descent (BGD) — from scratch | ✅ Done |
| BGD loss tracking per epoch | ✅ Done |
| Stochastic Gradient Descent (SGD) — from scratch | ✅ Done |
| SGD loss tracking per epoch | ✅ Done |
| MAE / MSE / R² evaluation on test set (original scale) | ✅ Done |
| BGD vs SGD — loss curve comparison plot | ✅ Done |
| BGD vs SGD — metrics comparison table + discussion | ✅ Done |

---

## Task 4 — Polynomial Regression + Regularisation *(Jayesh)*

| Sub-task | Status |
|---|---|
| Polynomial features degree 2 (from scratch) | ❌ Pending |
| L1 Lasso regularisation | ❌ Pending |
| L2 Ridge regularisation | ❌ Pending |
| Evaluation & comparison with linear regression | ❌ Pending |
| Summary of performance differences and model complexity effects (Task 4d) | ❌ Pending |
| Visualisations | ❌ Pending |

> **Dependency for Jayesh:** You can directly reuse the normalisation, split, and metric helper cells Tushya added (cells 16–19 in the notebook). No need to wait for Kartik's `get_data()` refactor to start. The variables `X_train`, `X_test`, `y_train`, `y_test`, `y_mean`, `y_std`, `denorm_y()`, `mae()`, `mse()`, `r2_score()` are all available once those cells are run.

---

## Task 5 — Classification Reformulation *(Jayesh)*

| Sub-task | Status |
|---|---|
| Labelling strategy (low / medium / high emissions) — justified | ❌ Pending |
| Logistic Regression (from scratch) | ❌ Pending |
| Naive Bayes (from scratch) | ❌ Pending |
| Perceptron (from scratch) | ❌ Pending |
| Accuracy, Precision, Recall, F1, Confusion Matrix | ❌ Pending |
| Visualisations | ❌ Pending |
| Discussion: suitability, limitations, information loss from discretisation | ❌ Pending |

---

## Notes

- **No external ML libraries.** All algorithms must be implemented from scratch. Only NumPy, Pandas, Matplotlib, and Seaborn are permitted.
- Submission filename: `TeamXX_Assignment1.ipynb`
- Team details header is already at the top of the notebook ✅
- Run the entire notebook end-to-end before submitting — all outputs must be visible.
- Cite any external references (textbooks, papers, docs) used.
