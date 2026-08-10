# Hi, I'm Saba Aslani 👋

**Data Analyst & Data Engineer** | Python · SQL · dbt · Power BI · Machine Learning  
📍 Vancouver, BC &nbsp;·&nbsp; 🌐 [Portfolio](https://saba-aslani.github.io) &nbsp;·&nbsp; 🔗 [LinkedIn](https://linkedin.com/in/saba-aslani) &nbsp;·&nbsp; 📧 aslanisaba2@gmail.com

---

Messy data in. Clear decisions out.

5+ years across operations, manufacturing, and retail — with an electrical engineering foundation that shows up in how I read signal from noise.

---

## 🛠 Tech Stack

**Languages & Analytics**  
`Python` `SQL` `pandas` `NumPy` `Scikit-learn` `XGBoost` `SHAP` `SciPy` `statsmodels`

**Data Engineering**  
`dbt` `PostgreSQL` `SQLite` `Neon` `ETL/ELT Pipelines` `GitHub Actions` `Docker` `Incremental Models` `SCD Type 2`

**BI & Visualization**  
`Power BI` `DAX` `Power Query` `Tableau` `Streamlit` `Plotly` `Matplotlib` `Seaborn`

**Statistics & ML**  
`A/B Testing` `Hypothesis Testing` `Power Analysis` `EDA` `RFM Segmentation` `Predictive Modeling`

**Tools**  
`Git` `GitHub` `Jupyter Notebook` `VS Code` `Docker` `Excel`

---

## 🚀 Featured Projects

### 🚢 [Canada Trade Gateway — Live DE Pipeline](https://github.com/saba-aslani/canada-trade-gateway)
> Real-time analytics pipeline on Pacific port & land border congestion | Every 15 minutes | Live dashboard

- Ingests live AIS vessel positions (WebSocket) and CBSA border delay data (CSV) every 15 minutes via **GitHub Actions cron**
- Stores raw data in **Neon Postgres** (region-matched to BC); transforms with **dbt** incremental models, 28 data tests
- Surfaces congestion signals: vessel holding-position share across Vancouver and Prince Rupert port approaches; commercial lane delays across 29 CBSA crossings
- Key engineering decisions: read-only dashboard role (security), 240-second AIS window to correct for transmission bias, `status_speed_conflict` flag to measure AIS data quality, external scheduler to keep 15-min cadence reliable on free infrastructure
- 📊 **[Live Dashboard →](https://canada-trade-gateway-dashboard.streamlit.app/)**

**Stack:** `Python` `dbt` `PostgreSQL` `Neon` `GitHub Actions` `Streamlit` `AIS WebSocket`

---

### 🛍 [Brazilian E-Commerce Analytics — dbt + PostgreSQL](https://github.com/saba-aslani/ecommerce-analytics-dbt)
> Modern ELT pipeline on ~1.5M rows | Star schema | CI/CD | Power BI

- Transformed ~1.5M rows of Olist e-commerce data through 3-layer dbt pipeline: raw → staging (8 models) → dimensional marts (`dim_customers`, `dim_products`, `fct_orders`)
- Star schema with fan-out prevention (pre-aggregated CTEs before joins); `fct_orders` materialized **incrementally**
- **SCD Type 2 snapshot** on `order_status` to preserve status-change history
- Automated data-quality tests: `unique`, `not_null`, `relationships`, `accepted_values` on all keys and critical columns
- **CI/CD**: GitHub Actions spins up ephemeral PostgreSQL service and validates full dbt build on every push
- Key findings: 97% fulfillment rate, avg order value ~161 BRL across 99,441 orders, SP dominates revenue
- Power BI dashboard connected directly to marts layer

**Stack:** `dbt` `PostgreSQL 16` `Power BI` `Docker` `GitHub Actions` `SQL`

---

### 📉 [Quantitative Backtesting Framework](https://github.com/saba-aslani/quant-backtesting-framework)
> Research-grade backtesting engine for FX & crypto | Walk-forward validation | AI agent layer

- Vectorized engine with **no look-ahead bias** (signals at bar *t* execute at *t+1*)
- Realistic cost model: commission + spread + slippage per unit of turnover; gross-vs-net cost drag reporting
- **Volatility targeting** — position sizing scaled to target annualized vol for fair strategy comparison
- **Walk-forward out-of-sample validation**: rolling grid-search on train windows, OOS evaluation; demo correctly flags MA strategy as overfit (in-sample Sharpe ≈ 1.24 → OOS ≈ 0.11)
- Risk metrics: Sharpe, Sortino, Calmar, max drawdown, VaR & CVaR (95%); statistical significance: bootstrap Sharpe CI and Sharpe-difference test
- **Model-agnostic AI agent layer** — natural-language CLI driving the full system (Anthropic API / Ollama / mock)

**Stack:** `Python` `pandas` `NumPy` `yfinance` `ccxt` `SciPy`

---

### 🤖 [Telco Customer Churn Prediction Platform](https://github.com/saba-aslani/churn_prediction)
> Production-grade ML platform | AUC 0.851 | Recall 0.93 | Net ROI $84,220/cohort

- Engineered 27 features from 7,043 customer records; Stratified 5-Fold CV across LR, XGBoost, Random Forest
- Optimized decision threshold via **F2-score** (0.29 vs default 0.50): recall 0.79 → **0.93**; modeled cost asymmetry ($1,200 lost revenue vs $50 retention cost)
- **SHAP** explainability: top drivers — MonthlyCharges, fiber optic service, tenure, contract type
- 4-page **Streamlit** dashboard: KPI overview, customer explorer, live predictor, model performance
- 📊 **[Live App →](https://churnprediction-customer.streamlit.app/)**

**Stack:** `Python` `Scikit-learn` `XGBoost` `SHAP` `Plotly` `Streamlit` `Joblib`

---

### 🧠 [Customer Segmentation — RFM + ETL Pipeline](https://github.com/saba-aslani/Customer-Segmentation-RFM)
> Modular ETL + SQL analytics + Streamlit dashboard | 50,000+ transactions

- ETL pipeline processing 50,000+ retail transactions; RFM segmentation — top 20% driving 80% of revenue
- Advanced SQL: CTEs, window functions, revenue by segment, top customer ranking; stored in SQLite
- 📊 **[Live App →](https://customer-segmentation-rfm-earfpdvjqosyqkkacpjnpu.streamlit.app/)**

**Stack:** `Python` `SQLite` `SQL` `Streamlit` `pandas`

---

### 📊 [A/B Testing Analysis](https://github.com/saba-aslani/A-B-Testing-Analysis)
> Statistical experiment design | Power analysis | Two-proportion z-test

- Power analysis: 4,433 users/group at 80% power, α=0.05; removed 1,895 inconsistent-assignment users
- p-value = 0.2394 → no significant difference; recommendation: pivot to higher-impact tests

**Stack:** `Python` `SciPy` `statsmodels` `Seaborn`

---

### 🛒 [E-commerce Sales Analysis](https://github.com/saba-aslani/Ecommerce-Sales-Analysis)
> Advanced SQL on 540,000+ records | 35% query time reduction

- CTEs, window functions, aggregations across 540K+ records; 35% query execution time reduction
- Uncovered seasonal patterns driving 15% quarterly revenue spikes

**Stack:** `Python` `SQL` `SQLite` `Streamlit` `pandas`

---

### 📈 [SuperStore Sales Analytics — Power BI](https://github.com/saba-aslani/superstore-sales-powerbi)
> 51,000 orders | 7 markets | Star schema | 7 RLS roles | What-If simulator

- Star schema, 20+ DAX measures, 7 RLS roles, discount What-If simulator, 5-page executive report

**Stack:** `Power BI` `DAX` `Power Query (M)`

---

## 📫 Let's connect

[![Portfolio](https://img.shields.io/badge/Portfolio-saba--aslani.github.io-black?style=flat&logo=github)](https://saba-aslani.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Saba%20Aslani-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/saba-aslani)
[![GitHub](https://img.shields.io/badge/GitHub-saba--aslani-181717?style=flat&logo=github)](https://github.com/saba-aslani)
[![Live Dashboard](https://img.shields.io/badge/Canada%20Trade-Live-FF4B4B?style=flat&logo=streamlit)](https://canada-trade-gateway-dashboard.streamlit.app/)
