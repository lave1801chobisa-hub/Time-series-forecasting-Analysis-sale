# Time-series-forecasting-Analysis-sale

📈 Time Series Sales Forecasting with SARIMA
Forecasting 24 months of champagne sales using classical time series modeling — built from scratch as a learning project.

📌 Project Overview
This project applies ARIMA and Seasonal ARIMA (SARIMA) models to predict future sales using the Perrin Frères monthly champagne sales dataset (1964–1972). The goal was to learn the full time series pipeline end-to-end.

📂 Dataset
PropertyDetailsSourcePerrin Frères Monthly Champagne SalesPeriodJanuary 1964 – September 1972Records105 monthsAvg Sales~4,761 units/monthPeak Sales13,916 units (December)

🔄 Project Workflow
Raw Data → Cleaning → Stationarity Test → Differencing → ACF/PACF Analysis → ARIMA → SARIMA → Forecast
Steps:

Data Cleaning — Renamed columns, dropped null rows, parsed dates as datetime index
Stationarity Testing — Augmented Dickey-Fuller (ADF) test confirmed non-stationarity
Seasonal Differencing — Applied lag-12 differencing to remove seasonality
ACF & PACF Analysis — Identified optimal p, d, q parameters
ARIMA Modeling — Built baseline model with order (1,1,1)
SARIMA Modeling — Upgraded to SARIMAX(1,1,1)(1,1,1,12) to capture 12-month seasonal cycles
Forecasting — Generated 24-month future sales predictions


📊 Key Insight

Champagne sales spike every December — almost like clockwork.
A plain ARIMA model missed this entirely. SARIMA captured it perfectly.

Seasonality is not noise — it's one of the most powerful signals in your data.
