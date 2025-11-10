# RetailMind — Smart Demand Forecasting & Retail Dashboard

RetailMind is a **smart demand forecasting and sales analytics tool** designed for online retail businesses.  
It transforms transactional data into actionable insights, helping retailers optimize **inventory, purchasing, and operations**.

Dataset: Online Retail — UCI Machine Learning Repository (Dec 2010–Dec 2011)


## Features

### Time-Series Forecasting
- Supports **multiple forecasting models**:
  - ETS Additive / ETS Multiplicative
  - ARIMA (Seasonal & Non-seasonal)
- Automatically evaluates model performance using:
  - **RMSE, MAE, MAPE**
- Backtesting included

### Interactive Dashboard UI (mockup / wireframe)
- Sales Dashboard (Revenue, Orders per country, Forecast vs Actual)
- Orders page (pagination, status tracking)
- Inventory page (stock visibility & restock actions)

### Dashboard
![Dashboard](https://raw.githubusercontent.com/sunny22123/retail-forecasting-ml-dashboard/main/wireframe/1.png)

### Orders Page
![Orders](https://raw.githubusercontent.com/sunny22123/retail-forecasting-ml-dashboard/main/wireframe/2.png)

### Inventory Page
![Inventory](https://raw.githubusercontent.com/sunny22123/retail-forecasting-ml-dashboard/main/wireframe/3.png)

### Business Impact
- Prevent stockouts and overstocking
- Reduce forecasting guesswork
- Increase inventory turnover efficiency


## Architecture Overview

Online Retail Dataset (Raw CSV/XLSX)
Data Processing & Cleaning (Python / Pandas)
Time Series Forecasting (ETS / ARIMA / Prophet tested)
Model Evaluation (MAPE / RMSE / MAE)
Dashboard Visualization (Figma wireframe → interactive UI later)


## Models & Evaluation

| Model            | Seasonality | Result |
|------------------|-------------|--------|
| **ETS Additive** | Yes       | Best performance |
| ARIMA Seasonal   | Yes       | Good but less consistent |
| ARIMA Non-seasonal | No     | Moderate |
| ETS Multiplicative | Yes    | Performs poorly on this dataset |

![Result](https://github.com/sunny22123/retail-forecasting-ml-dashboard/blob/main/result_1.png)

> **ETS Additive consistently outperformed all other models** across revenue, product-level demand, and order count forecasting.

## Output examples

- Weekly revenue forecasting
- Per product demand forecasting (top-selling SKUs)
- Order volume forecasting for resource planning

Screenshots of visualizations are included in the `/dashboard` folder.


## Tech Stack

| Area | Technology |
|------|------------|
| Data processing | Python, Pandas |
| Forecasting Models | Statsmodels, pmdarima, Prophet (test candidate) |
| Visualization | Matplotlib, Seaborn |
| Dashboard | Figma (UI concept), future: Streamlit / React |


## 👥 Team

**Team 2 — Time Series Forecasting Project, Carnegie Mellon University**  



