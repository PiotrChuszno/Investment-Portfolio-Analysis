# Investment Portfolio Analysis & Scoring Models

## 📌 Overview
This repository collects my personal tools and models used for investment analysis. The project combines three key pillars: **Quantitative Scoring**, **Fundamental Valuation**, and **Risk Management**.

My goal is to identify high-quality, undervalued companies using a structured checklist and then optimize how they fit into a portfolio.

## 📈 Performance (Backtest)
I backtested the scoring strategy to see how it performs over the long term.
* **Period:** 01.06.2006 – 01.12.2025
* **CAGR:** **22.07%**
* **Strategy:** Long-only equity selection based on the scoring model described below.
* *📂 Go to folder `1_Scrab_Strategy_Backtest` for detailed equity curves and drawdown metrics.*

## 🛠 Tools & Methodology

My workflow integrates external data platforms (Scrab, Portfolio Visualizer) with custom logic built in Excel.

### 1. Scoring Model (20 Criteria)
I designed a custom scoring system based on 20 fundamental indicators to filter stocks. It focuses heavily on cash flow generation and financial safety.
* **Valuation & Growth:** I analyze **Price-to-FCF** and look for growth trends (e.g., is growth accelerating or slowing down?).
* **Safety & Risk:** Strict screening using **Free Cash Flow to Debt** ratios and the **Ohlson O-score** to filter out companies with high bankruptcy risk.

### 2. Intrinsic Value Calculation (DCF & Relative Model)
Selected candidates undergo a deep-dive valuation. I built a dynamic **Excel model** that bridges two approaches:
* **DCF (Discounted Cash Flow):** Calculates value based on projected Free Cash Flow.
* **Target P/E:** Adjusts valuation based on market sentiment and business quality.
* **Blended Value:** The final output is a weighted average of both methods.
* *📂 Go to folder `2_Valuation_Models_Excel` to see the model and case study (Expand Energy Corp).*

### 3. Risk Management & Asset Allocation
Instead of simple equal weighting, I use a risk-parity approach to manage volatility.
* **Correlation Data:** I extract correlation matrices and standard deviation metrics using **Portfolio Visualizer**.
* **Optimization:** I feed this data into a custom spreadsheet that calculates the optimal weight for each position to minimize the overall portfolio risk.
* *📂 Go to folder `3_Risk_Correlation_Analysis` for correlation matrices and allocation logic.*

---
**Author:** Piotr Chuszno
*Data Analyst | Financial Modeling Enthusiast*
*Check out my LinkedIn profile for more details.*
