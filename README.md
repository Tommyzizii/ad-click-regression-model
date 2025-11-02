# 🧠 Ad Click Regression Model

A mini machine learning project applying **Linear Regression** to analyze the relationship between ad impressions, spending, and click performance.  
This project demonstrates how data transformation and regression modeling can be used to evaluate and predict ad conversion efficiency.

---

## 📘 Overview

This mini-project explores how the number of ad impressions and amount spent affect ad clicks.  
Using **Python**, **Pandas**, **Seaborn**, and **Statsmodels**, the notebook visualizes relationships, applies transformations, and fits a linear regression model to predict ad performance.

---

## 📂 Dataset

**File:** `ad_conversion.csv`  

| Column | Description |
|---------|--------------|
| `spent_usd` | Amount of money spent on ads (USD) |
| `n_impressions` | Number of ad impressions displayed |
| `n_clicks` | Number of ad clicks received |

---

## 🧩 Methodology

1. **Data Import & Visualization**  
   - Plotted scatter and regression plots of impressions vs clicks.  
   - Observed non-linear relationship between features.

2. **Feature Transformation**  
   - Applied quartic-root transformation (`x^0.25`) to stabilize variance and linearize the relationship.

3. **Model Building**  
   - Built an Ordinary Least Squares (OLS) regression model using:
     \[
     \text{qdrt\_n\_clicks} = 0.0717 + 0.1115 \times \text{qdrt\_n\_impressions}
     \]

4. **Prediction & Evaluation**  
   - Generated prediction data for impressions up to 3,000,000.  
   - Calculated key metrics:
     - **Mean Squared Error (MSE):** 0.0387  
     - **Residual Standard Error (RSE):** 0.197  
   - MSE value close to zero indicates a good model fit.

---

## 📈 Visualizations

| Visualization | Description |
|----------------|-------------|
| Scatter Plot | Shows the relationship between ad impressions and clicks |
| Regression Plot | Displays best-fit line before and after transformation |
| Prediction Overlay | Compares actual vs predicted values using red markers |

---

## 🧮 Tools & Libraries

| Library | Purpose |
|----------|----------|
| **NumPy** | Mathematical computation |
| **Pandas** | Data manipulation |
| **Matplotlib / Seaborn** | Data visualization |
| **Statsmodels** | Statistical modeling (OLS regression) |

---
