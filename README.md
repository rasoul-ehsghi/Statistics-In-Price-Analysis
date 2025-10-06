# 📈 NVIDIA Stock Analysis  
### Quantifying the Impact of the COVID-19 Pandemic on NVDA Returns

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Statistical](https://img.shields.io/badge/Methodology-Statistical%20Testing-orange)

---

## 📖 Overview

This project answers a timely question with **data-driven clarity**:

> **Did the COVID-19 pandemic significantly alter NVIDIA’s (NVDA) stock return behavior?**

Instead of speculating, we use rigorous **hypothesis testing**, **visual analytics**, and **forecasting models** in Python to analyze the shift in return distributions before and during the pandemic. The result? A clear **statistical confirmation** that the pandemic caused a meaningful change in NVDA’s historical price dynamics.

---

## 🧪 Methodology at a Glance

The analysis is divided into **three scientific phases**:

---

### 🔬 Phase 1: Assumption Checking & EDA
Before testing hypotheses, we verified if the data satisfied parametric test assumptions.

- 🧠 **Shapiro-Wilk Test** – Assesses normality of daily returns  
- 📉 **Levene’s Test** – Checks for equality of return variances across time periods  
- 📊 **Q-Q Plot** – Visual confirmation of normal distribution

---

### 📈 Phase 2: Hypothesis Testing

Once assumptions were validated, we conducted the core statistical test:

- 🔎 **Welch’s t-test** — Robust against unequal variances and sample sizes  
  - **H₀ (Null Hypothesis):** μ_pre_covid = μ_covid  
  - **H₁ (Alternative Hypothesis):** μ_pre_covid ≠ μ_covid  
- ✅ **Confidence Level:** 95%  
- 📌 **Outcome:** *Null hypothesis rejected — the pandemic had a statistically significant effect*

---

### 📊 Phase 3: Visualization & Forecasting

- 🕹️ **Interactive Charts** — Candlestick, return series, rolling volatility  
- 🔮 **Prophet Forecasting** — Simple model to illustrate trends and short-term projections  
  *(Note: Forecasting is supplementary to the statistical analysis)*

---

## 🎯 Key Findings

> 📢 **COVID-19 caused a statistically significant shift in NVIDIA's return behavior.**

- Welch's t-test revealed a meaningful change in **mean daily returns**
- The change is both **statistically and economically** significant
- This method is **reproducible** for any asset or external market shock

---

## 📦 Tech Stack

| Category | Libraries |
|---------|-----------|
| **Language** | Python 3 |
| **Data Collection** | `yfinance` |
| **Manipulation** | `pandas`, `numpy` |
| **Statistical Testing** | `scipy.stats` |
| **Visualization** | `plotly`, `seaborn`, `matplotlib` |
| **Forecasting** | `prophet` |

---


## 📂 Project Structure

### 📥 Data Collection
- Fetch NVDA data using `yfinance`
- Period: **2019-01-01 to 2021-12-31**
- Data includes: **Open, High, Low, Close, Volume (OHLCV)**

### 🧹 Data Preprocessing
- Calculate daily **percentage returns**
- Clean **missing or null values**
- Split dataset into:
  - **Pre-pandemic (2019)**
  - **Pandemic (2020–2021)**
- Generate return series for analysis

### 📊 Exploratory Data Analysis
- Interactive **candlestick charts**
- Distribution plots & **histograms** of returns
- Rolling volatility (e.g., rolling standard deviation)
- **Normal Q-Q plots** for distribution checking
- Visual comparisons between time periods

### 🧪 Statistical Testing
- **Shapiro-Wilk test** (normality check)
- **Levene’s test** (variance homogeneity)
- **Welch’s t-test** (mean comparison between periods)
- Hypothesis testing at **95% confidence level**
- **P-value interpretation** for statistical significance

### 📈 Results & Interpretation
- Summary of **statistical test results**
- **Economic interpretation** of findings
- **Confidence interval** analysis
- **Effect size** and practical significance
- Final **conclusions** and **limitations**

### 🔮 Forecasting (Supplementary)
- Time series forecasting using **Prophet**
- **Trend and pattern** analysis
- Short-term **price projection**
- Evaluation of **forecast performance**

---
## 🔗 Related LinkedIn Post

📢 I shared insights and key takeaways from this project on LinkedIn.  
Check out the full post and join the discussion here:  
👉 [View the LinkedIn Post](https://www.linkedin.com/in/your-username/post-url)

