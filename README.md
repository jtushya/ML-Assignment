# ML Assignment 1 — BITS F464 Machine Learning

**Course:** BITS F464 | **Semester:** 1, 2025–26 | **Campus:** BITS Pilani, Hyderabad  
**Deadline:** March 1, 2026, 11:59 PM | **Demo:** Week of March 2, 2026

---

## Team Overview

| Person   | Module                     | % Done | Status         |
|----------|----------------------------|--------|----------------|
| Kartik   | Data & Utilities           | ~43%   | 🟡 Partial     |
| Gursidak | EDA                        | ~75%   | 🟡 Partial     |
| Tushya   | Linear Models              | ~30%   | 🔵 In Progress |
| Jayesh   | Advanced Models            | 0%     | 🔴 Not Started |

---

## Task 1 — Data Loading & Preprocessing *(Kartik)*

| Sub-task | Status |
|---|---|
| Load dataset; inspect shape & dtypes | ✅ Done |
| Identify missing values | ✅ Done |
| Define target variable (`Total_GHG_kgCO2e`) | ✅ Done |
| Explicit numerical vs categorical feature separation | ❌ Pending |
| Z-score normalisation (from scratch) | ⚠️ Done by Tushya — see note below |
| 80/20 train-test split (from scratch) | ⚠️ Done by Tushya — see note below |
| Shared metric helpers (`mae`, `mse`, `r2_score`) | ⚠️ Done by Tushya — see note below |

> **Note for Kartik:** The three items marked ⚠️ were implemented early by Tushya to unblock the linear models module (no sklearn — pure NumPy). Please wrap these into a reusable `get_data()` function so Jayesh's module can call it cleanly without copy-pasting.

---

## Task 2 — Exploratory Data Analysis *(Gursidak)*

| Sub-task | Status |
|---|---|
| Descriptive statistics (`df.describe()`) | ✅ Done |
| Histograms for all numerical features | ✅ Done |
| Boxplots + outlier analysis | ✅ Done |
| Correlation heatmap | ✅ Done |
| ≥3 insights in markdown | ✅ Done |
| Scatter plots — each feature vs `Total_GHG_kgCO2e` (Task 2c) | ❌ Missing |
| Bar chart of descriptive stats (min/max/mean/median/std) | ❌ Missing |

> **Note for Gursidak:** Two items are missing that the assignment explicitly requires. Add scatter plots (Task 2c) and the descriptive stats bar chart before final submission.

---

## Task 3 — Linear Regression *(Tushya)*

| Sub-task | Status |
|---|---|
| Feature selection + justification | ✅ Done |
| Z-score normalisation (from scratch) | ✅ Done |
| 80/20 train-test split (from scratch) | ✅ Done |
| Metric helpers: `mae()`, `mse()`, `r2_score()`, `denorm_y()` | ✅ Done |
| Batch Gradient Descent (BGD) — from scratch | ❌ Pending |
| SGD loss tracking per epoch | ❌ Pending |
| Stochastic Gradient Descent (SGD) — from scratch | ❌ Pending |
| BGD loss tracking per epoch | ❌ Pending |
| MAE / MSE / R² evaluation on test set (original scale) | ❌ Pending |
| BGD vs SGD — loss curve comparison plot | ❌ Pending |
| BGD vs SGD — metrics comparison table + discussion | ❌ Pending |

---

## Task 4 — Polynomial Regression + Regularisation *(Jayesh)*

| Sub-task | Status |
|---|---|
| Polynomial features degree 2 (from scratch) | ❌ Pending |
| L1 Lasso regularisation | ❌ Pending |
| L2 Ridge regularisation | ❌ Pending |
| Evaluation & comparison with linear regression | ❌ Pending |
| Visualisations | ❌ Pending |

> **Dependency for Jayesh:** You can directly reuse the normalisation, split, and metric helper cells Tushya added (cells 15–18 in the notebook). No need to wait for Kartik's `get_data()` refactor to start.

---

## Task 5 — Classification Reformulation *(Jayesh)*

| Sub-task | Status |
|---|---|
| Labelling strategy (low / medium / high emissions) — justified | ❌ Pending |
| Logistic Regression (from scratch) | ❌ Pending |
| Naive Bayes (from scratch) | ❌ Pending |
| Perceptron (from scratch) | ❌ Pending |
| Accuracy, Precision, Recall, F1, Confusion Matrix | ❌ Pending |
| Visualisations + strengths/limitations discussion | ❌ Pending |

---

## Notes

- **No external ML libraries.** All algorithms must be implemented from scratch. Only NumPy, Pandas, Matplotlib, and Seaborn are permitted.
- Submission filename: `TeamXX_Assignment1.ipynb`
- Run the entire notebook end-to-end before submitting — all outputs must be visible.
