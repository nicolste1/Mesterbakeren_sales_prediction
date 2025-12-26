# Sales Predictor using Meta Prophet

A time series forecasting tool designed to predict daily sales trends by leveraging Meta’s Prophet model and data preprocessing.


## 📊 Data Preprocessing
Before modeling, the raw daily CSV data undergoes a transformation pipeline to ensure the **Principle of Equal Contribution**:

* **Schema Mapping:** Standardizing the dataset into `ds` (datestamp) and `y` (target sales value) for Prophet compatibility.
* **Feature Engineering:** Injecting a **Custom Holiday DataFrame** to capture specific local events and payday cycles that impact sales volume.



## 📈 Modeling & Evaluation
The Prophet model decomposes the daily sales signal into its core components:

* **Trend:** Capturing long term growth trajectories.
* **Daily Seasonality:** Optimizing for daily granularity to identify weekly cycles.
* **Uncertainty:** Generating `yhat_upper` and `yhat_lower` confidence intervals.

### Performance
The model achieved a **MAPE (Mean Absolute Percentage Error) of 10.41%**, indicating high predictive accuracy for the target sales period.
<img width="654" height="436" alt="Skjermbilde 2025-12-23 234008" src="https://github.com/user-attachments/assets/867500a5-4cd8-4fb9-b621-3a4a2b952b35" />
