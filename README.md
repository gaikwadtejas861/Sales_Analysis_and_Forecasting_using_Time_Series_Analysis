# 📊 Sales Analysis & Forecasting using Time Series Analysis

## Overview

This project analyzes a synthetic e-commerce sales dataset to uncover business insights and forecast future sales using Time Series Analysis. The workflow includes data cleaning, exploratory data analysis (EDA), customer segmentation (RFM Analysis), and 12-month sales forecasting using the Holt-Winters Exponential Smoothing model.

The project demonstrates how historical sales data can be transformed into actionable business insights for inventory planning, marketing, customer retention, and demand forecasting.

---

## Dataset

- **Dataset:** Cleaned Synthetic E-commerce Sales Dataset
- **Records:** 100,000
- **Columns:** 21 (after feature engineering)
- **File Format:** CSV

### Key Features
- Order Date
- Revenue
- Product Category
- Region
- Customer ID
- Quantity
- Discount
- Customer Rating
- Month & Year (derived features)

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Jupyter Notebook

---

## Project Workflow

### 1. Data Cleaning
- Converted date columns into datetime format.
- Handled missing values and duplicate records.
- Verified revenue outliers using IQR and Z-score.
- Created Month and Month-Year features for trend analysis.

### 2. Exploratory Data Analysis
- Monthly and yearly sales trends
- Peak vs Low sales months
- Product category performance
- Regional revenue analysis
- Customer purchase behavior

### 3. Customer Segmentation
Performed **RFM (Recency, Frequency, Monetary) Analysis** to classify customers into:
- High Value Customers
- Loyal Customers
- At-Risk Customers
- Lost Customers
- New Customers
- Potential Loyalists
- Promising Customers

### 4. Sales Forecasting
- Aggregated transaction data into monthly revenue.
- Applied **Holt-Winters Exponential Smoothing**.
- Used:
  - Additive Trend
  - Additive Seasonality
  - Seasonal Period = 12 Months
- Forecasted sales for the next 12 months.

### 5. Model Evaluation
Model performance was evaluated using:
- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

---

## Results

### Key Business Insights

- Sales show a clear seasonal trend.
- November consistently generates the highest revenue.
- February records the lowest sales.
- Beauty and Home categories show strong growth potential.
- Oceania, Asia, and North America are the highest revenue-generating regions.
- Customer segmentation identified loyal, high-value, at-risk, and lost customer groups.
- The Holt-Winters model forecasts stable business growth while preserving seasonal patterns.

---

## Project Structure

```
Sales-Analysis-Forecasting/
│
├── Project.ipynb
├── synthetic_ecommerce_sales_2025.csv
├── cleaned_synthetic_ecommerce_sales_2025.csv
├── Customer_rfm_Analysis.csv
├── Future_Forecast_Summary.csv
├── Data Cleaning Report.pdf
├── Sales Forecasting Report Using Time Series Analysis.pdf
├── Sales Analysis & Forecasting Report.pdf
├── charts.pdf
└── README.md
```

---

## How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/Sales-Analysis-Forecasting.git
```

2. Move into the project folder

```bash
cd Sales-Analysis-Forecasting
```

3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn statsmodels jupyter
```

4. Launch Jupyter Notebook

```bash
jupyter notebook
```

5. Open `Project.ipynb` and run all cells.

---

## Future Improvements

- Implement ARIMA and Prophet models for comparison.
- Build an interactive Power BI or Tableau dashboard.
- Deploy the forecasting model using Streamlit or Flask.
- Automate monthly forecast generation.

---

## Author

**Tejas Pradeep Gaikwad**

**LinkedIn:** *www.linkedin.com/in/tejasgaikwad1608*

**GitHub:** *https://github.com/gaikwadtejas861*
