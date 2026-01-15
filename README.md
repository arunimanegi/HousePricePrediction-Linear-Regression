# Housing Price Prediction using Linear Regression

A clean end-to-end Machine Learning project to predict house prices using **Linear Regression**.  
This project demonstrates a complete supervised ML workflow including **data preprocessing, scaling, model training, evaluation, and interpretation** (feature importance).

---

## Problem Statement
Given housing-related features such as crime rate, number of rooms, tax rate, etc., the goal is to build a regression model that predicts the **median value of owner-occupied homes** (target variable).

---

## Dataset
The project uses a housing dataset (Boston housing-style schema) with numerical features.

**Target:** `MEDV` / `Price` (median house value)

**Typical features include:**
- `CRIM` — per capita crime rate
- `RM` — average number of rooms
- `TAX` — property tax rate
- `LSTAT` — % lower status population
- etc.

> Note: The official `load_boston()` dataset is deprecated in scikit-learn. This project uses a CSV-based version or OpenML equivalent.

---

## Workflow
1. **Load dataset**
2. **Train-test split**
3. **Feature scaling**
   - `StandardScaler` is fit on training data only
   - test data is transformed using the same scaler (avoids data leakage)
4. **Model training**
   - `LinearRegression()` from scikit-learn
5. **Evaluation**
   - Mean Squared Error (MSE)
   - R² Score
6. **Interpretation**
   - Model coefficients (feature importance)
7. **Visualization**
   - Actual vs Predicted plot
   - Feature importance bar chart

---

## Tech Stack
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Installation
Clone the repository and install dependencies:

```bash
git clone <repo-url>
cd <repo-folder>
pip install -r requirements.txt
