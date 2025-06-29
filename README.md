# Retail-Sales-Analytics-with-Medallion-Architecture-Azure-ML-
This project implements a full-stack retail analytics solution using Azure cloud and open-source ETL/ML tools. It follows the Medallion Architecture (Bronze → Silver → Gold) and provides actionable insights for sales forecasting, customer segmentation, churn prediction, and recommendations.


- **Bronze:** Raw retail data ingested from Azure Blob Storage.
- **Silver:** Cleaned and transformed data stored as Parquet.
- **Gold:** Machine learning outputs including forecasting and segmentation.

---

## Technologies Used

- **Cloud:** Azure Blob Storage, Azure Data Factory (optional)
- **ETL Tools:** Databricks (Community), Python (pandas, pyarrow)
- **ML Libraries:** Prophet, ARIMA, XGBoost, Scikit-Learn, HDBSCAN
- **Storage Format:** CSV / Parquet (Gold Layer)
- **IDE:** Visual Studio Code / Jupyter

---

## Data Source

- **Dataset:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
- **Format:** CSV → Parquet
- **Location:** Uploaded to Azure Blob Storage in folders:
  - `ecommerce-data/bronze`
  - `ecommerce-data/silver`
  - `ecommerce-data/gold`

---

## Data Engineering Pipeline

1. **Bronze Layer:**
   - Raw data uploaded to Blob Storage
2. **Silver Layer:**
   - Data cleaning (nulls, duplicates, missing values)
   - Type conversions, calculated fields (TotalAmount = Quantity × UnitPrice)
3. **Gold Layer:**
   - RFM Calculation + Segmentation (KMeans, GMM, HDBSCAN)
   - Sales Forecasting (Prophet, ARIMA, XGBoost)
   - Customer Churn or High-Value Prediction *(in progress)*
   - Product Recommendation Engine *(in progress)*

---

## Completed So Far

- ✅ Customer Segmentation with KMeans, GMM, HDBSCAN
- ✅ Prophet-based Daily Sales Forecast
- ✅ ARIMA Forecast (with comparison)
- 🔄 XGBoost Forecast *(next)*
- 🔄 Churn Prediction *(planned)*
- 🔄 Recommendation Engine *(planned)*

---

## Outputs (Gold Layer)

- `customer_segments.csv`
- `daily_sales_forecast.csv`
- `arima_forecast.csv`
- *(More to be added)*

---

## Next Steps

- Implement XGBoost forecasting
- Build classification model for churn prediction
- Train item-based recommendation model

---

## Author

**Palash Sharma**  
Business Insights & Analytics | Azure | Power BI | Python | ML  
🇨🇦 Based in Canada | Humber College

---

> ⭐ If you're viewing this on GitHub, feel free to fork or contribute!
