# 🔍 ML: Classification and Regression

This project demonstrates a complete machine-learning workflow for **exploratory data analysis (EDA)** and **predictive modeling** using classical regression methods. The goal is to understand how linear models behave on structured data, identify feature relationships, and apply regularization techniques to improve model stability and generalization.

The project is divided into **three main parts**, each building upon the previous one:

- **Part 1:** Exploratory Data Analysis (EDA)
- **Part 2:** Linear Regression (OLS)
- **Part 3:** Ridge Regression (L2 Regularization) & Model Comparison

---

## 📊 Dataset Overview

This project uses the **Diamonds Dataset**, a structured dataset with **53,940 samples** and **10 features** describing diamond characteristics and market prices.

### 🔹 Dataset Name
**Diamonds Dataset (53,940 rows × 10 features)**

### 🔹 Numerical Features
These continuous variables describe physical measurements:

- **carat** — diamond weight  
- **depth** — total depth percentage  
- **table** — width of the top surface  
- **price** — price in USD  
- **x** — length (mm)  
- **y** — width (mm)  
- **z** — depth (mm)

### 🔹 Categorical Features

- **cut** — quality of the cut *(Fair, Good, Very Good, Premium, Ideal)*  
- **color** — color grade *(J = worst, D = best)*  
- **clarity** — clarity grade *(I1, SI2, SI1, VS2, VS1, VVS2, VVS1, IF)*  

### 🔹 Initial Data Profiling Includes:
- Data types and missing-value inspection  
- Summary statistics using `.describe()`  
- Outlier and skewness detection  
- Category distribution analysis  
- Identification of correlated and redundant features  

This dataset is ideal for regression studies due to strong relationships between physical measurements and price.

---

# 🧩 Part-by-Part Breakdown

## 📘 **Part 1 — Exploratory Data Analysis (EDA)**

This section focuses on understanding the structure and patterns within the dataset. It includes:

- Distribution plots (histograms, KDE)  
- Boxplots & violin plots for categorical-numerical relationships  
- Pairwise scatter plots  
- Correlation heatmap to reveal multicollinearity  
- Analysis of how cut, color, and clarity influence price  
- Identification of skewness, outliers, and feature scaling needs  

This exploratory phase guides the modeling strategy used in later parts.

---

## 📘 **Part 2 — Linear Regression (OLS-Based)**

Part 2 implements **Ordinary Least Squares (OLS)** as the baseline regression model.

Key components include:

- One-hot encoding of categorical variables  
- Train-test splitting  
- Fitting the OLS model  
- Evaluating performance with:  
  - **MSE (Mean Squared Error)**  
  - **RMSE**  
  - **R² Score**  
- Scatter plot of predictions vs. actual price  
- Analysis of residuals and model limitations  

**Insights:**

- OLS is easy to interpret and fast to compute  
- Multicollinearity among physical measurements affects stability  
- Model sensitivity to outliers is visible in residual patterns  

---

## 📘 **Part 3 — Ridge Regression (L2 Regularization) & Model Comparison**

Part 3 introduces **Ridge Regression**, which adds an L2 penalty to shrink coefficients and reduce variance.

This section includes:

- Applying Ridge Regression across different regularization strengths (λ)  
- Comparing Ridge performance with OLS on the test set  
- Visualization of coefficient shrinkage  
- Evaluating model generalization and stability  
- Bias–variance tradeoff discussion  
- Demonstrating how regularization handles multicollinearity  

**Key Takeaways:**

- Ridge reduces overfitting  
- Produces more stable coefficients  
- Handles correlated features better  
- Often improves prediction quality compared to plain OLS  

---
'''
## 📂 Project Structure

project/
├── Part1.ipynb # Exploratory Data Analysis (EDA)
├── Part2.ipynb # Linear Regression Modeling
├── Part3.ipynb # Ridge Regression & Model Comparison
├── dataset.csv # Dataset for analysis 
└── README.md # Project documentation

''''

---

## 🧰 Tools & Frameworks

- **Python 3.x**  
- **NumPy**  
- **Pandas**  
- **Matplotlib**  
- **Seaborn**  
- **scikit-learn**  

---



