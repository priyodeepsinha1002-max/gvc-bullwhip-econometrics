# Analysing US Demand Shocks and Industrial Production in Export-Oriented Asian Economies

An advanced econometric and predictive analytics project evaluating the propagation of downstream macroeconomic demand shocks through international supply chains to impact Asian industrial production.

## 📊 Project Overview
This project integrates data engineering, predictive modeling, and macroeconomic theory to evaluate the structural dependencies within Global Value Chains (GVCs). By cleaning, merging, and analyzing five distinct integrated datasets, the model explores how external demand shocks originating in the United States affect industrial production across key export-oriented Asian economies, and evaluates whether a nation's trade dependency acts as a regional amplifier for volatility.

---

## 🛠️ Technical Workflow & Methodology

The analysis follows a rigorous, end-to-end data science and econometric pipeline:

### 1. Data Engineering & Integration
- Extracted, engineered, and integrated features across **5 distinct macroeconomic datasets** using `pandas` and `NumPy`.
- Handled missing values, aligned time-series frequencies, and executed data normalization (log transformations) to prepare variables for stable regression modeling.

### 2. Hypothesis Testing & Diagnostics
- Performed comparative hypothesis testing using independent and paired t-tests (`scipy.stats`) to check statistical differences across economic eras.
- Executed strict quality checks using the **Shapiro-Wilk test** to analyze distribution normality and curve characteristics.

### 3. Advanced Econometric Modeling
- Constructed Ordinary Least Squares (OLS) regression frameworks using `statsmodels` to map the elasticity of production.
- Implemented **Clustered Robust Standard Errors** (`cov_type='cluster'`) to control for intra-country correlation and panel data complexities, guaranteeing highly reliable statistical inference.
- Evaluated **High Condition Numbers** to systematically diagnose and mitigate potential multicollinearity issues among GVC indicators.

---

## 📈 Key Insights & Results

- **High Joint Significance:** The model achieved a robust and highly significant **F-statistic**, successfully validating the joint predictive power of the independent variables and rejecting the null hypothesis ($H_0$).
- **The Bullwhip Effect Quantified:** The empirical analysis revealed a highly elastic **10.98 US Import coefficient**. Grounded in supply chain literature (*Lee et al., 1997*), this mathematically validates how deep integration into global value chains subjects downstream manufacturers to amplified, highly volatile demand shocks.
- **The GVC Paradox:** Advanced reflections show that while deep GVC participation accelerates manufacturing growth during global expansions, it simultaneously acts as a structural transmission channel for severe systemic vulnerability during global demand contractions.

---

## 🚀 Technologies Used

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Statistical Modeling:** `statsmodels` (OLS, Robust Covariance Estimators)
- **Scientific Computing:** `scipy.stats` (T-tests, Shapiro-Wilk)
- **Data Visualization:** `matplotlib`, `seaborn`

---
