# Investment Portfolio Analysis & Scoring Models

## 📌 Project Overview
This repository documents a proprietary investment strategy combining **Quantitative Scoring**, **Fundamental Analysis**, and **Risk Management**.

The objective is to identify high-quality, undervalued companies using a rigorous 20-point checklist and optimize portfolio allocation to maximize risk-adjusted returns.

## 📈 Performance (Backtest)
* **Period:** 01.06.2006 – 01.12.2025
* **CAGR:** **21.77%**
* **Strategy:** Long-only equity selection based on the proprietary scoring model detailed below.
* *📂 See folder `1_Scrab_Strategy_Backtest` for detailed equity curves and drawdown metrics.*

## 🛠 Tools & Methodology

My workflow integrates specialized data platforms (Scrab, Portfolio Visualizer) with custom modeling logic in Google Sheets/Excel.

### 1. Proprietary Scoring Model (20 Criteria)
I designed a custom scoring algorithm based on 20 fundamental indicators to filter stocks. The model emphasizes cash flow generation and financial safety.
* **Valuation & Growth:** Analysis of **Price-to-FCF** and expected growth rates in Operating Cash Flow, Net Income, and Revenue.
* **Trend Analysis:** Comparative analysis of Projected Growth vs. Historical Growth (acceleration/deceleration detection).
* **Safety & Bankruptcy Risk:** Strict screening using **Free Cash Flow to Debt** ratios and the **Ohlson O-score** (Default Probability) to filter out distressed assets.

### 2. Intrinsic Value Calculation (DCF Model)
Selected candidates undergo a deep-dive valuation using a custom **Discounted Cash Flow (DCF)** model built in Google Sheets.
* **Quantitative Inputs:** Calculation of Projected Free Cash Flow and **WACC** (incorporating Total Debt and Cash & Equivalents).
* **Forecasts:** Modeling future **EPS** trajectories and earnings growth rates.
* **Qualitative Adjustments:** Manual assessment of business moat, margin stability, and sector outlook ("Future-proof" analysis).
* *📂 See folder `2_Valuation_Models_Excel` for the valuation template.*

### 3. Risk Management & Asset Allocation
I utilize a hybrid workflow to optimize portfolio weights, moving away from equal-weighted allocation to a risk-parity approach.
* **Correlation Data:** Extraction of Asset Correlations and Standard Deviation metrics using **Portfolio Visualizer**.
* **Optimization Algorithm:** Data is fed into a custom spreadsheet model that calculates the optimal weight for each position to minimize portfolio volatility based on the input covariance matrix.
* *📂 See folder `3_Risk_Correlation_Analysis` for correlation matrices and allocation logic.*

---
**Author:** Piotr Chuszno
*Junior Data Analyst | Financial Modeling Enthusiast*
*Check out my LinkedIn profile for more details.*
