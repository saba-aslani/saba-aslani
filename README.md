# Hi, I’m Saba Aslani 👋

**Data Analyst & Data Engineer** | Python · SQL · Power BI · Machine Learning  
📍 Vancouver, BC  ·  🌐 [Portfolio](https://saba-aslani.github.io)  ·  🔗 [LinkedIn](https://linkedin.com/in/saba-aslani)  ·  📧 [aslanisaba2@gmail.com](mailto:aslanisaba2@gmail.com)

-----

Messy data in. Clear decisions out.

5+ years across operations, manufacturing, and retail — with an electrical engineering foundation that shows up in how I read signal from noise.

-----

## 🛠 Tech Stack

**Languages & Analytics**  
`Python` `SQL` `pandas` `NumPy` `Scikit-learn` `XGBoost` `SHAP` `SciPy` `statsmodels`

**Data Engineering**  
`PostgreSQL` `SQLite` `ETL Pipelines` `Data Cleaning` `Data Transformation`

**BI & Visualization**  
`Power BI` `DAX` `Power Query` `Tableau` `Streamlit` `Plotly` `Matplotlib` `Seaborn`

**Statistics & ML**  
`A/B Testing` `Hypothesis Testing` `Power Analysis` `EDA` `RFM Segmentation` `Predictive Modeling`

**Tools**  
`Git` `GitHub` `Jupyter Notebook` `VS Code` `Excel`

-----

## 🚀 Featured Projects

### 📉 [Quantitative Backtesting Framework](https://github.com/saba-aslani/quant-backtesting-framework)

> Research-grade backtesting engine for FX & crypto | Walk-forward validation | AI agent layer

- Built vectorized backtesting engine with **no look-ahead bias** (signals at bar *t* execute at *t+1*)
- Realistic cost model: commission + spread + slippage applied per unit of turnover; reports gross-vs-net cost drag
- **Volatility targeting** — position sizing scaled to target annualized vol for fair strategy comparison
- **Walk-forward out-of-sample validation** — rolling grid-search on train windows, evaluated on unseen OOS window; stitched OOS equity curve and IS-vs-OOS Sharpe gap (demo: in-sample Sharpe ≈ 1.24 collapses to OOS ≈ 0.11 → correctly flagged as overfit)
- Professional risk metrics: Sharpe, Sortino, Calmar, max drawdown, VaR & CVaR (95%), win rate, profit factor
- Statistical significance: paired t-test, bootstrap Sharpe CI, bootstrap Sharpe-difference test
- **Model-agnostic AI agent layer** — natural-language CLI driving the full backtesting system (Anthropic API / Ollama / mock)

**Stack:** `Python` `pandas` `NumPy` `yfinance` `ccxt` `SciPy`

-----

### 🤖 [Telco Customer Churn Prediction Platform](https://github.com/saba-aslani/churn_prediction)

> Production-grade ML platform | AUC 0.851 | Recall 0.93 | Net ROI $84,220/cohort

- Engineered 27 features from 7,043 customer records (IBM Telco dataset)
- Compared Logistic Regression, XGBoost, and Random Forest via **Stratified 5-Fold CV** — LR matched tree models (AUC 0.851 vs 0.850); preferred for production: faster inference, easier to audit
- Optimized decision threshold using **F2-score** (0.29 vs default 0.50): recall 0.79 → **0.93**, capturing $1,200 in lost revenue per churner vs $50 retention cost
- **SHAP** explainability: top drivers — MonthlyCharges, fiber optic service, tenure, contract type
- Deployed 4-page **Streamlit** dashboard: KPI overview, customer explorer, live predictor, model performance
- 📊 **[Live App →](https://churnprediction-customer.streamlit.app/)**

**Stack:** `Python` `Scikit-learn` `XGBoost` `SHAP` `Plotly` `Streamlit` `Joblib`

-----

### 🧠 [Customer Segmentation — RFM + ETL Pipeline](https://github.com/saba-aslani/Customer-Segmentation-RFM)

> End-to-end segmentation: ETL + SQL analytics + Streamlit dashboard | 50,000+ transactions

- Built modular ETL pipeline processing 50,000+ retail transactions
- Calculated RFM metrics; segmented customers into Champions, Loyal, Potential Loyalists, At-Risk — top 20% driving 80% of revenue
- Stored processed data in **SQLite**; advanced SQL analysis: CTEs, window functions, revenue by segment, top customer ranking
- Deployed interactive **Streamlit** dashboard with drill-down segment analysis and executive KPI views
- 📊 **[Live App →](https://customer-segmentation-rfm-earfpdvjqosyqkkacpjnpu.streamlit.app/)**

**Stack:** `Python` `SQLite` `SQL` `Streamlit` `pandas` `Matplotlib`

-----

### 📊 [A/B Testing Analysis — Website Layout Optimization](https://github.com/saba-aslani/A-B-Testing-Analysis)

> Statistical experiment design and hypothesis testing on real user behavior data

- Ran power analysis: 4,433 users/group required at 80% power, α=0.05
- Identified and removed 1,895 users with inconsistent group assignments to protect data integrity
- Performed **two-proportion z-test**; p-value = 0.2394 → no statistically significant difference
- Recommendation: design change is neutral — pivot to higher-impact tests

**Stack:** `Python` `SciPy` `statsmodels` `Seaborn` `Jupyter`

-----

### 🛒 [E-commerce Sales Analysis](https://github.com/saba-aslani/Ecommerce-Sales-Analysis)

> Advanced SQL analytics on 540,000+ records | 35% query execution time reduction

- Analyzed 540,000+ records using advanced SQL: CTEs, window functions, aggregations
- Uncovered seasonal patterns driving 15% quarterly revenue spikes
- Optimized complex queries, cutting database execution time by 35% for automated reporting
- Built interactive Streamlit dashboard for business stakeholder reporting

**Stack:** `Python` `SQL` `SQLite` `Streamlit` `pandas` `Matplotlib`

-----

### 📈 [SuperStore Sales Analytics — Power BI](https://github.com/saba-aslani/superstore-sales-powerbi)

> Senior-level BI report | 51,000 global orders | 7 markets | 2011–2014

- Star schema: 1 fact table + 5 dimension tables built in Power Query
- 20+ DAX measures: `TOTALYTD`, `SAMEPERIODLASTYEAR`, rolling 12-month revenue, custom DAX forecast
- **7 Row-Level Security (RLS)** roles, one per market (APAC, EMEA, EU, US, LATAM, Africa, Canada)
- What-If discount scenario simulator (0–50%) for executive scenario planning
- 5-page report: Executive Summary, Sales Performance, Customer Analytics, Product Intelligence, Forecasting

**Stack:** `Power BI` `DAX` `Power Query (M)`

-----

## 📌 Currently

- 🔭 Extending the quant backtesting framework with ML signal generation (XGBoost direction prediction)
- 🌱 Advancing SQL optimization: indexes, execution plans, query tuning
- 👀 Open to **Data Analyst**, **Data Engineer**, and **Quant Analyst** roles in Vancouver or remote

-----

## 📫 Let’s connect

[![Portfolio](https://img.shields.io/badge/Portfolio-saba--aslani.github.io-black?style=flat&logo=github)](https://saba-aslani.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Saba%20Aslani-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/saba-aslani)
[![GitHub](https://img.shields.io/badge/GitHub-saba--aslani-181717?style=flat&logo=github)](https://github.com/saba-aslani)
[![Streamlit](https://img.shields.io/badge/Churn%20App-Live-FF4B4B?style=flat&logo=streamlit)](https://churnprediction-customer.streamlit.app/)