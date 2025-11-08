# Retail Sales Forecasting (Time Series Analysis)

This project analyzes monthly retail sales data and builds a forecasting model to project future sales trends.  
The goal was to clean, prepare, visualize, and forecast retail sales over time using time series modelling techniques.

---

## 📊 Key Steps

1. **Loaded and inspected raw data**  
   Data: `data/raw/retail_sales.csv`

2. **Cleaned & Preprocessed the Data**
   - Converted dates to datetime format
   - Set date as index
   - Resampled to monthly frequency
   - Created **12-month rolling average** to smooth seasonal fluctuations  
   Output saved to: `data/processed/retail_sales_processed.csv`

3. **Visualized Sales Trend**
   - Created a Python line chart to show monthly patterns and seasonality
   - Created a Power BI dashboard visual comparing:
     - Raw sales values
     - 12-month rolling trend  
   Files:
   - `visuals/retail_sales_trend.png`
   - `visuals/retail_sales_trend_powerbi.png`

4. **Forecasting with Facebook Prophet**
   - Fitted a Prophet model on the processed dataset
   - Forecasted **24 months into the future**
   - Exported forecast visual  
   File: `visuals/retail_sales_forecast.png`

---

## 🛠 Tools Used
| Tool | Purpose |
|------|---------|
| Python (Pandas, Matplotlib) | Data cleaning & trend visualization |
| Prophet | Time Series Forecasting |
| Power BI | Dashboard visualization & trend reporting |
| Jupyter Notebook | Workflow + exploration |

---

## 📈 Results & Insights
- Clear yearly seasonality in monthly sales
- Long-term upward trend in retail demand
- Rolling average helps show real trend direction without month-to-month noise
- Forecast suggests **continued growth** over the next 24 months

---

## 🚀 Next Improvements
- Add ARIMA / SARIMA model for comparison
- Deploy forecast results to a Power BI dashboard with filters
- Create an automated pipeline to refresh future predictions monthly

---

## 📂 Project Structure
02-retail-forecasting/
│
├── data/
│ ├── raw/
│ │ └── retail_sales.csv
│ └── processed/
│ └── retail_sales_processed.csv
│
├── notebooks/
│ ├── 01_exploration.ipynb
│ └── 02_model_or_analysis.ipynb
│
├── visuals/
│ ├── retail_sales_trend.png
│ ├── retail_sales_trend_powerbi.png
│ └── retail_sales_forecast.png
│
└── README.md
