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
| Jayesh   | Advanced Models            | 100%   | ✅ Complete     |

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
| Scatter plots — each feature vs `Total_GHG_kgCO2e` (Task 2c) | ✅ Done |
| Correlation heatmap | ✅ Done |
| ≥3 insights in markdown | ✅ Done |
| Bar chart of descriptive stats (min/max/mean/median/std) | ✅ Done |
| Additional plots wherever useful (Task 2e) | ✅ Done |



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
| Polynomial features degree 2 (from scratch) | ✅ Done |
| L1 Lasso regularisation | ✅ Done |
| L2 Ridge regularisation | ✅ Done |
| Evaluation & comparison with linear regression | ✅ Done |
| Summary of performance differences and model complexity effects (Task 4d) | ✅ Done |
| Visualisations | ✅ Done |

> **Note:** Jayesh's tasks build on the preprocessing and metric helpers from Tushya's Task 3 cells (`X_train`, `X_test`, `y_train`, `y_test`, `denorm_y()`, `mae()`, `mse()`, `r2_score()`).

---

## Task 5 — Classification Reformulation *(Jayesh)*

| Sub-task | Status |
|---|---|
| Labelling strategy (low / medium / high emissions) — justified | ✅ Done |
| Logistic Regression (from scratch) | ✅ Done |
| Naive Bayes (from scratch) | ✅ Done |
| Perceptron (from scratch) | ✅ Done |
| Accuracy, Precision, Recall, F1, Confusion Matrix | ✅ Done |
| Visualisations | ✅ Done |
| Discussion: suitability, limitations, information loss from discretisation | ✅ Done |

---

## Recent Fixes & Attributions by Tushya

The following fixes and additions were made by Tushya during the final audit and implementation pass to ensure the notebook runs end-to-end and aligns with the assignment requirements:

- **Data & Utilities (Kartik)**
  - I made data loading environment-agnostic so the notebook works on both Colab and local VS Code.
  - I renamed `get_data()` outputs to `*_full` to avoid variable name clashes with Task 3 preprocessing.

- **EDA (Gursidak)**
  - I removed a duplicate scatter-plot entry in the README.
  - I deleted an empty stray code cell between EDA and Task 3 that caused a visual gap.

- **Linear Models / Audit work (Tushya)**
  - I ensured metric helpers and normalization utilities are consistently defined and used across tasks.
  - I re-ran and validated Task 1–3 cells after installing missing packages (e.g., seaborn).

- **Advanced Models (Jayesh)**
  - I implemented Task 4 (Polynomial regression, L1/L2 regularisation) and Task 5 (classification reformulation) from scratch, and added evaluation, visualisations, and discussion.

All changes were committed to the repository after I verified that the notebook executes end-to-end and that outputs are visible.

---

## Notes

- **No external ML libraries.** All algorithms must be implemented from scratch. Only NumPy, Pandas, Matplotlib, and Seaborn are permitted.
- Submission filename: `TeamXX_Assignment1.ipynb`
- Team details header is already at the top of the notebook ✅
- Run the entire notebook end-to-end before submitting — all outputs must be visible.
- Cite any external references (textbooks, papers, docs) used.
